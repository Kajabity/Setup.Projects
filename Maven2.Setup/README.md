Windows Installer (WiX) for Apache Maven 2
==========================================

This project folder contains most of the files you need to build a WiX based installer
for Apache Maven 2.  The project file (Maven2.Setup.wixproj) is a Microsoft Visual Studio 2012
project - and may be built with any version - or using MSBuild.

The current version is specified in the .\Includes\Maven2Variables.wxi.

To build the project you will need to download and extract Apache Maven 2.2.1 into a
.\apache-maven-2.2.1\ folder. - from http://maven.apache.org/download.cgi