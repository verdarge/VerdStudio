<p align="center">
  <img src="https://www.verd.com.tr/content/img/logo.png" />
</p>

About
-----

The VERD Studio is an integrated development environment for VERD programming language. It allows a user to upload VERD project files, compile and run VERD projects, and debug them. Users can also search and replace in files within VERD Studio.

VERD Studio works with workspaces. A workspace is simply a collection of projects grouped together. In VERD Studio user can create new workspaces or add existing workspaces. In initial screen of VERD Studio user can choose from one of the workspaces that are previously added or created. 

VERD Studio keeps mainly three types of files to maintain its operations. First file that VERD Studio keeps is login file. Login file keep track of information such as workspace path and name about workspaces that are previously created or added.  Second file that VERD Studio keeps is workspace files. Workspace files are in XML format and include information about the projects such as project path, project name and breakpoints that projects have. Last file that VERD Studio keeps is project files. Each project in a workspace should have a project file. Project files are in XML format and include information about folder structure of project and files included in project. 

VERD Studio supports Unicode characters in workspace paths, folder paths, file paths and file names. VERD Studio requires all files including login, workspace, project and source code files to be encoded in UTF-8 format. VERD Studio also supports Unicode characters during searching and replacing source code files.

Source code files that VERD Studio uses should have the “.v” extension which indicates that source code file is VERD language source code file.

VERD Studio is freeware for non-commercial use.

Functions supported by VERD Studio
---------

| Function                                                   | 
| :----------------------------------------------------------| 
| Create new Workspace                                       | 
| Add existing Workspace                                     | 
| Import existing project                                    | 
| Create a new VERD Project                                  | 
| Open and close a VERD Project                              | 
| Create a new folder or a file                              | 
| Delete an existing VERD project                            | 
| Remove an existing VERD project from workspace             |
| Rename a VERD project                                      |
| Copy & Paste a folder                                      |
| Copy & Paste a file                                        |
| Delete an existing folder or file                          |
| Rename a folder or file                                    |
|	Search and Replace in the current file or workspace        |
| Format Selected Text                                       |
| Build, Run and Debug VERD Project                          |
| Build Workspace                                            |

Detailed explanations and screenshots for each functionality can be found in VERD Studio Reference Manual.

VERD Programming Language
-------

VERD is a high-level programming language designed to ease ERP development and database reporting. VERD is an abbreviation for “**Veri Tabanı Raporlama Dili**” in Turkish. “Veri Tabanı Raporlama Dili” in Turkish means “**Database Reporting Language**”

VERD language takes some features from **ABAP**, **C** and **HTML**. It was developed by using **C++** and **JavaScript** languages. Development of VERD programming language dates back to 2015.

VERD language runs in either embedded or client/server mode. In embedded form client and server runs in a single application. Embedded form is used mainly for debugging purposes. Server is core of the language in client/server mode and is written by using C++ language. Client and server communicate by exchanging XML data. Client can be written in any language (**C++**, **Javascript**, **Python** etc.)

Currently, **C++** and **Javascript** (Web) Clients are available. **C++** Client is written by using **WxWidgets** and **Expat** libraries. **SlickGrid** and **Bootstrap** javascript libraries are used for Web Client.

VERD programming language currently supports only **Firebird** database management system. In the future, it is planned to add support for **SQL Server**, **PostgreSQL**, **MariaDB** and **Oracle** database management systems.

Installation
-------
VERD Studio currently runs only in Windows. VERD Studio can be installed by using **msi installer** that can be found in **Releases** section. VERD Studio comes with embedded form of VERD programming language conponents such as VERD compiler, VERD runtime and VERD debugger. 

VERD Studio installs its files into path specified during installation. Default installation location is "**Program Files (x86)**" folder. One of files that VERD Studio installs, is login file that is modified by VERD Studio. If installation location is protected as in the case of default installation location, VERD Studio elevates to administrative privileges to modify login file during operations such as adding or creation workspace. If you don't want VERD Studio to elevate, you can change read write permisssion of login file by using following commands in cmd that is run as administrator. 

<code>cd C:\Program Files (x86)\VerdStudio && icacls Login.xml /grant Users:(f)</code>

Example Workspace and Database
-------



