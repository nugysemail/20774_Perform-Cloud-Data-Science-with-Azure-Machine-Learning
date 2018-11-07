# 20774A: Perform Cloud Data Science with Azure Machine Learning

## Virtual Machine Setup

All students and the instructor must perform the following tasks prior to commencing module 1:

### Start the VMs

1.  In Hyper-V Manager, under Virtual Machines, right-click **MT17B-WS2016-NAT**, and then click **Start**.
2.  In Hyper-V Manager, under Virtual Machines, right-click **20774A-LON-DC**, and then click **Start**.
3.  In Hyper-V Manager, under Virtual Machines, right-click **20774A-LON-DEV**, and then click **Start**.
4.  In Hyper-V Manager, under Virtual Machines, right-click **20774A-LON-SQLR**, and then click **Start**.
5.  Right-click **20774A-LON-DEV**, and then click **Connect**.
6.  Log in as **Admin** with the password **Pa55w.rd**.

### Install RStudio on the LON-DEV VM

1.  In Internet Explorer, browse to **https://download1.rstudio.org/RStudio-1.0.136.exe**.
2.  In the Internet Explorer message box, click **Run**.
3.  In the **User Account Control** dialog box, click **Yes**.
4.  In the **RStudio Setup** wizard, on the **Welcome to the RStudio Setup Wizard** page, click **Next**.
5.  On the **Choose Install Location** page, click **Next**.
6.  On the **Choose Start Menu Folder** page, click **Install**.
7.  On the **Completing the RStudio Setup Wizard** page, click **Finish**.
8.  Click the Windows Start button, and in the **Recently added** list, click **RStudio**.
9.  In the RStudio Console, type the following command and then press Enter.
    ````
    remoteLogin("http://LON-SQLR:12800", session=TRUE, commandline=TRUE, diff=TRUE)
    ````
10. In the **Remote Server** dialog box, in the **User name** box type **admin**, in the **Password** box, type **Pa55w.rd**, and then click **OK**.
11. In the RStudio Console, verify that a remote R session starts successfully.
12. Type **exit** to close the remote session.
13. Close RStudio without saving the workspace image. 

### Install PuTTY on the LON-DEV VM

1.  In Internet Explorer, browse to **https://the.earth.li/~sgtatham/putty/0.68/w64/putty-64bit-0.68-installer.msi**.
2.  In the Internet Explorer message box, click **Run**.
3.  In the **PuTTY release 0.68 (64-bit) Setup** wizard, on the **Welcome to the PuTTY release 0.68 (64-bit) Setup Wizard** page, click **Next**.
4.  On the **Destination Folder** page, click **Next**.
5.  On the **Product Features** page, click **Install**.
6.  In the **User Account Control** dialog box, click **Yes**.
7.  When the wizard has completed, clear the **View README file** check box, and then click **Finish**.
8.  Right-click the Windows Start button, and then click **System**.
9.  In the **System** dialog box, click **Advanced system settings**.
10. In the **System Properties** dialog box, click **Environment Variables**.
11. In the **Environment Variables** dialog box, click **Path**, and then click **Edit**.
12. In the **Edit User Variable** dialog box, append the path **C:\Program Files\PuTTY** to the **Variable Value**, and then click **OK**.
13. In the **Environment Variables** dialog box, click **OK**.
14. In the **System Properties** dialog box, click **OK**.
15. Close the System dialog box.
16. Open a command prompt window.
17. In the command prompt window, type the following command, and then press Enter:
    ````
    putty
    ````
18. Verify that the PuTTY Configuration window appears, and then click **Cancel**.
19. Close the command prompt window.
20. Log out of the virtual machine.
