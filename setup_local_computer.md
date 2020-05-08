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

# Setup Vitis on your own computer

To run (or build) these labs on your own computer, install Vitis. For non-commercial/academic use, Vitis licenses are free.

[Download Vitis 2019.2](https://www.xilinx.com/support/download/index.html/content/xilinx/en/downloadNav/vitis/2019-2.html) and install the tools.

[Download XRT and the U200 package](https://www.xilinx.com/products/boards-and-kits/alveo/u200.html#gettingStarted) for your computer, and install both packages.

### Setup the tools

Add the following to your environment setup.

```sh
source /opt/xilinx/xrt/setup.(c)sh
source $XILINX_VITIS/settings64.(c)sh
export PLATFORM_REPO_PATHS=$ALVEO_PLATFORM_INSTALLATION_DIRECTORY
```
