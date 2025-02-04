Installation Guide
===================

.. _installation:

This tutorial will briefly introduce the basic tools you are going to use throughout this course and how to install
them. The tools are essential for the homeworks and projects so please make sure you grasp the basic ideas
and all the tools are good to go after you follow this guide.

You will need to use `ROS2 <https://docs.ros.org/en/humble/index.html>`_ (Robot Operating System). ROS2 is easier to install and run in Linux-like
systems. So this tutorial will only introduce how to install ROS2 HUmble on Ubuntu 22.04.5 Jammy Jellyfish. You are free to use other version of ROS2 if you are familiar with this framework (all variants of ROS2
share the same coding conventions). There are three ways to install Ubuntu on your pc: Virtual Machine, Dual-boot, and WSL (Windows Subsystem for Linux).

Virtual Machine ``recommended``
--------------------------------

1. Download an Ubuntu Image

You can download an Ubuntu image `here <https://releases.ubuntu.com/jammy/>`_. Make sure to save it to a memorable location on your PC! For this tutorial, we will use the latest Ubuntu 22.04.5 LTS (long term support) release.

.. image:: images/iso.png
   :width: 600

2. Download and install VirtualBox

You can download VirtualBox from the `downloads page <https://www.virtualbox.org/wiki/Downloads>`_. Follow instructions on how to install VirtualBox for your specific OS. 
Once you have completed the installation, go ahead and run VirtualBox.

.. image:: images/virtualbox.png
   :width: 600

3. Create a new virtual machine

Click New to create a new virtual machine. Fill in the appropriate details:

    - Name: If you include the word Ubuntu in your name the Type and Version will auto-update.
    - Machine Folder: This is where your virtual machines will be stored so you can resume working on them whenever you like.
    - ISO Image: Here you need to add a link to the ISO you downloaded from the Ubuntu website.

.. image:: images/virtual_step1.png
   :width: 600

4. Create a user profile

To enable the automatic install we need to prepopulate our username and password here in addition to our machine name so that it can be configured automatically during first boot.

The default credentials are:

    - Username: vboxuser
    - Password: changeme

It is important to change these values since the defaults will create a user without sudo access.

.. note::
    Ensure your Hostname has no spaces to proceed!

.. image:: images/virtual_step2.png
   :width: 600