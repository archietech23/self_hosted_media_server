# Self Hosted Media Streaming Server Hosted on Raspberry Pi 4

![https://logos-world.net/wp-content/uploads/2021/02/Docker-Logo.png](https://www.docker.com/wp-content/uploads/2022/03/horizontal-logo-monochromatic-white.png)
![plex logo](https://upload.wikimedia.org/wikipedia/commons/thumb/7/7b/Plex_logo_2022.svg/320px-Plex_logo_2022.svg.png)

</br>
This repository contains a self-hosted personal streaming service powered by Docker and Plex. It is inspired by a guide I found on Reddit: https://www.reddit.com/r/Piracy/comments/pqsomd/the_complete_guide_to_building_your_personal_self/

## Project Overview
The main objective of this project is to apply my theoretical knowledge of Linux and Linux kernels, features such as cgroups, Union File Systems (UFS), and namespaces. By leveraging Docker and Plex, I aim to create an efficient and isolated streaming environment for my personal media content.

## Prerequisites
Before running this project, ensure you have the following installed on your system:

1. Docker
2. Docker Compose

## Getting Started
To set up the personal streaming service, follow these steps:

1. Clone this repository to your local machine:
```
git clone https://github.com/archietech23/self_hosted_media_server.git
```
2. Navigate to the project directory:
```
cd self_hosted_media_server/media-streaming
```
3. Customize the docker-compose.yml file to suit your preferences, such as media directories, Plex settings, Qbittorrent, etc.

4.Start the containers:
```
docker-compose up -d
```
5. Access Plex by opening your browser and navigating to http://localhost:32400/web. Follow the Plex setup wizard to configure your media libraries.

Enjoy your personal streaming service with Plex!

## Notes: 
- I used Prowlarr instead of jacket as I'm primarily interested in Usenet indexers
- I'll advice you to setup a VPN as well for privacy and security concerns. I used my self hosted wireguard VPN instead of OpenVPN 
- Make sure to follow the configuration of default save paths on Qbittorrent's part
- I used pihole instead of AdguardHome as I'm more familiar with using pihole
