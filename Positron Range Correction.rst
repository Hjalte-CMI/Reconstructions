Positron Range Correction
==========================

Installation of NiftyPet
^^^^^^^^^^^^^^^^^^^^^^^^

NiftyPet install doc (Ubuntu)

1. Install cuda

Disable “secure boot” in bios, if it is enabled. Cannot install newest driver is it is for some reason.

Check for newest supported driver

.. code-block:: python

    $ apt search nvidia-driver

If newest for ex is 430:

.. code-block:: python

    $ sudo apt install nvidia-driver-430

Go to https://developer.nvidia.com/cuda-toolkit and follow instructions for installing the newest CUDA toolkit.
When installing the CUDA toolkit, do not install the graphics driver, but make sure that the driver downloaded previously is newer.

To set CUDA to path, type:

.. code-block:: python

    $ sudo touch /etc/profile.d/cuda.sh
    $ sudo gedit /etc/profile.d/cuda.sh

Now add in the following lines in the document that opened:
export PATH=$PATH:/usr/local/cuda/bin
export CUDADIR=/usr/local/cuda

To enable the path now, type:

.. code-block:: python

    $ source /etc/profile.d/cuda.sh

Check if CUDA is on path by:

.. code-block:: python

    $ nvcc --version


2. Other software
Ensure that CMAKE and git are installed, can be checked with:

.. code-block:: python

    $ CMAKE --version
    $ git --version

else install with:

.. code-block:: python

    $ sudo apt install cmake
    $ sudo apt install git

Make sure that the compiler is installed, to install type:

.. code-block:: python

    $ sudo apt-get install build-essential


Download and install anaconda navigator for python 2.


3. Install NiftyPet

Create a new enviorment for NiftyPet by:

.. code-block:: python

    $ conda create –name niftypet python=2.7


activate it by:

.. code-block:: python

    $ conda activate niftypet


Install the following packages:

.. code-block:: python

    conda install -c anaconda pycurl
    conda install -c anaconda matplotlib
    conda install -c anaconda ipython
    conda install -c conda-forge nibabel
    conda install -c conda-forge pydicom

Install jupyter:

.. code-block:: python

    $ conda install -c anaconda jupyter

Ongoing progress with integration of NiftyPET
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

+ 4/9-19
    + Can't run the tutorials test, https://niftypet.readthedocs.io/en/latest/tutorials/gpuaccess.html - problem might be GPU
+ 10/09-19
    + installation of new GPU (Quadro P2000)
+ 11/09-19
    + Successful run of the tutorial
    + NiftyPET is created to run data from a PET/MRI scanner - trying to convert to multiple use.
