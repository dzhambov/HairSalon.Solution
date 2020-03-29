# _Eau Claire's Salon_

#### _A C# MVC application to track stylists and clients by category._, _March 20, 2020_

#### By _**Hristo Dzhambov**_

## Description

_A web application that helps a hair salon owner to manage the stylists and thier clints. The owner is able to see the list of stylists and their clients,add new stylists and clients to that particular stylist._

## Project Specifications

| Behavior | Input | Output |
|---|:---:|:---:|
|The program displays a welcome message "Welcome to the Eau Claire's Salon!" and two links for viewing stylists "See all stylists" and viewing clients "See all clients"|User enters the following url: http://localhost:5000| Welcome Message: "Welcome to the Eau Claire's Salon!"|
|User clicks on "See all stylists" or "See all clients" and is routed to the corresponding view with options to add new stylist or client|User clicks on link and the programs displays currently added clients or stylists|Stylist:   Client:|
|A user clicks the "add new stylist/client" link and is routed to a new stylist/client view where they can insert stylist/client details. Once the user inputs the details, the user can hit submit and will be routed to the stylists/clients view|User clicks on selected "add new" link and inserts stylist/client details, and hits submit|"Add a new stylist/client", Description: ""/"", click "Add new sylist/client" button|

## Setup/Installation Requirements

_In Terminal:_

* Navigate to where you want this application to be saved, i.e.:
```cd desktop```
* Clone the file from GitHub with HTTPS
```git clone https://github.com/dzhambov/HairSalon.git```
* Open file in your preferred text editor
* On Mac: ```open -a {your text editor} HairSalon.Solution```
* On Windows: ```HairSalon.Solution```

_Download Manually:_

* Navigate to https://github.com/dzhambov/HairSalon.Solution
* Click the green "Clone or Download" button.
* Click "Download ZIP".
* Click downloaded file to unzip.
* Open folder called "HairSalon.Solution".

Installing MySQL | MacOS
* Download the MySQL Community Server DMG File from [MySQL Community Server](https://dev.mysql.com/downloads/file/?id=484914)
* You can exit the mysql program by entering ```exit```.
* Download the MySQL Workbench DMG File from [MySQL Workbench](https://dev.mysql.com/downloads/file/?id=484391). (Use the No thanks, just start my download link.)
* Install MySQL Workbench to Applications folder.
* Open MySQL Workbench and select the ```Local instance 3306 server```. You will need to enter the password you set. (We used ```epicodus```.) If it connects, you're all set.

 Installing MySQL | Windows 10
* Download the MySQL Web Installer from [MySQL Downloads](https://dev.mysql.com/downloads/file/?id=484919) (Use the No thanks, just start my download link.)
* You can exit the mysql program by entering ```exit```
* Add the MySQL environment variable to the System PATH. We must include MySQL in the System Environment Path Variable. This is its own multi-step process. Instructions here are for Windows 10:
  1. Open the Control Panel and visit System > Advanced System Settings > Environment Variables...
  2. Then select PATH..., click Edit..., then Add.
  3. Add the exact location of your MySQL installation, and click OK. (This location is likely ```C:\Program Files\MySQL\MySQL Server 8.0\bin```, but may differ depending on your specific installation.)
* Open MySQL Workbench and select the ```Local instance 3306``` server (it may have a different name). You will need to enter the password you set (We used ```epicodus```). If it connects, you're all set.
 
 MySQL Workbench Database Setup
  > CREATE DATABASE `hristo_dzhambov`;

  > USE `hristo_dzhambov`;
  
  > CREATE TABLE `stylists` (`StylistId` INT PRIMARY KEY NOT NULL AUTO_INCREMENT, `Name` VARCHAR(255) NULL, `Description` VARCHAR(255) NULL);

  > CREATE TABLE `clients` (`ClientId` INT PRIMARY KEY NOT NULL AUTO_INCREMENT, `Name` VARCHAR(255) NULL, `Description` VARCHAR(255) NULL, `StylistId` INT DEFAULT "0");

_Note For Editors:_ 
* Download the .NET Core SDK [Software Development Kit](https://dotnet.microsoft.com/download)
* Open the .Net Core SDK file and install
* To confirm installation was successful, run the ```$ dotnet --version``` command in your terminal
* Install dotnet script, run the ```$ dotnet tool install -g dotnet-script``` command in your terminal
* Restart your terminal to complete installation, and run the ```$ dotnet run``` command to run application within your terminal - Note: To exit, simply press ```Ctrl + C```
* Open project's productions directory within your terminal ```$ cd HairSalon.Solution/HairSalon```
* Run the command ```> dotnet restore```
* Run the command ```> dotnet build``` 
* If build is successful, run the command ```> dotnet run```, if build failed, make necessary updates and repeat ```> dotnet restore``` followed by ```> dotnet build```

## Known Bugs

_No known bugs at this time._

## Support and contact details

_Have a bug or an issue with this application? [Open a new issue](https://github.com/dzhambov/HairSalon/issues) here on GitHub._

## Technologies Used

* _Git 2.23.0_
* _C# language_
* _.NET Core 2.2.106_
* _dotnet script 0.50.1_
* _VS Code 1.43.1_
* _Model-View-Controller(MVC) framework_
* _Creat, Read, Update, Delete(CRUD) functionality_
* _MySQL 8.0.19_
* _MySQL Workbench 8.0.19_
* _Entity Framework Core 2.2.4_
* _Language-Integrated Query(LINQ)_
* _ASP.NET Razor_

### License

*This webpage is licensed under the MIT license.*

Copyright &copy; 2020 **_Hristo Dzhambov_**