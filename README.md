# Configuration Overview 
- Only Install Word, Excel, and PowerPoint
- Only works on 64-bit Windows system
- Office language installed is only English US (Without additional languages or proofing)
- Override (Uninstall) any existed MSI-based Office edition (like 2007, 2010..)

# Usage
1. Download office deployment tool [here](http://go.microsoft.com/fwlink/?LinkId=691958) and put setup.exe in same directory with the xml configuration files. 365.xml for office 365, 2021.xml is for office 2021 and so on. Difference between them is [here](https://support.microsoft.com/en-us/office/what-s-the-difference-between-microsoft-365-and-office-2024-ed447ebf-6060-46f9-9e90-a239bd27eb96)
2. Copy the directory address
3. Open elevated (run as administrator) command prompt and paste the directory, example we used here: `cd /d C:\office`
4. Download the office data, run `setup.exe /download 365.xml` don't close the command prompt window and wait until command finishes to run. Although no activity showed on command prompt, the download is running on the background
5. Install the office, run `setup.exe /configure 365.xml` wait until installer finishes

Read here for further documentation:
https://learn.microsoft.com/en-us/microsoft-365-apps/deploy/overview-office-deployment-tool
