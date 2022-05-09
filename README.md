# PYNQ Composable Pipeline & Partial Programming

## Outline of the lab lecture
* PYNQ
  1. PYNQ Introduction & Background
  2. PYNQ Overlays 
  3. PYNQ Libraries
  4. Overlay Design Methodology
* PYNQ Composable Overlays
  1. A Composable Video Pipeline
  2. Composable Overlay Methodology
  3. Default Paths
* Tutorial
  1. Composable Video Pipeline 

## A Composable Video Pipeline
To demonstrate the benefits of the composable overlay, we reference a composable video pipeline from offical.
https://github.com/Xilinx/PYNQ_Composable_Pipeline

## Setup Juypter notebook examples of Composable Video Pipeline
Requirements
* PYNQ-Z2 board with pynq 2.7up
* HDMI input signal of 720P
* HDMI displayer
* USB Webcam supports 720P

Open a Jupyter Lab terminal

    $ root@pynq:/# cd /home/xilinx/
    $ root@pynq:/home/xilinx# git clone https://github.com/Xilinx/PYNQ_Composable_Pipeline
    $ root@pynq:/home/xilinx# python3 -m pip install PYNQ_Composable_Pipeline/ --no-build-isolation
    $ root@pynq:/home/xilinx# pynq-get-notebooks pynq_composable -p $PYNQ_JUPYTER_NOTEBOOKS

## Build Composable Video Pipeline sources on Vivado server
Requirements
* Ubuntu 20.04 and Vivado 2020.2
* Install libc6-dev-i386 dependency package 
* Install PYNQ-Z2 board files

Make Composable Video Pipeline source

    $ git clone https://github.com/Xilinx/PYNQ_Composable_Pipeline --recursive
    $ cd PYNQ_Composable_Pipeline/boards/Pynq-Z2/
    $ make
