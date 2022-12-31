---
title: "Home Server"
date: 2022-12-27T22:29:18-05:00
draft: true
type: page
---

Since I've been into computers the idea of making a NAS was on my radar, but never saw the use of it until I got around to starting a media server using my laptop. Space started filling up quickly and the idea of a home lab server came up again. At the same time, one of my friends upgraded a bunch of his computer and he wanted to sell parts for cheap. Everything lined up so I decided I would build my own server.

Here are the components I'm working with:
- CPU: INTEL i7-6700K
- COOLER: Cooler Master Hyper 212 Black Edition
- GPU: ________ GTX 1070
- RAM: Vengenance LPX DDR4 2400 MHz [8 GB x 2]
- MOBO: ASUS Z170-A
- PSU: Corsair RM 550x
- CASE: Cooler Master N400
- STORAGE: WD Black NVMe SSD [1 TB] + 2 x WD Red [4 TB]

I am using Proxmox as my virtualization management system. Within Proxmox, I'm running 3 virtual machines:
1. TrueNAS - my NAS
2. Windows - to run some services
    1. Jellyfin - media server
    2. Transmission - torrent client
    3. Sonarr - internet PVR
    4. Jackett - indexer
    4. ProtonVPN - VPN service
3. Pihole - to be my local DNS server

Here are the steps I followed:
1. I built the computer. 
*insert pictures*
2. Next, in the bios...
3. I installed Proxmox using a USB key
4. Created the TrueNAS vm
5. Created the Windows VM
6. Installed all the services on the Windows VM
7. Installed Pihole and setup the local DNS



