# _Hair Salon_

#### _Business app for tracking stylists and clients_, _March 20, 2020_

#### By _**Joseph Wangemann**_

## Description

This project creates an application for tracking stylists at the salon and their associated clients . 

## Project Specifications

| Behavior | Input | Output |
|---|:---:|:---:|
| Allow user to create a stylist | Example: Click add stylist, fill out form  | Output: Name of stylist shown on stylist list page |
| Allow user to create a client | Example: Click add client from stylist detail page, fill out form  | Output: Name of client shown on stylist detail page |
| Allow user to delete | Example: Click delete for stylist or client, submit confirmation  | Output: Name of stylist or client is removed from list |
| Allow user to edit | Example: Click edit for stylist or client, submit form  | Output: Changes are shown on detail page |



## Setup/Installation Requirements
_Make sure you have these tools installed on your computer:_
*  [Git version control](https://git-scm.com/downloads)
*  [MySql](https://azure.microsoft.com/en-us/free/mysql/)
*  [Microsoft .Net Core 2.2](https://docs.microsoft.com/en-us/dotnet/framework/install/)
*  [.Net Script](https://dotnet.microsoft.com/download/dotnet-core/2.2)


_In Terminal:_


* Using your terminal navigate to where you want to save this project by typing:
```sh
cd desktop
```

* Clone the file from GitHub by typing:
```sh
git clone  https://github.com/fractalscape13/HairSalon
```

* Navigate to the project folder by typing:
```sh
cd HairSalon.Solution/HairSalon
```
* Restore the project with this terminal command:
```sh
dotnet restore
```

* Open up MySql in your terminal with this command:
```sh
mysql -uroot -p{your password}
```

* Create a new table by typing:
```sh
CREATE DATABASE joseph_wangemann;
```

* Open your new database by typing:
```sh
USE joseph_wangemann;
```

* Create Cuisine table by typing:
```sh
CREATE TABLE stylists (StylistId serial PRIMARY KEY, Name VARCHAR (255), Phone VARCHAR (255), Hours VARCHAR (255), KeyWords TEXT);
```

* Create Restaurants table by typing:
```sh
CREATE TABLE clients (ClientId serial PRIMARY KEY, Name VARCHAR (255), Phone VARCHAR (255), StylistId INT);
```

* Now exit MySql by typing:
```sh
exit;
```

* Then start the webserver by typing:
```sh
dotnet run
```

* Open your web browser and navigate to localhost:5000
```sh
http://localhost:5000/
```

* If your setup worked you should see a welcome page with a rainbow background. 

**Note: To exit, simply press**
```sh
Ctrl + C
```

## Known Bugs

_Updating a client currently deletes the client._

## Support and contact details

If you have any comments or questions, please submit a pull request on my repository. 

## Technologies Used
* [_Git_](https://git-scm.com/downloads)
* [_C#_](https://docs.microsoft.com/en-us/dotnet/csharp/)
* [_.NET Core 2.2_](https://docs.microsoft.com/en-us/dotnet/framework/install/)
* [_dotnet script_](https://github.com/filipw/dotnet-script)
* [_Asp.Net Core 2.2 MVC_](https://docs.microsoft.com/en-us/aspnet/core/tutorials/first-mvc-app/start-mvc?view=aspnetcore-3.1&tabs=visual-studio)
* [_Visual Studio Code_](https://code.visualstudio.com/)
* [MySQL 8.0.15](https://downloads.mysql.com/archives/community/)
* [MySQL Workbench 8.0.15](https://downloads.mysql.com/archives/workbench/)
* [Entity Core framework](https://docs.microsoft.com/en-us/ef/)
* [LINQ](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/linq/)

### License

*This webpage is licensed under the MIT license.*

Copyright (c) 2020 **_JW_**