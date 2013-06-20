Windows Installer (WiX) for Apache Maven 2
==========================================

This project folder contains most of the files you need to build a WiX based installer
for Apache Maven 2.  The project file (Maven2.Setup.wixproj) is a Microsoft Visual Studio 2012
project - and may be built with any version - or using MSBuild.

The current version is specified in the .\Includes\Maven2Variables.wxi.

To build the project you will need to download and extract Apache Maven 2.2.1 into a
.\apache-maven-2.2.1\ folder. - from http://maven.apache.org/download.cgi

Change Log
==========
09-JAN-2013

	Original version of the installer published on the Kajabity.com blog in binary form only.

12-JUN-2013

	


Included Files and Folders
==========================

.\apache-maven-2.2.1\

	Download and extract a copy of Apache Maven 2.2.1 into this folder.  See the README.md in that folder for details.

.\Includes\

	Holds include files for the project.  The Maven2Variables.wxi file is here and contains details such as the 
	product name, version number and Upgrade GUID.

.\LICENSE.rtf

	A copy of the Apache 2.0 License for inclusion in the Installer.

.\Maven2.Setup.wixproj

	The Microsoft Visual Studio 2012 project file.

.\Maven2.wxs

	This is the main WiX source file for the Apache Maven 2 installer.

.\Maven2URL.txt

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

	The build process will capture the Apache Maven 2 files in a WiX fragment file, 
	Maven2FilesFragment.wxi, in this directory

.\Maven2.Setup.wixproj.user

	Created when you load the project into Visual Studio to hold user specific settings and passwords.
