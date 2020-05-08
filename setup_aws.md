<table style="width:100%">
  <tr>
    <th width="100%" colspan=8><h2>XUP Vitis Labs (2019.2)</h2></th>
  </tr>
  <tr>
    <td align="center"><a href="setup_vitis.md">1. Setup Vitis</a></td>
    <td align="center"><a href="GUI_Flow_lab.md">2. Introduction to Vitis</a></td>
    <td align="center"><a href="Improving_Performance_lab.md">3. Improving Performance</a></td>
    <td align="center"><a href="Optimization_lab.md">4. Optimization</a></td>
    <td align="center"><a href="rtl_kernel_wizard_lab.md">5. RTL Kernel Wizard</a></td>
    <td align="center"><a href="debug_lab.md">6. Debugging</a></td>
    <td align="center"><a href="Vision_lab.md">7. Vision Application</a></td>
    <td align="center"><a href="PYNQ_lab.md">8. PYNQ Lab</a></td>
  </tr>
</table>

# Connecting to AWS

To get started with AWS, you will need an Amazon account. You will also need AWS credit to run the tutorial. If you are a professor or a student, you may be eligible to free credit by registering with [AWS educate](https://aws.amazon.com/education/awseducate/).

## Set up an AWS instance

Use [this guide](https://docs.aws.amazon.com/efs/latest/ug/gs-step-one-create-ec2-resources.html) to setup and AWS instance. Make sure to use the [FPGA Developer AMI version 1.8.1](https://aws.amazon.com/marketplace/pp/B06VVYBLZZ/ref=portal_asin_url) which includes Xilinx Vitis 2019.2 tools that this tutorial is based on.

### Login into the AWS and starting an F1 instance

1. Once you have an account, log in to the EC2 AWS Console:

    https://console.aws.amazon.com/ec2

    This should bring you to the EC2 dashboard (Elastic Compute).

    In the EC2 dashboard, select Launch Instance. From here you should be able to start your instance.

## Additional setup

You may want to do some additional setup to allow you to VNC to your instance. You can also follow the instructions in [Setup XUP AWS Workshop](setup_xup_aws_workshop.md) to connect to your instance.

### VNC server setup

When setting up an instance for the first time, you need to install vncserver software.

#### Install VNC server
In a terminal, execute the following commands

```sh
 sudo yum install -y tigervnc-server
 sudo yum groupinstall -y "Server with GUI"
```

When launching vncserver, you will be prompted to set up a password that you will need later.

### Start vncserver

Each time you start an instance, you will need to start vncserver

```sh
vncserver -geometry 1920x1080
```

  1. You can choose your preferred geometry (screensize)

  1. You should see a status message in the terminal once *vncserver* has started.

  1. Take note of the number after the “:”

  1. In this case, 1. This is the port the VNC viewer will connect to on the VNC server and needs to be specified as a two digit number below: 01.

  1. Connect to AWS instance from VNC viewer.

  1. From VNC viewer, specify the IP address of your AWS instance, followed by the VNC port number (as identified above), in this case :1

  1. When prompted, enter the VNC server password set up earlier.

  1. You should then be connected to the AWS instance.

### Clone AWS-FPGA repository

1. Open a terminal

1. Exectue the following to clone the *aws-fpga* repository and setup the Xilinx tools. `aws-fpga` includes the AWS F1 tools, HDK and documentation:

  ```sh
   cd ~
   git clone https://github.com/aws/aws-fpga
   cd ~/aws-fpga                                         
   source vitis_setup.sh
   source vitis_runtime_setup.sh
  ```

For more details see:

https://github.com/aws/aws-fpga/blob/master/Vitis/README.md
