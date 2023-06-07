# Git and GitHub Training (Workshop) at Gandaki University


Author: **<u>Nirajan Dhakal</u>**

<img src="https://www.freecodecamp.org/news/content/images/2022/07/git-github.png" height=120 width=230 alt="Git Image">&nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp;<img src="https://www.elegantthemes.com/blog/wp-content/uploads/2019/01/000-VS-Code.png" height= 120 width = 230 alt= "Visual Studio Code Logo">

Credit: FreeCodeCamp  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; Credit: Elegant Themes

![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)&nbsp;
![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)&nbsp;
![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-0078d7.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white)&nbsp;
![C](https://img.shields.io/badge/c-%2300599C.svg?style=for-the-badge&logo=c&logoColor=white)&nbsp;
![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)&nbsp;
![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)&nbsp;
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)&nbsp;
![NodeJS](https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white)&nbsp;
![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)&nbsp;

<br>

<strong>It is advised that you read all the text here once throughly and then return to the top to follow the instructions on what and how to do things for this workshop.</strong>

Here you will learn:
- How to Use *Terminal* or *Command Prompt* on your computer, 
- About **Git**, **GitHub** and **Visual Studio Code** (VS Code),
- How to use **Git** from **Terminal**,
- How to use VS Code and use **Git**, **Github** from *VS Code*.

<br>

If you are **Windows 11** user, you will find **Terminal** when you `Right-Click` on your screen. In Windows 10 and lower versions, you will find **Command Prompt**. To open Command Prompt, hold `Windows` key and press `R` (`Windows + R`) key at the same time. A dialogue box appears. Type `cmd` and press `Enter` key. A black screen appears which is Terminal / Command Prompt.

<br>

To properly utilize our time, please download the following programs:

- **Git**,
- **GitHub Desktop Application**,
- **GCC Compiler** for C/C++ programming compiler (If you are going to write and compile C programs, you can install MingW and GCC compiler. Else, it is not necessary) and
- **Visual Studio Code**

<strong> The path to download each program is provided below.</strong>


Note that you download all the necessary applications first and do not go on installing right into your computer after it is downloaded. After you download all the applications, please install **VS Code** and **GitHub Desktop Application** but do nothing as the settings might affect. For **Git**, you have to set `Environment Variables` in `PATH` directory, which can be overwhelming. **VS Code** takes long time to install in the device, and to continue with smoothy work, please install it after the file is downloaded.  Follow the following links to download specific applications:

## Download:

- To *Download* **Git**, [Click Here](https://git-scm.com/downloads). As of writing, **Git** version is 2.40.0. For your simplicity, there is a monitor icon at the right side on the website. You can download from that button. **Git** comes pre-installed in **Linux Distribution OSS**, so you don't need to download and install **Git**.


- To *Download* **Github Desktop Application**, [Click Here](https://desktop.github.com/). It is advised that you install this application.

- To *Download* **Visual Studio Code**, [Click Here](https://code.visualstudio.com/download). It is advised that you install this application. Follow [this instructions](https://youtube.com/watch?v=JPZsB_6yHVo) from **YouTube** to properly setup **Visual Studio Code** on your computer.


<br>

If you have any problem regarding `Git`, please visit [this url](https://stackoverflow.com/questions/315911/git-for-beginners-the-definitive-practical-guide). This is redirect hyperlink to Stackoverflow ang 

If you have any problem in downloading Git, go to a pdf file [here](https://github.com/dhakalnirajan/git-workshop/blob/main/Git%20PDF%20Files/what%20is%20git.pdf) and read the document, you will find the solution. The PDF is large, and GitHub won't show the file in the Rendered Block. Download the file and look into it.

To Follow the Git Manual, go to the [Manual](https://github.com/dhakalnirajan/git-workshop/blob/main/Git%20PDF%20Files/Progit-Git%20Manual.pdf) and follow along.


- To *Download* **Mingw** (**GCC Compiler**), To *Set Up* **VS Code** for **GCC Compiler**, please follow the instructions from the videos in the link below:
  

  - To *Download* **Mingw**, follow [this link](https://youtu.be/0HD0pqVtsmw)


-------------   **Mingw** and **GCC Compiler** are necessary to compile and run C/ C++ programs. If you are not contributing related to  or C++ programming languages, it is not necessary to install them.    -------------------

  
<b> ULTIMATE VS CODE AND GCC COMPILER ALONG WITH C PROGRAMMING REFERENCE </b>
   
   [Click Here](https://youtu.be/irqbmMNs2Bo) for the Ultimate Resource.

<br>


- To setup **VS Code** for writing and executing C and C++ programs, follow [this link](https://youtu.be/77v-Poud_io)

- To *Download* **NodeJS** to execute **JavaScript** program, follow [this link](https://nodejs.org/en)


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
   

---

Go to [Git.md](https://github.com/dhakalnirajan/git-workshop/blob/main/Git.md) to learn about Git, GitHub, and many more!

---

If you have been follwing the Git.md file, when you commit to a repository on GitHub, you will encounter with a error that needs you to have agreed to Contributor's License Agreement (**CLA**). To do that, go to [https://cla.developers.google.com/about/google-individual](https://cla.developers.google.com/about/google-individual) and read the terms of the agreement, and provide your GitHub username and the mailing address that was used to sign in into GitHub so as to maintain commits to the Open Source Community.
