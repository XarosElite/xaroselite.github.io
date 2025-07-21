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
- [Links & Resources](#links--resources)

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

## 🧱 Architecture Overview {#architecture overview}


The Architecture of Playhub is fairly simple. The main components you have are a React front end web app based off of Mantine UI. Which communicates to our Flask Backend API that has access to our Redis Queue to start and check on "Jobs". These "Jobs" interact with docker to then bring up/down containers that host a game server.


---

## ✨ Key Features {#key-features}


Highlight the main features your project supports.

- ✅ Real time server CPU/RAM usage updates
- ✅ Create a game server (Curretly supports Minecract, Palworld)
    * Server Name
    * Server Settings
- ✅ Delete a game server
- ✅ Restart a game server
- 

---

