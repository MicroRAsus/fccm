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

# Connecting to Nimbix

* Log in to Nimbix: https://platform.jarvice.com/

* Click Compute in the top left menu to select a compute instance

* Type Xilinx to filter the list of instances

![](./images/connecting_lab/nimbix/select_instance.png)

* Select the *Xilinx Vitis Unified Software Platform 2019.2* instance

* Click on Desktop mode with FPGA

![](./images/connecting_lab/nimbix/select_desktop_mode.png)

* Select the instance you prefer.

The smallest instance can be used for the labs. For the first part of the labs, you don't need to select an instance with Alveo hardware.

> Note that only  `/data/` folder is persistent storage, everything outside of this folder will be lost after powering-off the instance

![](./images/connecting_lab/nimbix/select_instance_config.png)

When the instance is ready, you will see the option to *Click here to connect*.

* Click on the desktop preview to connect.

![](./images/connecting_lab/nimbix/connect_to_instance.png)

A Linux desktop will open in a new tab in your browser.

![](./images/connecting_lab/nimbix/linux_desktop.png)

# Enroll to an Alveo trial

Nimbix provides up to 100 hours of free time on the Nimbix Cloud using Xilinx Tools and Accelerators.

* Request an [Alveo trial](https://www.nimbix.net/alveotrial)

* Fill in the form and make sure you select U200 Alveo board.

![](./images/connecting_lab/nimbix/alveo_trial.png)

* Shortly after you will get an email with a coupon number and instructions to continue the process.

* You will be asked to fill in billing information for non-alveo use.

* After that, you will get another email to complete the registration.

* Finally, you can log in https://platform.jarvice.com/
