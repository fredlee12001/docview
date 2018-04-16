=============
DxHDCP readme
=============

.. contents:: Table of Contents
    :depth: 3

General
=======

- General explanation about ARM HDCP product can be found `here <https://www.arm.com/products/security-on-arm/trustzone-protected-hdcp>`__
- The product implements `HDCP 2.2 Interface Independent Adaptation (IIA) protocol stack <https://en.wikipedia.org/wiki/High-bandwidth_Digital_Content_Protection>`_.
- In order to reach high security, security sensitive logic is running inside HW assisted Trusted Execution Environment.
  More information is here: `\\\\eukfn-nas02.kfn.arm.com\\pj02462_ta\\lectures\\HWA\\HWA-Platforms Introductions by Dima.heb.avi`
- Specification, Errata and Compliance Test Specification (CTS) can be found in the `DCP site <http://digital-cp.com/hdcp-specifications/>`_
- This project depends on:

    - `TZInfra library <https://github.com/ARMmbed/ta-TZInfra>`_
    - `VOS library <https://github.com/ARMmbed/ta-Vos6>`_
    - `DxInfra library <https://github.com/ARMmbed/ta-Infra>`_

- TZInfra library introduction is `here <http://teamsites.arm.com/sites/IOTBU/Engineering/EngineeringGroupGrinbergDmitry/TZInfra/TZInfra%20Introduction.pptx>`__
- Recorded lectures related to the TZInfra library are saved under `\\\\eukfn-nas02.kfn.arm.com\\pj02462_ta\\lectures\\TZinfra`
- Recorded lectures related to the VOS library are saved under `\\\\eukfn-nas02.kfn.arm.com\\pj02462_ta\\lectures\\VOS`
- Recorded lectures related to the DxInfra library are saved under `\\\\eukfn-nas02.kfn.arm.com\\pj02462_ta\\lectures\\DXInfra`
- Recorded lectures related to the HDCP product are saved under `\\\\eukfn-nas02.kfn.arm.com\\pj02462_ta\\lectures\\HDCP`

    - Explanation of entire HDCP ecosystem can be found here: `\\\\eukfn-nas02.kfn.arm.com\\pj02462_ta\\lectures\\HDCP\\HDCP ecosystem overview by Dima.heb.avi`
    - Explanation of HDCP protocol can be found `here <http://teamsites.arm.com/sites/IOTBU/Engineering/EngineeringGroupGrinbergDmitry/HDCP/Internal/Introduction%20to%20the%20HDCP%20Protocol.pptx>`__,
      `here <http://teamsites.arm.com/sites/IOTBU/Engineering/EngineeringGroupGrinbergDmitry/HDCP/Internal/Introduction%20to%20the%20HDCP%20Protocol%20(version%202.2)%20-%20May%202016.pptx>`__ and
      here: `\\\\eukfn-nas02.kfn.arm.com\\pj02462_ta\\lectures\\HDCP\HDCP Spec Explanation by Gil.heb.avi`

- Recorded lectures for application engineers can be found here: `\\eukfn-nas02.kfn.arm.com\pj02462_ta\lectures\HDCP\2017-06_AE_Training`
- Development of the HDCP protocol stack can be done on Linux Ubuntu 14 PC or on Windows 8.1 with Visual Studio 2015 Update 3 (or later).
- Definition of Done for each project task is `here <http://teamsites.arm.com/sites/IOTBU/Engineering/EngineeringGroupGrinbergDmitry/HDCP/Internal/Standard%20DoD.pptx>`__
- Status of supported platforms, list of upcoming deliveries can be found `here <http://teamsites.arm.com/sites/IOTBU/Engineering/Shared%20Documents/Trustlets>`__
- Open source

    - Any open source code used by HDCP product for internal or external use (including HDCP tests) should be approved
      by legal.
    - List of open source code can be found `here <http://teamsites.arm.com/sites/IOTBU/Engineering/EngineeringGroupGrinbergDmitry/HDCP/open_source/>`__

- Project wiki page is `here <http://confluence.arm.com/display/taHDCP/>`__. For now it is empty.

Obtaining HDCP sources
======================

- HDCP sources are located into `GitHub private repository <https://github.com/ARMmbed/ta-DxHDCP>`_.
- Connect to `GitHub <https://github.com/>`_ with SSH key as described `here <https://help.github.com/articles/connecting-to-github-with-ssh/>`__.
- To get HDCP source code, clone HDCP repository to a local PC (permission is required):
   `git clone git@github.com:ARMmbed/ta-DxHDCP.git`

Documentation
=============

- Documentation is stored into `docs folder of the repo <docs>`_ or into `teamsites server <http://teamsites.arm.com/sites/IOTBU/Engineering/EngineeringGroupGrinbergDmitry/HDCP>`_
- Design documents can be found `here <http://teamsites.arm.com/sites/IOTBU/Engineering/EngineeringGroupGrinbergDmitry/HDCP/Internal/Design/>`__
- CTS specs can be found `here <http://teamsites.arm.com/sites/IOTBU/Engineering/EngineeringGroupGrinbergDmitry/HDCP/dcp/>`__
- An explanation by `DCP <http://www.digital-cp.com/>`_ of compatibility issues related to HDCP repeaters with zero device count is `here <http://teamsites.arm.com/sites/IOTBU/Engineering/EngineeringGroupGrinbergDmitry/HDCP/dcp/plugfest042005.pdf>`__
- DCP provisioning files format spec can be found here `here <http://teamsites.arm.com/sites/IOTBU/Engineering/EngineeringGroupGrinbergDmitry/HDCP/dcp/HDCP_Specification_2_Signing_Facility%2007122013.pdf>`__
- Readme file related to HDCP over Windows Phone platform is `here <docs/internal/HDCP_Qualcomm_Windows_Phone.md>`__
- Legacy HDCP documentation for customers can be found `here <http://teamsites.arm.com/sites/IOTBU/Engineering/EngineeringGroupGrinbergDmitry/HDCP/deliverables/>`__
- Release notes for external releases stored `here <https://armh.sharepoint.com/sites/Iot-customer-engineering-o365/Shared%20Documents/Release%20Notes/HDCP/>`__ 
  and `here <http://teamsites.arm.com/sites/IOTBU/Engineering/EngineeringGroupGrinbergDmitry/HDCP/releases/>`__
- Sprint Retrospective and Review can be found `here <https://confluence.arm.com/display/IoTBU/HDCP+Sprint+Retrospective+and+Review>`__

Git working procedure
=====================

- Git version control is used for HDCP project.
- Git working procedure is described `here <http://teamsites.arm.com/sites/IOTBU/Engineering/EngineeringGroupGrinbergDmitry/HDCP/Internal/Git%20working%20procedures%20for%20common%20use%20cases.docx>`__.
- After cloning project GIT repository, in order to setup-up git hooks - execute `install_git_hooks.py <install_git_hooks.py>`_ script from the root repository directory.

Code review
===========

- Code review is mandatory for each commit to the Main Development Branch (MDB), Long term branch or Release branch (see Git working procedure above).
- Code review should be done using: `review board server <http://ta-lab-master.kfn.arm.com:8000/>`_. For more information, see `review board wiki page <docs/internal/ReviewBoard.md>`_

Continuous Integration (CI)
===========================

- We use `Jenkins CI <http://ta-lab-master.kfn.arm.com:8080/job/HDCP/>`_ server for continuous integration
- Jenkins CI polling GIT repository periodically
- After each commit to MDB, compilation and tests execution of all major configuraitons
  (including SW and HW platforms) is started
- When compilaton and tests execution finish, a status email is sent to
  `Engineering-Group-Grinberg-Dmitry` group. 
- For different branches it is possible to configure different email notfication policies
- It is also possible to force Jenkins CI to build/run tests manually. Use
  `ta-DxHDCP-Manual <http://ta-lab-master.kfn.arm.com:8080/job/HDCP/job/ta-DxHDCP-Manual/>`_
  Jenkins job for this.
- Jenkins CI supports gathering of `code metrics <http://ta-lab-master.kfn.arm.com:8080/job/HDCP/job/ta-DxHDCP-Metrics/>`_
  (e.g. tests coverage report can be found into `Metrix <http://ta-lab-master.kfn.arm.com:8080/job/HDCP/job/ta-DxHDCP-Metrics/>`__ Jenkins job under `Coverage.SW_Linux_x32`).
- Jenkins CI configuraiton files are `here <Jenkinsfile>`__ and `here <Scripts/jenkins_core.groovy>`__

Copyright disclaimer
====================

All new files ("C" files, "H" files, scripts, etc...) should have copyright disclaimer on the beginning of each file
Copyright disclaimer should be: ::

   Copyright (C) 2017 ARM Ltd (or its subsidiaries).
   All Rights Reserved.

Copyright disclaimer should specify each year the code was changed in, for example if code was changed in 2016 and 2017
the copyright disclaimer should include year range: ::

   Copyright (C) 2016-2017 ARM Ltd (or its subsidiaries).
   All Rights Reserved.

It is not mandatory to change Discretix copyright disclaimer into existing files to new ARM copyright disclaimer

Syncronization between Linux and Windows PCs
============================================

- Normaly we use two PCs: Linux PC and Windows PC for development
- To syncronize source files on both PCs it is possible to use Unison File Synchronizer
- An explanaiton about Unison File Synchronizer setup and usage can be found `here <https://github.com/ARMmbed/ta-TZInfra/blob/master/devenv/unison_sync/README.md>`__
- To start syncronization process, execute `sync_start_unison.bat <sync_start_unison.bat>`_ script on Windows PC

Project tree structure
======================

+----------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------+
| Directory                                                                                          | Comment                                                                 |
+====================================================================================================+=========================================================================+
| `docs <docs>`_                                                                                     | Documentation                                                           |
+----------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------+
| `Externals <Externals>`_                                                                           | External projects (download from github during project build)           |
+----------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------+
| `HDCP/BaseLayer <HDCP/BaseLayer>`_                                                                 | HLOS code                                                               |
+----------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------+
| `HDCP/IFLayer <HDCP/IFLayer>`_                                                                     | HLOS external API layer                                                 |
+----------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------+
| `HDCP/TEE <HDCP/TEE>`_                                                                             | TEE code                                                                |
+----------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------+
| `HDCP/external/HDCP_API <HDCP/external/HDCP_API>`_                                                 | External API H files and configuration files                            |
+----------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------+
| `HDCP/external/PlatformUtils/Common/Drmversion <HDCP/external/PlatformUtils/Common/Drmversion>`_   | Product version definition and version handling code                    |
+----------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------+
| `HDCP/tools <HDCP/tools>`_                                                                         | Tools, Provisioning binary files, Provisioning PC tool                  |
+----------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------+
| `Testing/GTest <Testing/GTest>`_                                                                   | Google tests infrastructure                                             |
+----------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------+
| `Testing/Tests <Testing/Tests>`_                                                                   | Testing infrastructure and tests                                        |
+----------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------+
| `Testing/WorkSpace <Testing/WorkSpace>`_                                                           | Test workspace, provisioning and SRM data files and configuration files |
+----------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------+
| `Scripts <Scripts>`_                                                                               | Build and automation scripts                                            |
+----------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------+
| `licenses <licenses>`_                                                                             | Licenses and credits for 3rd party open source code                     |
+----------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------+


Software Installation and Configuration
=======================================

- Linux:

   - Make sure Python version 2.7.x is installed, if not, run `sudo apt-get install python`.
   - Install pip (Python package manager) by running `sudo apt-get install python-pip`. Note: by default pip is
     configured to manage packages for Python 3. To manage packages for Python 2.7 the flowing command should be used:
     `python2.7 -m pip install <SomePackage>`. For more info see `this link <https://docs.python.org/2/installing/>`__.
   - Docker should be installed and configured to use local docker registry server. Installation and configuration
     instructions can be found `here <https://github.com/ARMmbed/ta-TZInfra/blob/master/devenv/docker/README.rst>`__.
     To simplify Docker installation process, it is possible to run `this script <https://get.docker.com/>`__ to install
     Docker SW.
   - Android NDK 13B should be installed to `/opt/android-ndk-r13b/` directory.
   - ADB version 1.0.39 or later should be installed to `/opt/platform-tools/` directory. It is possible to copy ADB
     binaries from shared drive: `/projects/iot/pj02462_ta/hwa/Tools/google/adb_1.0.39` to the PC.
   - Python lxml package should be instaled: ::

      sudo apt-get install python-dev libxml2-dev libxslt1-dev zlib1g-dev
      sudo pip install lxml

   - GCC 6.2 should be installed: ::

      sudo add-apt-repository ppa:ubuntu-toolchain-r/test
      sudo apt-get update
      sudo apt-get install g++-6 c++-6
      sudo update-alternatives --install /usr/bin/gcc gcc /usr/bin/gcc-6 60 --slave /usr/bin/g++ g++ /usr/bin/g++-6
      sudo apt-get install gcc-6-multilib g++-6-multilib

   - Also include the following SW: ::

      sudo apt-get install openssh-client software-properties-common 
      sudo apt-get install libstdc++6 libc6-dev libc6-dbg:i386 libgcc-4.8-dev
      sudo apt-get install build-essential gcc-multilib g++-multilib lib32bz2-dev libc6-dev-i386
      sudo apt-get install lib32z1-dev texlive-full wget git unzip zip make nano gcovr tree mc toilet
      sudo apt-get install rsync valgrind vim python-sphinx graphviz gdb

   - The following lines should be added to the `~/.bashrc` file: ::

      # GIT prompt configuration
      unset GIT_PS1_SHOWDIRTYSTATE
      unset GIT_PS1_SHOWUNTRACKEDFILES
      # non-printable characters must be enclosed inside \[ and \]
      PS1='\[\033[0m\]'              # VT100 compat: reset all colors
      PS1="$PS1"'\[\033[32m\]'       # change color
      PS1="$PS1"'\u@\h '             # user@host<space>
      PS1="$PS1"'\[\033[33m\]'       # change color
      PS1="$PS1"'\w'                 # current working directory
      PS1="$PS1"'$(__git_ps1)'       # bash function
      PS1="$PS1"'\[\033[0m\]'        # change color
      PS1="$PS1"'\n'                 # new line
      PS1="$PS1"'$ '                 # prompt: always $
      
      export PATH=/opt/android-ndk-r13b:/opt/platform-tools:$PATH
      export TZ_PLATFORMS_ROOT=/projects/iot/pj02462_ta/tzplatforms
      
      # This function is usable to access group shared folder (auto-mount of this folder should be done by IT)
      function mmm
      {
         cd /projects/iot/pj02462_ta
      }
 
   - Make sure that all the SW components and tools required for TZInfra library compilation are installed. List of
     these requirements can be found into readme files inside `TZInfra repository <https://github.com/ARMmbed/ta-TZInfra>`_

   - Network configuration tweaks:
        
      - Add the following lines to the `/etc/sysctl.conf` file (with sudo) ::

           net.ipv4.tcp_tw_reuse = 1
           net.ipv4.tcp_slow_start_after_idle = 0

      - Execute command: `sudo sysctl -p` to apply changes without reboot. For more information see `Sysctl tweaks <https://wiki.mikejung.biz/Sysctl_tweaks>`_ article
 
   - Copy file `99-android.rules <https://github.com/ARMmbed/ta-TZInfra/blob/master/tools/99-android.rules>`_ to
     `/etc/udev/rules.d/` folder. It will allow ADB to access Android devices using USB connection without root permission.
   - Edit `/etc/security/limits.conf` file with sudo - add the following line to this file: `*      -       rtprio  -1`.
     This will allow any user to run realtime priority processes without root privileges. HDCP tests should run as a
     real-time priority process.
   - It is recommended to run tests from ramdisk. It may prevent faulure due to slow I/O operation. (We saw situation when open() API call takes ~2 seconds).
     To do that, do the following steps:

      - Create /mnt/ramdisk direcory using `mkdir /mnt/ramdisk` command with sudo
      - Edit /etc/fstab file with sudo and add the following line: `tmpfs       /mnt/ramdisk tmpfs   nodev,nosuid,noatime,nodiratime,size=10G   0 0`

- Windows: 

   - Visual Studio 2015 with SP3 or later should be installed.
   - It is recommended to install `Git Extensions <https://gitextensions.github.io/>`_
   - It is recommended to install `Beyond Compare Pro <https://www.scootersoftware.com/>`_. Git Extensions should be
     configured to use Beyond Compare Pro as both: merge tool and diff tool.
   - It is recommended to install `BareTailPro <https://baremetalsoft.com/baretailpro/>`_ SW to analyze HDCP logs.
     Recommended BareTailPro configuration stored into `this <BareTailPro.udm>`__ file.
   - Install the latest version of `Python(x,y) <https://python-xy.github.io/downloads.html>`_.
   - Install pip (Python package manager):

      - Download `get-pip.py <https://bootstrap.pypa.io/get-pip.py>`_.
      - Run `python get-pip.py`.

   - Make sure that all the SW components and tools required for TZInfra library compilation are installed. List of
     these requirements can be found into readme files inside `TZInfra repository <https://github.com/ARMmbed/ta-TZInfra>`_.
   - Network protocol analyzer

      `Wireshark network protocol analyzer <https://www.wireshark.org/>`_ should be installed to analyze HDCP
      communication when running end-to-end tests against 3rd party HDCP devices. After Wireshark installation,
      `HDCP2 trafic analysis <https://wiki.wireshark.org/HDCP2>`_ should be enabled by entering:
      `Analyze->Enabled Protocols...` menu and checking options `HDCP2` and `hdcp2_tcp` as showed below:

      .. figure:: docs/images/WireSharkCfg1.jpg

   - Antivirus should be configured to exclude project root directory

HDCP and tests compilation
==========================

- General

   - Build script will automatically download dependent libraries from GIT repo and compile the project
   - List of dependent libraries can be found `here <Externals/externals.json>`__
   - Before travel, it is possible to download all dependent libraries to local PC using `this <Externals/get_external_projects.py>`__ script

- Windows

   - From the root directory of the HDCP repository - execute: `python project_builder.py` command to generate 
     Visual Studio 2015 solution (`DxHDCP_vs2015.sln.lnk` file will be created on the root directory)
   - Click on `DxHDCP_vs2015.sln.lnk` file into root project directly to open Visual Studio 2015 solution
   - Change `Solution Platforms` to `SW_Win32`
   - Into solution explorer - set `Tests` as a startup project
   - Build/rebuild the solution
   - It is OK to build and run both: `Debug_dynamic` and `Release_dynamic` configurations.

- Linux

   - From the root directory of the HDCP repository - execute: `Scripts/build_hdcp_and_tests.py sw_linux` command to
     generate make files and compile HDCP and tests
   - On successful compilation HDCP and tests binaries (both: 32-bit and 64-bit) will be created and copied to the
     `Artifacts` directory

- HW devices (Qualcomm, Mediatek, etc.)

   - In order to determine which platforms are currently supported execute `Scripts/build_hdcp_and_tests.py -h` command.
     Help menu will be displayed on the console.
   - In order to determine which build parameters are required for specific platform - execute
     `Scripts/build_hdcp_and_tests.py <platform> -h` command. For example: `Scripts/build_hdcp_and_tests.py qualcomm -h`
     command will show which build parameters are required for HDCP over Qualcomm platform compilation.
     For example, in order to build HDCP and tests for Qualcomm platform with default build parameters, execute command:
     `Scripts/build_hdcp_and_tests.py qualcomm`

HDCP and tests installation and running tests
=============================================

- Linux

     HDCP and tests executables should be installed before run. Use the following command to install it: ::

        python Scripts/install_hdcp_and_tests.py <bin_path>

     <bin_path> is a location of the build artifacts created by build_hdcp_and_tests.py script.

     The following command will install Linux 32-bit variant: ::

        Scripts/install_hdcp_and_tests.py Artifacts/Build_Artifacts_sw_linux32_release

     To run tests, execute the following command: ::

        python Scripts/run_gtests.py [-f=<tests filter>] <bin_path>

     - `<bin_path>` should point to the same directory that was used for `Scripts/install_hdcp_and_tests.py` 
       script. Logs will be collected to: `<bin_path>/logs/` directory (e.g. `Artifacts/Build_Artifacts_sw_linux32_release/logs/`)
     - `<tests filter>` is an optional parameter. In order to run only basic sanity tests, it is possible to use:
       `-f=*BB3*` filter. Example: ::

           Scripts/run_gtests.py -f=*BB3* Artifacts/Build_Artifacts_sw_linux32_release

     - For each running test, an explanation of test purpose and steps will be printed to the console.
     - If no tests filter is set or tests filter is set to `*` - all tests will run.
     - it is possible to concatenate more than one filter expressions using column separator. For example: filter
       `-f=*BB3*:-f=*BB2*` will run both: BB2 and BB3 tests.
     - More information about tests filter can be found `here <https://github.com/google/googletest/blob/master/googletest/docs/AdvancedGuide.md#running-a-subset-of-the-tests>`__
     - It is also possible to run tests executable without using install/run scripts. In order to do that, execute the following commands: ::

        cd Artifacts/Build_Artifacts_sw_linux32_release/bin/
        ./HdcpGTests32 -h   # show help menu
        ./HdcpGTests32 -l   # show list of all available tests

- Windows

   - It is possible to run HDCP tests from Visual Studio by pressing `F5` key.
   - It is also possible to set tests filter. An explanation about tests filter is same as for Linux (see above).
   - See example how to set `-f=*BB3*` filter on Windows:

     .. figure:: docs/images/VisualStudioConfigTestFilter.jpg

   - By default, tests logs will be saved under `Testing/WorkSpace/data/Gtest_Log` and `Testing/WorkSpace/data/xml_reports`.
     It is possible to override defaults by editing `Testing/WorkSpace/config/Windows/HdcpGTests.cfg` file.
   - By default, HDCP logs will be saved under `__build_vs2015/<configuration>/HdcpLogs/` 
     (`<configuration>` can be: `SW_Win32-140-Debug_dynamic` or `SW_Win32-140-Release_dynamic`).
     It is possible to override defaults by editing `Testing/WorkSpace/config/Windows/DxHDCP.cfg` file.

- Qualcomm Android MSM8996 (based on TZ 4.x)

   - In order to push files to device (using `ADB <https://developer.android.com/studio/command-line/adb.html>`_),
     USB configuration should be set to MTP. In the original Qualcomm MSM8996 image, 
     when the device reboot, the USB configuration goes back to `charging` even 
     if you set it to MTP before the reboot. To fix this do the following steps:

     - Connect device to the PC using USB cable and execute the following commands in the terminal: ::

        adb root
        adb shell setprop persist.sys.usb.config mtp,adb
        adb reboot

     - When device starts, on the Android UI go to `Settings` -> `Developer Options` -> `Select USB Configuration` menu
       and make sure that `Select USB Configuration` option is set to `MTP (Media Transfer Protocol)`.

   - Scripts `Scripts/install_hdcp_and_tests.py` and `Scripts/run_gtests.py` works for all Android devices. See
     explanaiton above how to use these scripts.

   - Normally working with Qualcomm devices is done on Linux PC, but it is also possible to work with Qualcomm device from Windows PC.
     In this case, Android SDK Platform Tools should be installed on Windows. If Qualcomm device is connected to Windows PC
     but not recognized, install `this <http://adbdriver.com/downloads/>`__ driver.

- Mediatek GP Android (mt6797 - yellow device)

   - An explanation about Mediatek platform can be found here: `\\\\eukfn-nas02.kfn.arm.com\\pj02462_ta\\hwa\\Mediatek\\readme.txt`
   - Scripts `Scripts/install_hdcp_and_tests.py` and `Scripts/run_gtests.py` works for all Android devices. See
     explanaiton above how to use these scripts.

Network configuration and HDCP traffic analysis
===============================================

In order to debug HDCP stack with HDCP tests or end-to-end tests against 3rd party equipment, it is possible to record
HDCP traffic using `tcpdump` command line utility and analyze recorded traffic using Wireshark Network protocol analyzer (see above).
`tcpdump` utility can be used on HDCP Sink device, HDCP Source device or on both devices.

   - Currently both HDCP Sink and HDCP Source tests are running on the 
     same device - in this case network traffic should be captured on a 
     loopback interface. Later, we plan do delvelop tests that will run 
     across network.

   - Stable bi-directional ping of at most 4 millisecond is required for HDCP 
     tests between two HDCP devices or for end-to-end HDCP tests. To achieve 
     this, the one of the following steps should be done:

     - Connect device to PC using USB tethering. In this case it is possible to 
       run HDCP tests on PC against device.
     - Connect two devices using Wi-Fi direct.
     - Connect two devices using Wi-Fi - one device can be a Wi-Fi hotspot and 
       another device can connect to it.

   - On Qualcomm device, the following steps are required:

     - Wi-Fi power saving mode should be turned off. To do this use 
       `QC_post_burn_script.py <Scripts/QC_post_burn_script.py>`_ script (use
       `Changing network configuration` option from the interactive menu)
     - Run `android_keep_devices_busy.sh <Scripts/android_keep_devices_busy.sh>`_ 
       script in background to prevent device entering power down mode
     - All network configuration dialogs should be closed (if not, Android OS 
       will poll Wi-Fi HW status and it causes network delays)

   - Root permissions is required to use `tcpdump` utility
   - For Linux Ubuntu PCs, `tcpdump` utility should be installed by `apt-get install tcpdump` command
   - For Android devices, `tcpdump` for Android should be installed to the device:

     - It can be downloaded from `here <http://www.androidtcpdump.com/android-tcpdump/downloads/>`__ and pushed to the device
     - On Qualcomm devices, `tcpdump` utility is part of factory image, installation of it is not required
     - On Mediatek decives, `MTKLogger` utility should be used for traffic analysis (see below)

   - In order to capture HDCP traffic on Android device, the following steps should be done:

     - Connect device to the PC using USB cable
     - Enter ADB shell (using `adb -s <device id> shell` command)
     - Execute the following command: `tcpdump -i any -s 0 -w <file name.pcap>`. `<file name.pcap>` parameter should be replaced by actual file name where all captured traffic will be saved (e.g. `/data/tmp/capture.pcap`)
     - In order to capture HDCP traffic on Linux Ubuntu PC, the following command should be used: `sudo tcpdump -s 0  -i <interface> -w <file name.pcap>`.

       - `<file name.pcap>` parameter should be replaced by actual file name where all captured traffic will be saved (e.g. `${HOME}/capture.pcap`)
       - `<interface>` parameter should be replaced by network interface name through which the HDCP traffic passes:

         1. `usb0` if USB tethering is used
         2. `wlan0` if Wi-Fi connection is used
         3. `eth0` if Ethernet connection is used
         4. For full list of available network interfaces, use `/sbin/ifconfig` command

   - In order to capture HDCP traffic on Mediatek device, the following steps should be done:

     - Dial `*#*#3646633#*#*` and MTK EngineerMode will pop up
     - Select `Log and debugging`
     - Select `MTKLogger`
     - Click the `Settings` button in the right-top corner on the screen switches UI will pop up
     - Check is the `NetoworkLog` is switched on and press "back"
     - Click the `Start logging` button in the center-bottom on the screen
     - Start your testing and get into the `MTKLogger` UI and click the `Stop logging` button in the center bottom on the screen
     - The netdump file will be in `/mnt/sdcard/mtklog/netlog`
     - It is possible to pull the entire log files using `adb pull /mnt/sdcard/mtklog mtklog`

Tests coverage analysis
=======================

It is possible to check tests coverage on Linux machine using `Scripts/run_coverage.py` script.
Execute this script with `-h` argument to see help menu.
`lcov <http://ltp.sourceforge.net/coverage/lcov.php>`_ SW version 1.13 or later should be 
installed to use this script.

Enabling WFD working with HDCP on Qualcomm Devices
==================================================

Before executing end-to-end HDCP tests on Qualcomm devices against 3rd party devices, HDCP should be in Wi-Fi Display (WFD)
configuration. For more information follow `this <docs/internal/Enabling_WFD_working_with_HDCP_on_Qualcomm_Devices.md>`__ link.

HDCP Dongles
============

- A dongle is a small piece of hardware that connects to another device to provide additional functionality.
- The term `dongle <https://en.wikipedia.org/wiki/Dongle>`_ associated with devices providing additional forms of wireless connectivity to devices (such as Wi-Fi or Bluetooth support).
- Also it's small digital media players, meant to plug directly into an HDMI input on a TV.
- Dongles are 3rd party devices, that supports the HDCP protocol and used as a Sink side for `end-to-end tests <docs/internal/HDCP%20End%20to%20End%20testing%20guide.docx>`_.
- Purposes of end-to-end tests against dongles:
  - To check interoperability of our HDCP product against 3rd party devices that supporting HDCP protocol.
  - To check integration of WFD applications with our HDCP binaries.
- More information about setup dongles can found `here <docs/internal/HDCP_Dongles.rst>`__.

Platform Resources
==================

- HDCP TrustZone application require:
  - Stack size: 65536 bytes
  - Heap size:

    - Service TZ session (service device) requires 25600 bytes of heap are required.
    - For each additional HDCP device (Sink or Source), an additional 25600 bytes of heap are required.
    - Context global requires addtional ~5K from the heap.
    - Total: 4 devices + 1 service device + context global gives approximately 160000 bytes
      of heap when creating 4 HDCP devices (1-Source and 3-Sink devices are normally created 
      by HDCP Google tests).

miscellaneous
=============

- General porsuse netwotk storage: `\\\\eukfn-nas01.kfn.arm.com`
