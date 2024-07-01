# How to Set Up Tenable Nessus to Scan a Windows 10 VM on VirtualBox for Vulnerabilities

To demonstrate my skill and experience with vulnerability scanning, I will walk you through the process of downloading, installing, and configuring Tenable Nessus to scan a Windows 10 machine running on VirtualBox for vulnerabilities. Nessus is a powerful vulnerability scanner that helps identify and fix security issues.

Lab requirements:
1. VirtualBox installed on your host machine.
2. A Windows 10 virtual machine installed and running on VirtualBox.
3. Tenable Nessus -  Download on their website (https://www.tenable.com/downloads)

After the installation is complete, Nessus will start its service and open the default web interface on https://localhost:8834.

## 1. Configure VirtualBox Networking
1. Under Settings > Network.
2. Ensure that Adapter 1 is enabled and attached to NAT.
3. Add Adapter 2, enable it, and attach it to Host-Only Adapter. This setup allows Nessus on the host machine to communicate with the VM.

## 2. Get Windows 10 VM IP Address:
1. Start your Windows 10 VM.
2. Open Command Prompt and type ipconfig to find the IP address of the VM's host-only adapter.

## 3. Scan Windows 10 VM with Nessus
1. Create a New Scan:
2. Go back to the Nessus web interface.
3. Click on Scans in the left sidebar, then click New Scan.
4. Choose the Basic Network Scan template.
5. Enter a name for your scan.
6. In the Targets field, enter the IP address of your Windows 10 VM.
7. Click on Save, then click on the Launch button to start the scan, Nessus will begin scanning the specified IP address for vulnerabilities.

Optional: Scans can be configure to be scheduled under advanced settings.

## 4. Scan Windows 10 VM with Nessus
1. Create a 


## Conclusion
By following these steps, you can effectively set up Tenable Nessus to scan your Windows 10 virtual machine on VirtualBox for vulnerabilities. Regular vulnerability scanning is a crucial part of maintaining a secure network environment.

Happy scanning!

