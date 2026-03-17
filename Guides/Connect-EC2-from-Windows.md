Guide: Connecting to EC2 Instance from Windows (Using MobaXterm)
Introduction

Many beginners face difficulties connecting to an EC2 instance from a Windows machine.

Common issues include:

Confusion with PuTTY configuration

Difficulty converting .pem files to .ppk

Using the AWS browser terminal instead of SSH

This guide explains a simple method to connect to an EC2 instance using MobaXterm, which works directly with .pem keys.

Benefits of this method:

No PuTTY configuration needed

No Linux VM required

Easy SSH connection from Windows

Goal of This Guide

After following this guide you will be able to:

Launch an EC2 instance

Install MobaXterm

Connect to the EC2 instance from a Windows laptop

The whole process usually takes less than 5 minutes.

Launch an EC2 Instance

Go to the AWS console and open the EC2 service.

Click Launch Instance.

Example configuration:

Instance Name: test-windows

Operating System: Ubuntu

Instance Type: t2.micro

This will create a Linux virtual machine.

Create a Key Pair

While creating the instance, create a new key pair.

Example:

Key Pair Name:

windows-demo

Settings:

Encryption: RSA

File Format: .pem

Important:

.pem files work directly with MobaXterm.

.ppk files are required only if using PuTTY.

The key file will automatically download to your Downloads folder.

Network Settings

Ensure the following settings are enabled:

Public IP enabled

SSH access allowed

Port 22 open

These settings allow remote SSH access to the instance.

Launch the Instance

Click Launch Instance.

AWS will create the EC2 instance.

Wait until the instance status becomes Running.

Download MobaXterm

Open a browser and search:

Download MobaXterm

Download it from the official website.

Choose:

Community Edition (Free)

Choose Installation Type

Two options will appear:

Portable Version

Installer Version

Recommended:

Installer Version

This installs the software properly on your system.

Install MobaXterm

Steps:

Open the Downloads folder

Right-click the ZIP file

Select Extract All

After extraction:

Open the extracted folder

Double-click the installer

Click Next

Accept the license

Click Install

Click Finish

Now MobaXterm is installed.

Open MobaXterm

Open Windows Search.

Type:

MobaXterm

Open the application.

Get EC2 Public IP

Go to the AWS Console.

Navigate to:

EC2 → Instances

Copy the Public IP Address.

Example:

3.110.xxx.xxx
Create SSH Session

Inside MobaXterm:

Click Session

Select SSH

Enter:

Host Name:

EC2 Public IP

Example:

3.110.xxx.xxx
Provide Username

For Ubuntu instances, the default username is:

ubuntu

Enter this as the SSH username.

Add Private Key

Configure SSH authentication.

Steps:

Click Advanced SSH Settings

Enable Use Private Key

Browse to your Downloads folder

Select the .pem key file

Example:

windows-demo.pem

Click OK.

Connect to the Instance

When connecting for the first time, a security popup will appear.

Click:

Accept

MobaXterm will authenticate using the .pem key.

Successful Connection

If everything is correct, the Linux terminal will open.

You are now connected to your EC2 instance.

Test command:

sudo apt update

If the command runs successfully, the connection is working.

Tools Used
Tool	Purpose
AWS EC2	Create virtual machine
Key Pair (.pem)	Authentication
MobaXterm	SSH connection from Windows
Result

You have successfully connected to an EC2 Linux instance from a Windows machine using MobaXterm.

This method avoids using:

PuTTY

AWS browser terminal

VirtualBox

Linux virtual machines 