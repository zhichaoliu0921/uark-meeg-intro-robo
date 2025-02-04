CoppeliaSim
===================


Installation on ``Ubuntu 22.04``
----------------------------------

1. **Download file**

Go to the `website <https://www.coppeliarobotics.com/>`_ and download the CoppeliaSim ``EDU``

.. image:: images/coppelia_install_step1.png
   :width: 600

Select the ``Ubuntu 22.04 [x86_64]`` and download

.. image:: images/coppelia_install_step2.png
   :width: 600

When the download is done, you can find a file ``CoppeliaSim_Edu_V4_9_0_rev2_Ubuntu22_04.tar.xz`` in the Folder ``Downloads``

2. **Extract file**

Right click the downloaded file and choose ``Extract Here``, and wait until the extraction is done. It might take a few minutes. 

.. image:: images/coppelia_install_step3.jpg
   :width: 600

3. **Run the Simulation**

Enter (Left click) the folder ``CoppeliaSim_Edu_V4_9_0_rev2_Ubuntu22_04``. Right click and choose ``Open in Terminal``. You will see a terminal like

.. image:: images/coppelia_install_step4.png
   :width: 600


Run the command

.. code-block:: console

    ./coppeliaSim.sh

You will see the simulator launching, and you are ready to use it.

.. image:: images/coppelia_install_step5.png
   :width: 600

Using Python
--------------

1. In a new terminal, Type

.. code-block:: console

   pip install cbor pyzmq


2. After the installation, re-open the CoppeliaSim and you will be asked to choose between ``Lua`` and ``Python``. Select ``Python``.

.. image:: images/coppelia_sim_python.png
   :width: 600


Using ROS 2 
------------

Make sure you have installed ROS2 Humble, created and sourced the workspace ``~\ros2_ws`` as shown in `Ubuntu and ROS2 Installation Guide <install.html>`_. 

1. **Enable ROS2 Plugin in CoppeliaSim**

In the input of ``Sandbox (python)`` at the very bottom, copy, paste and press ``enter`` on the keyboard 


.. code-block:: console

   simROS2 = require('simROS2')

.. image:: images/coppelia_ros2_step1.png
   :width: 600

You will see output in the background terminal as

.. image:: images/coppelia_ros2_step1_out.png
   :width: 600

So the plugin was successfully loaded.

2. **Install 2 ROS2 Packages**

