Windows Installer (WiX) for Apache Maven 3
==========================================

This project folder contains most of the files you need to build a WiX based installer
for Apache Maven 3.  The project file (Maven3.Setup.wixproj) is a Microsoft Visual Studio 2012
project - and may be built with any version - or using MSBuild.

The current version is specified in the .\Includes\Maven3Variables.wxi.

To build the project you will need to download and extract Apache Maven 3.0.5 into a
.\apache-maven-3.0.5\ folder - from http://maven.apache.org/download.cgi

Visit http://www.kajabity.com/category/apache-maven/ to find out more.

Change Log
==========

12-JUN-2013

	Created Apache Maven 3 installer based on Apache Maven 2 installer.
	Included Java version checking.
	Added README.md files.
	First uploaded to GitHub.

27-SEP-2013

    Added a custom action (C++ and a C# version I've deleted) to broadcast a WM_SETTINGCHANGE
	to tell Windows programs the Environment variables have changed.
	Soon after added modified to add both ANSII and Unicode to support Win 8.
	Changed to use "set" instead of "create" to force update of M2_HOME and M2.

Included Files and Folders
==========================

.\apache-maven-3.0.5\

	Download and extract a copy of Apache Maven 3.0.5 into this folder.  See the README.md in that folder for details.

.\Includes\

	Holds include files for the project.  The Maven3Variables.wxi file is here and contains details such as the 
	product name, version number and Upgrade GUID.

.\LICENSE.rtf

	A copy of the Apache 2.0 License for inclusion in the Installer.

.\Maven3.Setup.wixproj

	The Microsoft Visual Studio 2012 project file.

.\Maven3.wxs

	This is the main WiX source file for the Apache Maven 3 installer.

.\Maven3URL.txt

	This file contains a URL in a form that can be used by the WiX installer to create a Start Menu link 
	to the Apache Maven web site.

Other Files and Folders
=======================

The following files or folders are not included in the GitHub distribution but may be created in later
versions or by the build process.

.\bin\

	The output directory where the installer and associated files will be placed.

.\obj\

	The output directory where intermediate build files are placed.

.\CustomActions\, .\CustomDialogs\, .\Lang\, .\Resources\

	Directories provided by the project template which I haven't yet used.

.\Dist\

	Somewhere to collect successful builds of the project - ready for distribution.

.\Fragments\

	The build process will capture the Apache Maven 3 files in a WiX fragment file, 
	Maven3FilesFragment.wxi, in this directory

.\Maven3.Setup.wixproj.user

	Created when you load the project into Visual Studio to hold user specific settings and passwords.
