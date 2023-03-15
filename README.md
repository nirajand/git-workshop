# Git and GitHub Workshop/ Training at Gandaki University


<b>Hello and welcome to Git and GitHub Workshop. </b>

<img src="https://o.remove.bg/downloads/0317f84a-b38d-49ea-94ef-0656c88bfb3f/1color-orange-lightbg_2x-removebg-preview.png" height=150 width=400 alt="Git Image"> &nbsp; <img src="https://lthub.ubc.ca/files/2021/06/GitHub-Logo.png" height=150 width=300 alt="Github Image">

<br>

Here you will learn:
- How to Use *Terminal* or *Command Prompt* on your computer, 
- About **Git**, **GitHub** and **Visual Studio Code** (VS Code),
- How to use **Git** from **Terminal**,
- How to use VS Code and use **Git**, **Github** from *VS Code*.

<br>

If you are **Windows 11** user, you will find **Terminal** when you `Right-Click` on your screen. In Windows 10 and lower versions, you will find **Command Prompt**. To open Command Prompt, hold `Windows` key and press `R` (`Windows + R`) key at the same time. A dialogue box appears. Type `cmd`and press `Enter` key. A black screen appears which is Terminal / Command Prompt.

<br>

We will download few applications to save our time. We will have to download **Git**, **GitHub Desktop Application** , **GCC Compiler** for C programming compiler and **Visual Studio Code**. Please note that you are instructed to download the applications only. Do not install right after you install because it might fail when working with the applications. You can install **Github Desktop Application** and **VS Code** after you install because you have to set `Environment Variables` in `PATH` directory for **Git** and it can be overwhelming. **VS Code** takes long time to install in the device, and to continue with our work, please install it after the file is downloaded.  Follow the following links to download specific applications:

- To *Download* **Git**, [Click Here](https://git-scm.com/downloads). As of writing, **Git** version is 2.40.0. For your simplicity, there is a monitor icon at the right side on the website. You can download from that button. **Git** comes pre-installed in **Linux Distribution OSS**, so you don't need to download and install **Git**.

- To *Download* **Github Desktop Application**, [Click Here](https://desktop.github.com/). It is advised that you install this application.

- To *Download* **Visual Studio Code**, [Click Here](https://code.visualstudio.com/download). It is advised that you install this application. Follow [this instructions](https://youtube.com/watch?v=JPZsB_6yHVo) from **YouTube** to properly setup **Visual Studio Code** on your computer.

- To *Download* **Mingw** (**GCC Compiler**), To *Set Up* **VS Code** for **GCC Compiler**, please follow the instructions from the videos in the link below:
  
  - To *Download* **Mingw**, follow [this link](https://youtu.be/0HD0pqVtsmw)
  
  - To setup **VS Code** for writing and executing C and C++ programs, follow [this link](https://youtu.be/77v-Poud_io)


---


### Before We Dive In Into Git and Github, We Will Learn Simple *Terminal* Commands To Ease Up Our Workflow:

1. Changing Directory (Accessing Directory): ```cd```

   For example: To access Desktop, type ```cd desktop```. Note that there should be a whitespace (space) between `cd` and `desktop`. If `desktop` doesn't work, type `Desktop`.
   
   Again, to access a Directory (Folder) inside Desktop (If your computer has), type ```cd folderName``` where `foldername` is the name of the folder/ directory you want to access to.

2. Changing Drive Root: ```driveName:```
   
   ```driveName``` is the name of drive that you are currently on. Typically, you are in ```C:``` drive when you first open *Terminal*. To change the drive root, type the `name of drive` (capital letter) followed by `:` (colon).
   
   For example, I am currently in ```C:``` drive. If I want to go to ```N:``` drive, I will type ```N:``` and press `Enter` key.

3. Reaching Parent Directory: ```cd..```
  ```cd``` followed by two periods (fullstops).

4. Reaching Root Directory: ```cd\```
   `cd` followed by a backward slash.
   
5. Reaching to a folder from folder path:  ```cd\folderName\subFolderName```

   Reaching to a folder with less effort: ```cd initialLettersOfFolderName Tab Key```. Here, type `cd` and `space`, then type two or three letters of the folder and press ``Tab`` key.
   
---

6. Creating a Directory/ Folder: ``` mkdir directoryName ``` or ``` md directoryName ```
   
   For example, if you want to create a directory or a folder with name `Test Folder`, type `mkdir Test Folder`. You can use `mkdir` or `md` to create a directory.
   
7. To Know About the System Information: `systeminfo`

8. To Know In Which Volume Are We Working: `vol`

9. To Know the Version of Operating System (OS): `ver`

10. To Know Folder Content of a Certain Directory: `dir`

11. To **Rename** a file/ Folder: `ren oldFileName.fileType newFileName.fileType` or `rename oldFileName.fileType newFileName.fileType`

11. To **Delete** File: `erase fileName.fileType` or `del fileName.fileType`

12. To **Delete** Directory / Folder: `rmdir directoryName`

13. To check ping: `ping siteName`
   
   For example, I can do: `ping google.com` to check ping. It will display the following output as of writing:
   
     Pinging google.com [185.199.109.153] with 32 bytes of data:
     Reply from 185.199.109.153: bytes=32 time=71ms TTL=50
     Reply from 185.199.109.153: bytes=32 time=70ms TTL=50
     Reply from 185.199.109.153: bytes=32 time=70ms TTL=50
     Reply from 185.199.109.153: bytes=32 time=71ms TTL=50

     Ping statistics for 185.199.109.153:
       Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
     Approximate round trip times in milli-seconds:
       Minimum = 70ms, Maximum = 71ms, Average = 70ms


---

