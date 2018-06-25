# Setup

Configurations needed to work on the Azure labs.

## Courseware

1. Go to [Skillpipe](https://skillpipe.com/en-GB/).
1. Register or login with your account. If registering use a personal email address.
1. Select `Add a Course` and use the code given to you by the instructor.

## MIA-CL1 Virtual Machine 🖥️

Following are the steps to configure the `MIA-CL1` virtual machine:

1. Open `Virtual Machine Settings` via `Hyper-V Manager`.
1. Adjust the `Processor Count` to `4`.
1. Adjust the `Memory` as needed (10240 MB).
1. Set the `Network Adapter` to the `External Network` virtual switch.
1. Click `OK`.
1. Right Click `MIA-CL1` and select `Checkpoint`.
1. Right Click `MIA-CL1` and select `Start`.

## MIA-CL1 Network 🖧

Once `MIA-CL1` is running we need to configure the network:

1. Connect to the `MIA-CL1` virtual machine via `Hyper-V Manager`.
1. Login with the password `Pa55w.rd`
1. Right Click the `Start Menu` and select `Network Connection`.
1. Right Click the `Ethernet` network connection and select `Properties`.
1. Click on `Internet Protocol Version 4 (TCP/IPv4)` and then click `Properties`.
1. Select the top option `Obtain an IP address automatically`.
1. Select the middle option `Obtain DNS server address automatically`.
1. Click `OK` and then `Close` (select `Yes` if the network side panel shows up).
1. Right click the `Start Menu` and select `System`.
1. Click `Remote Settings` on the left menu.
1. Select the option `Allow remote connections to this computer`.
1. Click `OK`.
1. Use the `Start Menu` to open PowerShell and run `ipconfig`.
1. Write down the `IPv4 address` of `MIA-CL1`.
1. Close the `Connect` window.

## MIA-CL1 Desktop 🗔

The `MIA-CL1` desktop needs some final changes before we use it for labs:

1. On the host desktop open `Remote Desktop Client` from the `Start Menu`
1. Connect to `MIA-CL1` via its `IP address`.
1. Open Internet Explorer or Edge.
1. Download and install Firefox.
1. Set Firefox as the default browser.
1. Open `PowerShell` as Administrator.
1. Type `Update-Module -Name AzureRM -Force` and press enter.
1. Obtain the `AllFiles` ISO file from the instructor.
1. On the host use `Hyper-V Manager` to connect to `MIA-CL1`.
1. Use the `Media` menu in `Virtual Machine Connection` to mount the ISO file (insert disk).
1. Inside `MIA-CL1` copy the directories from the `ISO` file to the root of `E:` drive.
   * 20533 should look like this:
     * E:\Configfiles
     * E:\Demofiles
     * E:\Labfiles
     * E:\Modules
   * 10979 should look like this:
     * E:\Demofiles
     * E:\Labfiles

## Email Address 📧

__Do not use your existing Microsoft accounts to work with the labs!__

1. Open [Outlook.com](https://outlook.live.com/owa/).
1. Create a new `Outlook.com` account. Use your last name with the date eg: carthew20180618@outlook.com
1. Use this email address to create your Azure account.

## Azure Account ⚿

To create an Azure subscription you need to prove you are a person and an adult. This is done with a credit card. If you have been supplied with an Azure Pass you can avoid the need to use a credit card:

1. Open one of the links below and create your Azure account:
   * Azure Pass: https://www.microsoftazurepass.com/
   * Trial Account (Credit Card Required): https://azure.microsoft.com/en-us/free/
1. Follow the steps to create your Azure account.



