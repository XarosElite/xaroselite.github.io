---
title: "Playhub Project"
date: 2024-12-08T20:16:03Z
draft: false
toc: false
images:
tags:
  - untagged
---


# 🚀 Project Title: Playhub

> _A Modern Gameserver Manager Built off of Docker._

---

## 📌 Table of Contents

- [Introduction](#introduction)
- [Motivation](#motivation)
- [Goals](#goals)
- [Tech Stack](#tech-stack)
- [Architecture Overview](#architecture-overview)
- [Key Features](#key-features)
- [Setup Instructions](#setup-instructions)
- [Screenshots / Demos](#screenshots--demos)
- [Challenges Faced](#challenges-faced)
- [Lessons Learned](#lessons-learned)
- [What's Next?](#whats-next)

---

## 🧠 Introduction {#introduction}


Playhub is a full stack web application built to be ran and deployed on debian. Once deployed it allows users to get on a web portal and spin up supported game servers to their hearts desire.

---

## 💡 Motivation {#motivation}

The motivation behind playhub started because my friend's and I tend to play lots of multiplayer server based video games. Since I was often the one manually setting up and hosting these game servers for my friends it became a level of work to set them up and manage them every time. Thus the idea to create a web application for my friends to be able to self service themselves to spin up game servers.

---

## 🎯 Goals {#goals}

This project was a colaboration between a friend and I. Our goals with this project were:

- Learn / Improve React front end skills
- Learn / Improve Flask back end skills
- Be able to spin up the project in production
- Allow users to Configure and Create Game Servers with the click of a button

---

## 🛠️ Tech Stack {#tech-stack}


| Purpose         | Technology            |
|----------------|------------------------|
| Frontend        | React w Typescript |
| Backend         | Flask |
| Database        | Redis Queue |
| Hosting         | Personal Proxmox Cluster in Homelab |
| Dev Tools       | Nix-shell, Docker |

---

## 🧱 Architecture Overview {#architecture-overview}


The Architecture of Playhub is fairly simple. The main components you have are a React front end web app based off of Mantine UI. Which communicates to our Flask Backend API that has access to our Redis Queue to start and check on "Jobs". These "Jobs" interact with docker to then bring up/down containers that host a game server.


---

## ✨ Key Features {#key-features}


Highlight the main features your project supports.

- ✅ Real time server CPU/RAM usage updates
- ✅ Create a game server (Curretly supports Minecract, Palworld)
- ✅ Delete a game server
- ✅ Restart a game server
- ✅ Deployable as a Systemd Service 

---

## 📸 Screenshots / Demos {#screenshots--demos}
### Come See for yourself!
![PlayhubHome](/img/PlayhubHome.png)
- Here you see the main Dashboard page of playhub
- This is where you can see the load on your system as well as manage your game servers!

![PlayhubSysInfo](/img/PlayhubDemo/PlayhubSystemInfo.png)
- The System Info Polls an endpoint every few seconds to report the CPU % load as well as the total RAM usage!

![PlayhubAddServer](/img/PlayhubDemo/PlayhubAddServer.png)
- To start a new game server all you have to do is hit the ***Add Server*** button and presto! You can start setting up your first game server. 
 
![PlayhubAddServerDrop](/img/PlayhubDemo/PlayhubServerDrop.png)
- Right now we only support two types of game servers but hope to support more in the future
- All you have to do is choose the game you want to setup though

![PlayhubMiecraftServer](/img/PlayhubDemo/PlayhubMinecraftServer.png)
- After you select your game we allo you to customize it!
- The customization depends on the type of game server but for Minecract you can customize:
    * Game Mode
    * Server Name
    * World Seed
    * Max Play Count
    * Server Port
    * PvP Mode
    * Hardcore Mode
    * Command Block Enable

![PlayhubMinecraftFilled](/img/PlayhubDemo/PlayhubMinecraftFilled.png)
- Once you fill out what you want you can hit Submit and it will create your game server!

![PlayhubPopulatedServers](/img/PlayhubDemo/PlayhubPopulatedServers.png)
- Now on the Main page you should see your server populate and spin up!
- You can see the ***Name***, ***Type***, and ***State*** of each server in the list

![PlayhubServerExpanded](/img/PlayhubDemo/PlayhubServerExpanded.png)
- You can select and expand any server on the list to see more settings and options for it such as:
    * Creation Date
    * IP and Port
    * Restart
    * Delete
    * Up/Down Toggle

![PlayhubServerOptions](/img/PlayhubDemo/PlayhubServerOptions.png)
- Right now we only have basic functionality for managing the servers such as restarting, deleting, and bringing up/down the servers.

![PlayhubRestart](/img/PlayhubDemo/PlayhubRestart.png)
- When you ***Restart*** a server you will see a loading wheel while the server is in the process of being restarted or really any time the container is being changed.

![PlayhubDelete](/img/PlayhubDemo/PlayhubDelete.png)
- When deleting a server it was important to us to give the user a warning to make sure they wanted to delete the server as we curretly have no safety to restore this.

![PlayhubToast](/img/PlayhubDemo/PlayhubToast.png)
- When deleting a server or performing any action such as creating, deleting, or restarting you will get a toast notification on completion telling you the task completed correctly

---

## Lessons Learned {#lessons-learned}

- 

---

## What's Next? {#whats-next}

---



