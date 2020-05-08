<table style="width:100%">
  <tr>
    <th width="100%" colspan=8><h2>XUP Vitis Labs (2019.2)</h2></th>
  </tr>
  <tr>
    <td align="center">1. Setup Vitis</a></td>
    <td align="center"><a href="GUI_Flow_lab.md">2. Introduction to Vitis</a></td>
    <td align="center"><a href="Improving_Performance_lab.md">3. Improving Performance</a></td>
    <td align="center"><a href="Optimization_lab.md">4. Optimization</a></td>
    <td align="center"><a href="rtl_kernel_wizard_lab.md">5. RTL Kernel Wizard</a></td>
    <td align="center"><a href="debug_lab.md">6. Debugging</a></td>
    <td align="center"><a href="Vision_lab.md">7. Vision Application</a></td>
    <td align="center"><a href="PYNQ_lab.md">8. PYNQ Lab</a></td>
  </tr>
</table>

# Setup Vitis

There are two main parts to this tutorial - using the [Xilinx Vitis Unified Software Platform](https://www.xilinx.com/products/design-tools/vitis/vitis-platform.html) for building (compiling) designs and using and testing those designs in hardware.

You can run this tutorial in different ways.

* If you have an Alveo board, you can run all parts of the tutorial on a local machine.

* You can use the Vitis software in the cloud, with hardware in the cloud (AWS or Nimbix).
  * For running your design in AWS you will need to [create an AFI](Creating_AFI.md)

* You can use the Vitis software on a local machine for building designs, and only switch to the cloud to test in hardware, make sure you build for the correct shell.

This tutorial shows how to use Vitis with either AWS EC2 F1 or Alveo U200 (locally, or in the Nimbix cloud). Sources and precompiled solutions are provided for AWS EC2 F1 x2.large and Alveo U200. You may be able to use the Vitis tutorial instructions with other cloud providers, and other hardware.

Once you have decided how you want to run the tutorial, follow the appropriate instructions below.

## Local computer

To use your own computer, [install and set up Vitis and install the Alveo U200 packages](./setup_local_computer.md)

## Use Nimbix (Alveo)

The Xilinx Vitis tools and Alveo U200 hardware is available in the Nimbix cloud. Use the following instructions to [connect to a Nimbix Alveo instance](./setup_nimbix.md). A [free 100 hr Alveo trial](https://www.nimbix.net/alveo/) is currently available from Nimbix. This is the easiest way to work through this tutorial with Alveo U200 hardware. However, please note the [debug lab](debug_lab.md) is not currently supported on Nimbix as the Xilinx Virtual Cable is not available.

## AWS EC2 F1

An [FPGA Developer AMI](https://aws.amazon.com/marketplace/pp/B06VVYBLZZ) (Amazon Machine Image) is available with the Xilinx Vitis software preinstalled. This can be used to target AWS EC2 F1 hardware. An AMI is like a Virtual Machine image. You can use this AMI and the following instructions to [set up and connect to an AWS instance](./setup_aws.md)

You can also install [Vitis unified software platform](https://www.xilinx.com/support/download/index.html/content/xilinx/en/downloadNav/vitis.html) on your local machine, build design offline, and use AWS F1 hardware for testing. See the Amazon guide to use [AWS EC2 FPGA Development Kit](https://github.com/aws/aws-fpga) for details on setting up your machine.

## XUP AWS Tutorial

If you are attending a live instructor-led XUP AWS tutorial, preconfigured AWS F1 instances will be provided for you. Use the following instructions to [connect to your assigned AWS XUP tutorial instance](./setup_xup_aws_workshop.md)

# Getting started with the tutorials

Once you have setup your computer/cloud instance, you can *git clone* this repository to get started running the tutorial. The repository includes these instructions, and also a copy of source files, and solutions you will need for the tutorial.

The tutorial assumes you will clone this repository to your Linux home area. If you choose to clone it somewhere else, you will need to adjust the path where specified in the tutorial instructions.

```sh
 cd ~
 git clone https://github.com/xupgit/compute_acceleration
```

Proceed to the first lab [Introduction to Vitis](GUI_Flow_lab.md)
