

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

Architecture
Architecture Diagram
![image](https://github.com/Karima-brb/Docker-Project/assets/115697807/9422a5f6-78a3-4499-8027-30717130776f)

Description of the architecture and its components.

Setup Guide
Prerequisites
Docker and Docker Compose installed. Refer to the Docker documentation for installation instructions.
Building the Application
Worker Service
Instructions for setting up the Worker service.

Vote Service
Instructions for setting up the Vote service.

Seed Data Service
Instructions for setting up the Seed Data service.

Result Service
Instructions for setting up the Result service.

Running the Application
Steps to run the application once all services are set up.

Services
Worker Service
Details about the Worker service.

Vote Service
Details about the Vote service.

Seed Data Service
Details about the Seed Data service.

Result Service
Details about the Result service.

Deployment
Instructions and notes about deploying the application, including setting up the network and dealing with Docker registries.

Notes
Additional notes and limitations of the HumansBestFriend application.

Submission
Ensure that the deployment is done inside a network called humansbestfriend-network.
