Installation Script for Docker and Associated Tools
This script helps you install Docker-CE, Docker-Compose, NGinX Proxy Manager, Navidrome, recurring internet Speedtest, and Portainer-CE on various Linux distributions. The script supports CentOS, Debian, Ubuntu, and Arch Linux.

Features
Docker-CE: Community Edition of Docker
Docker-Compose: A tool for defining and running multi-container Docker applications
NGinX Proxy Manager: A Docker container for managing proxy hosts
Navidrome: Music streaming server
Recurring Internet Speedtest: Regularly tests and logs internet speed
Portainer-CE: A lightweight management UI for Docker, Swarm, and Kubernetes
Prerequisites
This script requires root or sudo privileges.
Ensure your system is connected to the internet.
Supported Operating Systems
CentOS 7 and 8
Debian 10 (Buster) / 11 (Bullseye)
Ubuntu 18.04 (Bionic) / 20.04 (Focal) / 21.04 (Hirsute) / 22.04 (Jammy)
Arch Linux
Usage
Download the Script: Save the script to your desired location.
Make the Script Executable: Run chmod +x <script_name>.sh to make the script executable.
Run the Script: Execute the script by running ./<script_name>.sh.
Script Workflow
OS Detection: The script will detect your operating system and prompt you to select the appropriate one.
Installation Prompts: You will be asked to confirm the installation of various components.
Docker-CE
Docker-Compose
NGinX Proxy Manager
Navidrome
Speedtest
Portainer-CE (with options for full Portainer or Portainer Agent)
Installation Process: The script installs the selected components and provides progress updates.
Components Installation Details
Docker-CE
The script checks if Docker-CE is already installed and running. If not, it will prompt you to install it. For Debian and Ubuntu, it installs using the Docker repository. For CentOS and Arch Linux, it uses the Docker installation script.

Docker-Compose
If Docker-Compose is not installed, the script installs it using the package manager for Debian/Ubuntu and a direct download for CentOS.

NGinX Proxy Manager
The script sets up a directory for NGinX Proxy Manager and downloads a default docker-compose.yml file. It then starts the container using Docker Compose.

Navidrome
The script sets up a directory for Navidrome, downloads the necessary docker-compose.yml, and starts the container.

Speedtest
The script sets up a directory for Speedtest, downloads the docker-compose.yml, and starts the container.

Portainer-CE
The script offers to install either the full Portainer-CE or just the Portainer Agent. It sets up the necessary Docker volumes and starts the containers.

Notes
If you install Docker-CE, the script will add your user to the Docker group. You will need to log out and log back in for the changes to take effect.
Ensure that Docker is running after installation. The script will attempt to start the Docker service if it is not active.
Troubleshooting
Permissions: Ensure the script is executable and you have the necessary permissions.
Internet Connection: Verify that your system has an active internet connection.
Dependencies: Ensure that curl and other required tools are installed on your system.
For further assistance, refer to the official documentation of each tool or consult community forums.