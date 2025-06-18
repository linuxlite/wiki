---
title: Hardware
description: 
published: true
date: 2025-06-18T04:58:25.943Z
tags: 
editor: markdown
dateCreated: 2025-06-18T03:57:18.277Z
---

## Hardware Database

Wondering if your laptop or desktop will work on Linux Lite?  
Check out our Hardware Database [here](https://www.linuxliteos.com/hardware.php) to see if your model is already listed. Don't forget you can also run Linux Lite live before you install it to see if your hardware is supported. This database feature is new so the list of computers at the moment is limited. If you already have Linux Lite installed, please consider adding your hardware to the [Linux Lite Hardware Database](https://www.linuxliteos.com/hardware.php) to help others.

## Graphics Drivers and Setup

**Legacy Binary Drivers and Proprietary Binary Drivers**

**Legacy binary driver** - a driver for older video cards no longer supported by the current driver.  
**Proprietary binary driver** - a driver for newer video cards.

If you're not sure whether your video chipset/card needs a legacy binary driver or a proprietary binary driver, please select from the following links for **nVidia** and **AMD**:

[nVidia Legacy information](http://www.nvidia.com/object/IO_32667.html) - If your card is listed here, you can either use the pre-installed video driver for Linux Lite or you can try the legacy driver. Linux Lite recommends you stick with the pre-installed video driver as it is the most reliable, and the safest choice.

[AMD Legacy information](https://help.ubuntu.com/community/BinaryDriverHowto/AMD) - Linux Lite recommends you stick with the pre-installed video driver as it is the most reliable, and the safest choice.

## Graphics - AMD Radeon

![](images/hardware/radeon/radeon-logo.png)

**NOTE: The newest Linux Lite is based on Ubuntu 22.04 'Jammy' and therefore cannot provide the AMDGPU proprietary drivers. This is something that is out of our control. If you want to use the AMDGPU proprietary drivers, there are advanced tutorials available online. Please note that we cannot provide support for the AMDGPU proprietary drivers.**

**

If you have an AMD graphics card, there is no need to install any graphics drivers in the Linux Lite Series, 5x, 6x. The open source drivers are already pre-installed. The following AMDGPU products are supported via a collection of pre-installed open source drivers in Linux Lite:

**

**R100, RV100, RS100, RV200, RS200, RS250, R200, RV250, RV280, RS300, RS350, RS400/RS480, R300, R350, R360, RV350, RV360, RV370, RV380, RV410, R420, R423/R430, R480/R481, RV505/RV515/RV516/RV550, R520, RV530/RV560, RV570/R580, RS600/RS690/RS740, R600, RV610/RV630, RV620/RV635, RV670, RS780/RS880, RV710/RV730, RV740/RV770/RV790, CEDAR, REDWOOD, JUNIPER, CYPRESS, HEMLOCK, PALM, SUMO/SUMO2, BARTS, TURKS, CAICOS, CAYMAN, ARUBA, TAHITI, PITCAIRN, VERDE, OLAND, HAINAN, BONAIRE, KABINI, MULLINS, KAVERI, HAWAII.**

As well as many legacy (older) ATI/AMD video cards including, but not limited to:

**ATI Rage 'r128' series, ATI Mach64 series and legacy AMD/ATI Mach64, Rage128, Radeon, FireGL, FireMV, FirePro, FireStream video cards**.



## Graphics - NVIDIA

If you're not sure if your graphics card is nVidia or not, open up a terminal and run this command:

Terminal Command:

						sudo lshw -C display

  

![](images/hardware/nvidia/nvidia1.png)

You see under **product:** **nVidia** or **GeForce** (and similar naming schemes for nVidia cards) depending on your card. The **vendor:** line may also show you the Product or Company name.

**NOTE: You must be connected to the internet before you start the driver install.**

The next step is to go to **Menu, Settings, Install Drivers**.

![](images/hardware/install_drivers.png)

The program will then scan your computer for any drivers that you may need, this may take some time.

![](images/hardware/nvidia/nvidia2.png)

When it has finished scanning, you will see a dialogue box similar to the one below.

![](images/hardware/nvidia/nvidia3.png)

Generally you will want to select the current version, the tested driver. In the above example we selected the **Using NVIDIA binary driver (proprietary, tested).**

**NOTE:** If you plan to play graphic intensive games or you have a lot of Steam games, you need to select the **proprietary, tested** driver.

Now click on **Apply Changes**. You will be prompted for your password:

![](images/hardware/driverpassword.png)

You will see the following dialog as it downloads and installs:

![](images/hardware/nvidia/nvidia4.png)

When the driver has finished, restart your computer.

Now head over to **Menu, System, NVIDIA X Server Settings**.

![](images/hardware/nvidia/nvidia5.png)

Once you open **NVIDIA X Server Settings,** you will have a number of options to select as well as some technical data to look over.

![](images/hardware/nvidia/nvidia6.png)



## Graphics - NVIDIA Prime

This method should ONLY be used if the above nVidia install method does not give you Prime options in the Nvidia Settings Manager. From a fresh install of Linux Lite, open up a terminal and type:

Terminal Command:

						sudo apt-get update

  

To install the recommended driver, run the following command:

Terminal Command:

						sudo ubuntu-drivers autoinstall

  

Now restart your computer.



## Dual Monitor Setup Instructions

If you have two monitors, they will start out 'mirroring' the same displayed output.

![](images/hardware/dualmonitors/dual-monitors1.png)

To get the monitors to act as one large area allowing you to spread your work out separately on each, you can now do that easily through the GUI **Settings Manager** instead of through terminal commands and manually editing configuration files.

Go to **Menu, Settings, Settings Manager**.

![](images/hardware/dualmonitors/dual-monitors2.png)

Click on **Display** under the **Hardware** category.

![](images/hardware/dualmonitors/dual-monitors3.png)

Initially, both monitors will have the **Mirror displays** box checked.

![](images/hardware/dualmonitors/dual-monitors4.png)

Click on the first monitor listed on the left and un-check **Mirror displays** on the right. Repeat the procedure for the second monitor.

Drag and drop each screen to where you want them to be arranged. Click **Apply** when you are finished.

![](images/hardware/dualmonitors/dual-monitors5.png)

Once they are no longer mirrored, you may see that one of them is missing the desktop wallpaper and the lower panel only spans one of them.

![](images/hardware/dualmonitors/dual-monitors6.png)

Click **All Settings** to go back to the main **Settings Manager** window and choose **Desktop** under the **Personal** category.

![](images/hardware/dualmonitors/dual-monitors7.png)

Whichever monitor the **Desktop** settings window is on, that is the one it will apply to. Drag it over to the monitor that is blank and notice how the monitor description changes according to which one it is on.

![](images/hardware/dualmonitors/dual-monitors8.png)

![](images/hardware/dualmonitors/dual-monitors9.png)

When you drag the Display settings window over to another monitor, the wallpaper that was highlighted on the one you dragged from stays highlighted, but no change will take effect on the second monitor until you actually click on one of the wallpapers. You may set a different wallpaper for each monitor.

![](images/hardware/dualmonitors/dual-monitors10.png)

If you want one picture to span across both screens, set the second screen to **None** in the **Style** drop down box. (Remember - you need to have the Desktop settings window positioned on the second monitor to do this.)

![](images/hardware/dualmonitors/dual-monitors11.png)

Then move the Desktop settings window back to the monitor with the wallpaper displayed and select **Spanning screens** from the **Style** drop down box.

![](images/hardware/dualmonitors/dual-monitors12.png)

Now, you will have wallpaper spanning across both screens; but you still have the panel stuck on only one of them.

![](images/hardware/dualmonitors/dual-monitors13.png)

To get your panel to also span both monitors, go back to the main Settings Manager window and choose **Panel** under the **Personal** category.

![](images/hardware/dualmonitors/dual-monitors14.png)

In the Panel settings window, click on the box next to **Span Monitors**.

![](images/hardware/dualmonitors/dual-monitors15.png)

Congratulations, you have successfully set up and configured dual monitors.

![](images/hardware/dualmonitors/dual-monitors16.png)



## Sound Configuration

The audio icon can be found in the lower right hand corner, commonly referred to as the system tray.

![](images/hardware/sound/sound_config1.png)

Left click on the speaker icon. You can drag the main slider to the left or right to control main volume. Now click on **Audio Mixer**.

![](images/hardware/sound/sound_config2.png)

You will be brought to a window similar to this one.

![](images/hardware/sound/sound_config3.png)

In the window above you can adjust volume settings for output. Using the sliding bars. You can toggle mute with the speaker icon: ![](images/hardware/sound/sound_config4.png)It will change it's background color when active: ![](images/hardware/sound/sound_config5.png) You can lock channels using: ![](images/hardware/sound/sound_config6.png) so that when volume is raised or lowered it is done equally. Or you can toggle and set the volume to be louder on one side. This icon: ![](images/hardware/sound/sound_config7.png)is used to specify the default device used by PulseAudio.

**Playback** \- will list programs currently producing audio, or able to. You can toggle access per program and or adjust volume per program here. The method used is the same as mentioned above.

![](images/hardware/sound/sound_config8.png)

**Recording** \- will list programs currently using an input method, be it line-in or a microphone. You can toggle access per program and or adjust volume per program here. The method used is the same as mentioned above.

![](images/hardware/sound/sound_config9.png)

**Output Devices** \- is for main configuration of sound levels across your system.

![](images/hardware/sound/sound_config3.png)

**Input Devices** \- this includes microphones and other line-in devices, such as TV tuner cards with line in. Adjusting the levels and settings are the same method as described above.

![](images/hardware/sound/sound_config10.png)

**Configuration** \- this lists known profiles for your sound card. In most cases there is no need to select anything here unless you intend to disable your sound completely, or have a unique profile setting, such as surround sound, mono, or stereo out.

![](images/hardware/sound/sound_config11.png)

**Notes**: Being able to toggle on mute and unmute on multiple things can cause issues. And at times the device may be muted upon install. Show caution here as you may mute a certain program and forget about it entirely. If unmuting and adjusting settings for your sound card and related programs do not work at all, there may be a driver issue. Refer below for resources on how to remedy this. You can find help by using the [Lite System Report tool](#sysreport) and using the directions to upload the generated report to the Forums.

## Volume Toggles

Here, we will show you how to set keyboard shortcuts for **Volume + Volume - and Mute Volume**.

Providing you are not already using the hot keys on a supported multimedia keyboard, the following is an excellent replacement.

First step is to right click on the **Volume** icon in the tray, select **Properties** and ensure **Enable keyboard shortcuts for volume control** is ticked.

![](images/hardware/sound/volumetoggle/volumetog1.png)

1\. Next click on **Menu, Settings, Keyboard** and click on the **Applications Shortcuts** tab.

![](images/hardware/sound/volumetoggle/volumetog2.png)

2\. Next click on the **Add** button and paste in the following:

**pactl -- set-sink-volume 0 +10%**

3\. Click Ok and then hold down the **Right Alt** key and the **\=/+** near the top of your keyboard.

![](images/hardware/sound/volumetoggle/volumetog3.png)

Now **Right Alt plus =/+** is set to raise the main volume.

![](images/hardware/sound/volumetoggle/volumetog4.png)

4\. To set a toggle to lower the volume by 10% each time, repeat steps 1 -3 above but this time to lower the volume, enter this command:

**pactl -- set-sink-volume 0 -10%**

5\. This time hold down the **Right Alt** key and the **\-/\_** near the top of your keyboard (next to the =/+ button).

Now **Right Alt plus -/\_** is set to lower the main volume.

![](images/hardware/sound/volumetoggle/volumetog5.png)

6\. To set a toggle to mute the volume repeat steps 1 -3 above but this time to mute the volume, enter this command:

**pactl -- set-sink-mute 0 toggle**

7\. This time hold down the **Right Alt** key and the **M** on your keyboard.

Now **Right Alt plus M** is set to mute the main volume.

![](images/hardware/sound/volumetoggle/volumetog6.png)

Now all 3 volume toggles have been set, try them out.

![](images/hardware/sound/volumetoggle/volumetog7.png)

## Resources for Audio Drivers

[Ubuntu Wiki - Sound](https://help.ubuntu.com/community/Sound) Contains a list of guides for configuring specific drivers for older and odd sets of sound cards.

[Ubuntu Wiki - Troubleshooting](https://help.ubuntu.com/community/SoundTroubleshooting) Contains steps to help trouble shoot and configure sound cards.

[Halfgaar](http://www.halfgaar.net/surround-sound-in-linux) Has a great guide to setting up surround sound under linux.

[More surround sound help from here](http://alexsleat.co.uk/2011/12/03/setting-up-surround-sound-in-linux/).



## Printer Setup

**1.** Plugging in a printer will prompt a dialog if detected and attempt to find a matching driver. (If your driver was plugged in during your initial install you may not see a prompt, you may refer to step 3 below.)

![](images/hardware/printing/printer1.png)

**2.** If a printer and driver has been detected you will see this dialog. (Note, the dialog should appear in upper right of your screen)

![](images/hardware/printing/printer2.png)

**3.** You can further configure or manage printing jobs or printers by going to printing located in **Menu, System, Printers**.

![](images/hardware/printing/printer3.png)

**4.** Once you open the **Printing** menu it will bring you to a simple dialog to select, view and manage options related to your printer.

![](images/hardware/printing/printer4.png)

**5.** You can find options for your printer by highlighting (left clicking) on your printer, then click on **Printer, Properties**.

![](images/hardware/printing/printer5.png)

**6.** If a printer if not listed in the window after opening it, you will need to plug in the device and click on the **+** sign located below the menu.

![](images/hardware/printing/printer6.png)

**7.** Once you click on the **+** sign above, you will see this window if the printer was detected properly. You can then select the method of connect and printer on the pane near the bottom of the window. (You may see more than one option if your device is an all in one device, so select from the left pane carefully.) From here you can also select a **Network Printer** if you are connected to a home network and a printer is available.

**7.1** If for some reason you are unable to see a network printer on a machine using Windows you may need to configure samba (a sharing and networking tool for Linux > Windows) You can find help doing this [here](https://help.ubuntu.com/community/NetworkPrintingWithUbuntu).

![](images/hardware/printing/printer7.png)

**8.** Clicking Forward on the above window will bring you to this window where you can set the **Printer Name, Description** and **Location** for the printer. However **Description** and **Location** are not required, unless you share a printer or use one over a network.

![](images/hardware/printing/printer8.png)

**9.** Cups is a web interface for managing your printer. Once installed, click [here](http://localhost:631) to manage your printer.



## Share your Printer from Linux Lite

The following tutorial gives an example of how to set up a shared printer connected to Linux Lite.

Make sure the printer connected to Linux Lite and is fully operational, drivers installed and set up.

Temporarily disable the Linux Lite Firewall, see [here](tutorials.html#firewall). After you are able to print from Windows to a Linux Lite shared printer, we will enable it again and create the correct rule for it. Firewall blocking services is usually overlooked.

Click on **Menu, System, Printers**.

Select (highlight) your Printer and select from the menu **Printer, Shared**.

![](images/hardware/printing/shared_printer1.png)

Then, considering this is a home network and that you want to make your life as easy as possible, let's allow quite a few options in **Server Settings**. Open **Server, Settings** and configure as shown below:

![](images/hardware/printing/shared_printer2.png)

That's all there is on your Linux Lite side. Now let's go to your Windows 10 machine to connect to the shared printer.

Before going into Windows, make sure you know the correct name of your printer. For example, my printer name is **Samsung-ML-2550** (case sensitive). This is the name you define when adding the printer to Linux Lite. You do not want to have spaces in the name and also understand that lower case and UPPER case do make a difference in Linux. So, with that said, in Windows 10:

**Devices and Printers -> Add a printer - The printer that I want isn't listed**.

![](images/hardware/printing/shared_printer3.png)

**Select a shared printer by name**.

The printer can the be added using the hostname or the IP address of your Linux Lite PC on port 631. To keep it simple, in case you do not have DNS resolution in your local network, you will use the IP address of your Linux Lite PC, as shown below:

_http://\[LINUX LITE PC IP\]:631/printers/\[YOUR PRINTER'S CASE SENSITIVE NAME\]_

![](images/hardware/printing/shared_printer4.png)

From there, just select the brand and model for your printer as you usually do in Windows... and you should be able to print thereafter.

![](images/hardware/printing/shared_printer5.png)

![](images/hardware/printing/shared_printer6.png)

![](images/hardware/printing/shared_printer7.png)

Once you can print from Windows, you can [re-enable](tutorials.html#firewall) your firewall and use the [firewall tutorial section](tutorials.html#firewall) to add CUPS as a Service, and allow port 631 for both TCP and UDP eg.

![](images/hardware/printing/shared_printer8.png)



## Resources for compatible Printers

**Manufacturers**

[Brother Linux Drivers](http://www.brother.com/html/download/index.htm)  
[Canon Linux Drivers](http://www.canon-europe.com/support/)  
[Dell Printer Drivers](https://www.dell.com/support/home/nz/en/nzbsd1/?app=drivers)  
[Epson Linux Drivers](http://download.ebz.epson.net/dsc/search/01/search/?OSC=LX)  
[HP Linux Drivers](https://developers.hp.com/hp-linux-imaging-and-printing)  
[Lexmark Linux Drivers](https://www.lexmark.com/en_us/support/download-search.html)  
[Samsung Linux Drivers](https://support.hp.com/us-en/products/printers/samsung-printers)  
[Sharp Linux Drivers](http://www.openprinting.org/driver/Postscript-Sharp/) (supported printers list)  
[Toshiba Linux Drivers](http://www.openprinting.org/driver/Postscript-Toshiba/) (supported printers list)  
[Xerox Linux Drivers](http://www.openprinting.org/driver/Postscript-Xerox/) (supported printers list)

**Resources**

[Open Printing](http://www.openprinting.org/printers) - A substantial resource for driver downloads and information.  
[Ubuntu's](https://wiki.ubuntu.com/HardwareSupportComponentsPrinters) Wiki also contains a list of known working and compatible drivers and printers.  
[TurboPrint](http://www.turboprint.info/) - Also offers a paid software alternative that has up to date drivers for Brother, Canon, Epson & HP.  

## HP Printers on Linux Lite

HP compatible printers can be found [here](https://developers.hp.com/hp-linux-imaging-and-printing/supported_devices/index).

The latest master driver for HP printers is available for download [here](https://developers.hp.com/hp-linux-imaging-and-printing/gethplip) (Select Ubuntu). Changelog [here](https://developers.hp.com/hp-linux-imaging-and-printing/release_notes).

If you have an HP Printer and you used this guide to successfully install your printer, there is a program that allows you to easily manage your printer. Open up a terminal and type:

Terminal Command:

						sudo apt-get install hplip-gui

  

Once it's installed go to **Menu, Settings, HPLIP Toolbox**. This will place and HP icon in your tray where you can configure and manage your HP printer. Right click on the icon for options.

![](images/hardware/printing/printing-hplip.png)



## Bluetooth - Enabling full support

If you need support for this, please read through the thread [here](https://www.linuxliteos.com/forums/network/(solved)-enabling-full-bluetooth-support-in-linux-lite/).

Credit to - N4RPS, Wirezfree and colin23erk (may be out of date).



## Keyboard Related

You can find information for adding or modifying hotkeys (or shortcuts) on the [XFCE wiki](http://docs.xfce.org/xfce/xfce4-settings/keyboard).



## Booting Issues

**Black screen whilst trying to boot**

This is usually due to the graphics chip you have, it is easily remedied and the problem should not reappear once you have installed the [graphics drivers](#graphics) for your computer. So first we need to boot you successfully into the desktop.

Hold down the Shift or ESC key as you boot up your computer. You should see a screen like the following:

![](images/hardware/bootissues/bootissues1.png)

Next press the **e** key whilst that top line is highlighted. This will take you to the next screen. Use your arrow keys to move down to the line highlighted in the picture below. Use the arrow key until you reach the end of that line.

![](images/hardware/bootissues/bootissues2.png)

Press the backspace key repeatedly until you remove: **ro splash quiet $vt\_handoff** and replace that text with: **nomodeset** so that it looks like the picture below.

![](images/hardware/bootissues/bootissues3.png)

Now press either **F10** or **Ctrl+X** to boot your machine. Your computer will begin to boot up with scrolling text similar to what is shown below:

![](images/hardware/bootissues/bootissues4.png)

After which shortly you will get your normal login screen. Now you can login and install your [graphics drivers](#graphics).

![](images/install/login.png)

## Dual Boot Modification/Repair

You may be in a situation where you want to modify or repair your dual boot set up.

**Boot Repair** is an excellent tool for the job. To install **Boot Repair**, open a terminal and type (one line at a time):

Terminal Command:

						sudo add-apt-repository ppa:yannubuntu/boot-repair

  

Terminal Command:

						sudo apt-get update

  

Terminal Command:

						sudo apt-get install -y boot-repair && (boot-repair &)

  

After the install **Boot Repair** will launch automatically and scan your computer for your boot configuration and other operating systems.

![](images/hardware/bootrep/bootrep1.png)

![](images/hardware/bootrep/bootrep2.png)

Click **Advanced options** to see all the features.

![](images/hardware/bootrep/bootrep3.png)

Now use **Boot Repair** to carry out the task you need doing. **Boot Repair** is in **Menu, System, Repair the boot of the computer**. More information can be found here - [https://help.ubuntu.com/community/Boot-Repair](https://help.ubuntu.com/community/Boot-Repair)



## Installation Issues

**No Option to Install Alongside Windows?**

If this happens, it usually means that Windows is already using four partitions on the hard drive, which is the limit for BIOS based computers using traditional MBR type partitions. (Newer computers may that use UEFI firmware _may_ use GPT partitioned drives that do not have the 4 partition limit. This discussion does not get into that.) You will need to either eliminate one of the current partitions, or add another hard drive to the computer for installing Linux Lite.

If you are unfamiliar with partitioning, it would be best to make a post on the [Forums](https://www.linuxliteos.com/forums/) for help before proceeding. Generally speaking, in this situation there is may be a partition set aside where the manufacture has put copies of drivers and other extras that were part of the initial installation. There may also be a recovery partition that gets used for reinstalling Windows in the event that is needed. If you went through the process of creating a recovery USB or set of recovery DVD's, then you can probably get rid of the recovery partition. Same goes for the partition set aside for manufacturer installed drivers and extras, if you made a copy of that.

Once one or both of those partitions has been deleted, you may also need to shrink the main (largest) Windows partition (probably labeled as "C: drive"). If you have the space, ideally you should try to allocate 50-100GB for Linux Lite. (It will be fine with +/-15GB; but you won't have much room for expansion). Before shrinking any partition, be sure to defragment the partition in Windows first. Then shrink the partition and leave the free space as it is, un-partitioned. Do not create Linux partitions with Windows disk manager. It is best done using Linux tools.

At that point, you can go ahead and run the installer again and it should now offer the choice to install "Alongside Windows". If it needs to it will create an "extended" partition that will serve as a container for the "logical" partitions needed for the installation. (That is a way that is commonly used to get around the 4-partition maximum rule. As long as only 3 partitions are "primary", an extended partition can be used to house multiple logical partitions within it - thus giving you the ability to have more than four partitions.)

**Does Your Newer Computer Use UEFI Firmware for Booting?**

If you have a newer model computer with UEFI firmware, it may allow for two modes of booting: UEFI/EFI-mode or BIOS/CSM/Legacy-mode. There is a good chance that Windows is installed to the hard drive in UEFI-mode. In that case it will also be using the newer GPT partitioning scheme on the hard drive. (This applies mainly to Windows 8, but some versions of Windows 7 may be installed that way too.)

You need to confirm for sure which way Windows is installed before attempting the Linux Lite installation. The first thing to check is whether or not you are using a 64-bit version of Windows. You should be able to find that out by going to the "System" section from the "Control Panel". If you find that it is a 32-bit version, then you **will** be able to install Linux Lite. (Only 64-bit versions of Windows currently support UEFI booting.)

If you have a 64-bit version of Windows, it could be installed in either BIOS/Legacy-mode or in UEFI-mode; so you will need to investigate further. Go to Windows disk management and take a look at the partitions on the hard drive. If you see a small partition near the beginning of the drive, formatted as **FAT32**, labeled along the lines of "System" or "EFI System Partition", then you have a UEFI installation of Windows and **will not** be able to properly install Linux Lite. If you don't see that partition, then you should have an MBR-partitioned disk and you **can** install Linux Lite. If you need help figuring that out, take a screenshot of your hard drive partitions and post that to the [Forums](https://www.linuxliteos.com/forums/) with your inquiry.

## Dual Boot Install on Systems with More Than One Hard Drive?

When choosing to install Linux Lite alongside Windows on a computer with more than one hard drive, the default action of the installer is to install the Linux boot loader to the MBR of the first hard drive. Since Windows is likely installed to the first drive, its boot loader will be replaced on the MBR with the Linux boot loader. The Linux boot loader will see the Windows installation and add it to the boot menu on start-up. This is how most people do the installation.

However, some people prefer to keep the Windows boot loader intact on its own drive and install the Linux boot loader to its own drive. (There are various reasons for doing that, the most common being that it makes booting Windows easier if they decide to remove the Linux installation.) After the installation completes, they then set the computer's BIOS to boot from the Linux drive. Even though the Linux boot loader is installed to a separate drive, it will see the Windows installation and add a boot choice for it. By booting from the Linux drive, you get the choice to boot either OS. If you later remove Linux, simply reset the BIOS to boot from the Windows drive and it will boot Windows as it did before your installation of Linux.

To accomplish this, you must choose the "Something else" option from the "Installation Type" screen during installation. On the following screen you will set-up your partitions and mount points manually. Then, near the bottom of the window, you need to set the "location for boot loader installation" to the MBR of the drive containing Linux Lite. For example, if you had two hard drives - /dev/sda (Windows) and /dev/sdb (Linux) - you would set the location to /dev/sd**b** (without any partition number at the end).

If you are not experienced with partitioning, or are unsure about how to proceed, post on our [Forums](https://www.linuxliteos.com/forums/) for assistance.



## Lite System Report tool

The **Lite System Report** tool was created to better help people who experienced a problem with their computer. The report contains useful information about the hardware, network and software. The idea of the tool is to run it, then you would attach the generated file to a [Forum](https://www.linuxliteos.com/forums/) thread with a title about the issue you are having. Lets get started.

Click on **Menu, Settings, Lite System Report**.

![](images/hardware/sysreport/systemreport1.png)

A window will pop open, read the information and click on **Continue** when ready.

![](images/hardware/sysreport/systemreport2.png)

Enter your password and press the Enter key.

![](images/hardware/sysreport/systemreport3.png)

Unselect the options you don't need to or have been asked to exclude from your Report.

![](images/hardware/sysreport/systemreport4.png)

The report will take anywhere from a few seconds to less than a minute depending on your hardware.

![](images/hardware/sysreport/systemreport5.png)

When it is finished, the Report will appear. The Report will be similar to the one below. Click on **Save**.

![](images/hardware/sysreport/systemreport6.png)

Next you'll be asked where to save the Report, in the following example we select our Home folder (**/home/jerry**).

![](images/hardware/sysreport/systemreport7.png)

In this example the Report is located in **/home/jerry**.

![](images/hardware/sysreport/systemreport8.png)

Go to the Linux Lite Forums. A link is provided here - [http://www.linuxliteos.com/forums/](https://www.linuxliteos.com/forums/) Start a new thread with an accurate Title description of the problem you are having, then a detailed write up of your problem. At the bottom of the page you will see where you can add attachments. **Browse** to **/home/youruser** and select the report.

![](images/hardware/sysreport/systemreport9.png)

Now click on **Post**, and someone will help you as soon as they're available.



## Finding help online

Feel free to seek advice or help on the [Forums](https://www.linuxliteos.com/forums/) at any point. Or use any other means of support or contact located [here](https://www.linuxliteos.com/support.html). If you can not find a solution contained in this page or links of related information.
