# Docker Lab: Containerizing a Three-Tier Application
**INET 4031 - Introductions to Systems**

This lab introduces Docker and Docker Compose by having you containerize a
real, multi-service application. You will package three components: Apache,
Flask, and MariaDB. These will be packaged into separate containers and wired together so they function as a complete application.

The application code and scaffolding are provided. Your job is to complete the Dockerfiles, verify the stack runs correctly, and document your work below.

> **Directions and explanations for this lab are on the repository Wiki.**
> Refer to the Wiki pages for step-by-step instructions.

---

*The sections below are for you to fill out. Replace each placeholder with your own content before submitting. Having a detailed README is the best practice for showing your work in future GitHub repositories.*

---

# Project Overview

<!-- Briefly describe what this application does in your own words.
     What problem does it solve? What does a user interact with? -->
     This is simply a ticket system which is made up of three components, The web server, the brain of the application, and the storage.
     Web: Apache.
     Brain: Flask.
     Storage: MariaDB.

# Prerequisites

<!-- List what needs to be installed or configured on the VM before this lab
     will work. Include Docker, Docker Compose, and anything else required. -->
     Ensure the system is ready for Docker, please install Docker and Docker Compose on the system. Also make sure your user account is also added into the docker group to ensure a smooth experience running commands without any forms of errors. Important: make sure port 80 is not being used during the process.

# Getting Started

<!-- Explain how a new teammate would bring this stack up from a fresh clone.
     Walk through every command they need to run, in order. -->
     Create a new configuration file by copying the example and adding your own passwords, when set, stop apache, or the host's apache service to ensure the port is open for the container. Once these steps are fulfilled, run the build and up command for the containers. If possible, there should be permission issues, refresh the session permissions using newgrp command.

# Configuration

<!-- Explain the .env file: what it is, what variables it contains,
     and what a teammate needs to provide that is not in this repository. -->
     The .env file is used to store any classified passwords and the settings for connections, due to the file being separate, the information will stay safe and will never be uploaded publically in the github repository. The variables are kept secretive.

# Verification

<!-- Describe how to confirm the stack is running correctly.
     Reference the check script and what a passing run looks like. -->
     Confirm everything works by checking the status of the containers in your terminal. Ensure the curl command also checks on the health endpoint. Finally, open the browser for the VM's IP address and verify the green health status is on and there is at least 2 tickets on the dashboard.

# Feedback (Optional)

<!-- Do you have any feedback you would like to give us after completing this lab? What are some things you enjoyed? What about others that you felt was lackluster? Or maybe there was something that we missed that you'd love for us to touch on! This will help us improve the INET 4031 lab experience. We appreciate everything we can get!  -->

No feedback.
