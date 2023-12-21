

#                                                                          HumansBestFriend App

# Introduction
HumansBestFriend is a simple, distributed application designed to run across multiple Docker containers. It integrates various technologies including Python, Node.js, .NET, Redis, and Postgres. This README provides a step-by-step guide for setting up and running the application.

# Table of Contents
Requirement
Getting Started
Architecture
Setup Guide
Prerequisites
Building the Application
Running the Application
Services
Worker Service
Vote Service
Seed Data Service
Result Service
Deployment
Notes
Submission
# Requirement
The project must be run inside a virtual machine that supports Docker and Docker Compose.
Getting Started
This solution uses Python, Node.js, .NET, with Redis for messaging and Postgres for storage.

# Architecture
Architecture Diagram
![image](https://github.com/Karima-brb/Docker-Project/assets/115697807/9422a5f6-78a3-4499-8027-30717130776f)

# Setup Guide
#Installation et Configuration:
- Mise à jour des paquets existants : 
sudo apt install docker-compose
-  Installation de Docker Compose :
  sudo apt install docker-compose 
Docker and Docker Compose installed. Refer to the Docker documentation for installation instructions.

# Building the Application
- Construire les images :
docker-compose -f docker-compose.build.yml build --no-cache,
docker compose up

# Vote Service
docker tag humans-bets-friend_vote localhost:5000/r_vote:v1,
docker push localhost:5000/r_vote:v1


# Seed Data Service
docker tag humans-best-friend_seed-data localhost: 5000/r_seed:v1,
docker push localhost:5000/r_seed:v1


# Result Service
docker tag humans-best-friend_result localhost: 5000/r_result:v1,
docker push localhost:5000/r_result:v1

- Vérification du Registre :
curl localhost:5000/v2/_catalog 

# Services
Worker Service
- Envoi des Images au Registre Docker 
docker tag humans-best-friend_worker localhost:5000/worker:v1

- Poussée de l'Image vers le Registre Local 
docker push localhost:5000/worker:v1 

# Deployment
Instructions and notes about deploying the application, including setting up the network and dealing with Docker registries.

# Notes
Additional notes and limitations of the HumansBestFriend application.

# Submission
Ensure that the deployment is done inside a network called humansbestfriend-network.
