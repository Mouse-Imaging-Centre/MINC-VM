# Builder of VirtualBox and VMWare VMs with minc-tools

This is a [packer](https://www.packer.io/) set of build scripts which takes
the Ubuntu ``mini.iso`` file, installs a minimal Lubuntu-core desktop, followed
by installing all of the MINC family of tools as well as R/RStudio for
statistical analysis.

## Download

You can find the VMs for download at:
<http://packages.bic.mni.mcgill.ca/virtual-machines/>

## Usage Instructions

The download file is an importable OVA VM, configured for
use with VirtualBox. Import into the virtual machine into VirtualBox. If you wish
to run analysis/processing on larger datasets, don't forget to assign more CPUs
and more memory to the virtual machine on import.

For help with importing VMs see:

<https://docs.oracle.com/cd/E26217_01/E26796/html/qs-import-vm.html>

**This VM is built against Virtualbox 6.0.12, if you have problems with Display/brain-view2, or rstudio,
you may need to upgrade your Virtualbox or disable 3D acceleration in your configuration.**

Getting files into and out of the VM is accomplished via the the shared folder
feature. Shared folders are automatically mounted inside ``/media/minc``

For help with shared folders in VirtualBox see <http://www.htpcbeginner.com/setup-virtualbox-shared-folders-linux-windows/>

All software is globally installed and available via the LXTerminal in
the Lubuntu menu.

To install additional software, the use the ``sudo apt`` tools, the user
password is ``minc``

**There is no need to install virutalbox guest additions, they are already installed in the VM**

## Tools included

-   [minc-toolkit-v1](https://github.com/BIC-MNI/minc-toolkit)
-   [minc-toolkit-v2](https://github.com/BIC-MNI/minc-toolkit-v2)
-   [pyminc](https://github.com/Mouse-Imaging-Centre/pyminc)
-   [minc-stuffs](https://github.com/Mouse-Imaging-Centre/minc-stuffs)
-   [R](https://www.r-project.org/)
-   [RStudio](https://www.rstudio.com)
-   [RMINC](https://github.com/Mouse-Imaging-Centre/RMINC)
-   [brain-view2](https://github.com/Mouse-Imaging-Centre/brain-view2)
-   [pyezminc](https://github.com/BIC-MNI/pyezminc)
-   [itksnap 3.4.0 with MINC support](https://github.com/vfonov/itksnap3) -- Currently broken
-   [mni.cortical.statistics](https://github.com/BIC-MNI/mni.cortical.statistics)
-   [generate_deformation_fields](https://github.com/Mouse-Imaging-Centre/generate_deformation_fields)
-   [mni-Display](https://github.com/BIC-MNI/Display)
-   [nipype with MINC support](http://nipy.org/nipype/)
-   [pydpiper](https://github.com/Mouse-Imaging-Centre/pydpiper)
-   [bpipe](http://bpipe.org)
