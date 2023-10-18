# Configuring Virtual Machines with Vagrant and Docker

This guide explains how to set up virtual machines using Vagrant and install Docker on two virtual machines. Vagrant is a tool that allows you to create and manage virtualized development environments. In this example, we are configuring two virtual machines with the Ubuntu 22.04 operating system and installing Docker on them.

## Prerequisites

Before you begin, make sure you have the following software installed on your machine:

- [Vagrant](https://www.vagrantup.com/downloads.html)
- [VirtualBox](https://www.virtualbox.org/)

## Steps

Follow these steps to configure the virtual machines and install Docker:

1. **Clone the Repository:** Clone the repository where you have your Vagrant configuration files and Docker installation script.

2. **Define Vagrant Configuration:**

   Open the `Vagrantfile` in your favorite text editor and paste the code you provided. This file defines the configuration of the virtual machines, including the amount of memory, CPUs, the operating system image, and the machine name.

   Make sure to adjust the settings as needed, such as the machine names, the amount of memory, and CPUs you want to allocate.

3. **Create and Start the Virtual Machines:**

   Open a terminal and navigate to the directory containing the `Vagrantfile`. Execute the following command to create and start the virtual machines:

   ```bash
   vagrant up

This will initiate the process of creating and configuring the virtual machines.

### 1 - Install Docker:

The virtual machines will be provisioned with Docker already installed using the install-docker.sh script. This script automatically downloads and installs Docker.

### 2 - Access the Virtual Machines:

After the process is complete, you can access your virtual machines using the vagrant ssh command followed by the machine name. For example, to access "node01":

bash
Copy code
vagrant ssh node01
You will be inside the virtual machine where Docker is already installed and ready to use.

### 3 - How to Use:

Now you can run Docker containers and perform development or testing as needed on your configured virtual machines.

### 4 - Shut Down Virtual Machines:

When you're done using your virtual machines, you can shut them down with the following command:

bash
Copy code
vagrant halt


## This will power off the virtual machines, conserving your computer's resources.

### *Additional Notes*

* You can further customize the Vagrant configuration to meet your needs, such as adding more virtual machines, changing network settings, and more.

* Ensure that Vagrant and VirtualBox are installed and functioning correctly on your machine before running the above steps.

* You now have a development environment set up with Docker on your virtual machines, ready for use. Enjoy!