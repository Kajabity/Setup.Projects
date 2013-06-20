Windows Installer (WiX) for Apache Maven 3
==========================================

This project folder contains most of the files you need to build a WiX based installer
for Apache Maven 3.  The project file (Maven3.Setup.wixproj) is a Microsoft Visual Studio 2012
project - and may be built with any version - or using MSBuild.

The current version is specified in the .\Includes\Maven3Variables.wxi.

To build the project you will need to download and extract Apache Maven 3.0.5 into a
.\apache-maven-3.0.5\ folder - from http://maven.apache.org/download.cgi

Files and Folders
=================

.\apache-maven-3.0.5\

	Download and extract a copy of Apache Maven 3.0.5 into this folder.

bin

	The output directory where the installer and associated files will be placed.

CustomActions, CustomDialogs, Lang

	Directories provided by the project template which I haven't yet used.