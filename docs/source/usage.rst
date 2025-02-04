Usage
=====

.. _installation:

Installation
------------

To use Lumache, first install it using pip:

.. code-block:: console

   (.venv) $ pip install lumache

Creating recipes
----------------

To retrieve a list of random ingredients,
you can use the ``lumache.get_random_ingredients()`` function:

.. autofunction:: lumache.get_random_ingredients

The ``kind`` parameter should be either ``"meat"``, ``"fish"``,
or ``"veggies"``. Otherwise, :py:func:`lumache.get_random_ingredients`
will raise an exception.

.. autoexception:: lumache.InvalidKindError

For example:

>>> import lumache
>>> lumache.get_random_ingredients()
['shells', 'gorgonzola', 'parsley']


Download an Ubuntu Image
------------

To install ROS2, first you need a computer that runs Ubuntu 22.04 operating system. If your computer runs
Windows or MacOS, you can either use method 1: dual-boot your machine, or method 2: use virtual
machine on your PC. For both methods, you need to download a ISO file for Ubuntu. Here is the link:
https://releases.ubuntu.com/jammy/
Please select the 64-bit PC (AMD64) desktop image to download.

.. note::
    If you are using macOS Applie Silicone (M1/M2), you may need to download ARM64 version https://cdimage.ubuntu.com/releases/22.04.5/release/ 