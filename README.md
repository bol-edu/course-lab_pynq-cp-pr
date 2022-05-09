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
To demonstrate the benefits of the composable overlay, we reference a composable video pipeline example from offical.
https://github.com/Xilinx/PYNQ_Composable_Pipeline

## Requirements of tutorial exercise
* A PYNQ-Z2 board with pynq 2.7up
* HDMI input signal of 1280x720
* HDMI displayer
* USB Webcam supports 1280x720

## Setup Juypter notebook examples of Composable Video Pipeline
Open a Jupyter Lab terminal

    $ root@pynq:/# cd /home/xilinx/
    $ root@pynq:/home/xilinx# git clone https://github.com/Xilinx/PYNQ_Composable_Pipeline
    $ root@pynq:/home/xilinx# python3 -m pip install PYNQ_Composable_Pipeline/ --no-build-isolation
    $ root@pynq:/home/xilinx# pynq-get-notebooks pynq_composable -p $PYNQ_JUPYTER_NOTEBOOKS

## Build Composable Video Pipeline sources on Vivado server

