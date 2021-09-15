I did this project during my internship in SmartPulse company. In fact, this is my second project related to React and .Net core. The main reason for me to do this project is to enhance my skills and be more familiar with the idea of using React with .Net Core. 

# Description 
Basically, the project is a web application to track the company’s IoT devices, which are distributed to power plants. The application should link each device with one power plant, in addition to be able to create, read, update, and delete devices. The project is dockerized, which means you can run it without having to install a SQL server if you have docker desktop installed. In addition, I used web socket connections to enable real-time of device related displayed data alongside normal HTTP connections. 

Various packages and libraries were used to Implement this application like:

1. .Net Core API and Console application
	- Entity Framework Core 
	- SignalR
	- MailKit
	- and more ... 
2. React 
	- Material-UI React 
	- Ag-Grid
	- SignalR  
	- and more ... 
3. Database 
	- SQL Server with SQL Server Management Studio
4. Docker
	- Docker with Dockerfile 
	- Docker compose with docker-compose.yml file 


The pictures below try to show you how the application would look like if you run it on your machine. 

# .Net Core API

The API gives the user the ability to access data and manipulate it. 

## Folder Structure 
<img src="Pictures\dotNetCore\FolderStructure.png" width=300> 



# React 

This is the client application where the the frontend is implemented and the user can access the functionality offered by the application. 

## Folder Structure  
<img src="Pictures\React\FolderStructure.png" width=300> 

## Home Page
<img src="Pictures\React\HomePage.png" width=800> 

## Companies Page 
Please note that in this page, data in the grid is updated using a WebSocket with SignalR. This means the update happen in real-time. 

![CompaniesPage](https://raw.githubusercontent.com/Nour0700/SmartPulseStockTracker/main/Pictures/React/CompaniesPage.gif)


## Inventory Page 

###  Inventory Page 
<img src="Pictures\React\Inventory\InventoryPage.png" width=800> 

###  Add Device Type
<img src="Pictures\React\Inventory\AddDeviceType.png" width=800> 

### Add Device 
<img src="Pictures\React\Inventory\AddDevice.png" width=800> 

###  Ag-Grid Company dropdown
<img src="Pictures\React\Inventory\SantralList.png" width=800> 

###  Delete Device
<img src="Pictures\React\Inventory\DeleteDevice.png" width=800> 


# Console App 

This application will work in the background as a windows task to update the state and message of devices as shown in companies' page to imitate a working device in a power plant. 

## Setting up a Windows Task
<img src="Pictures\ConsoleApp\SetUpWindowsTask.png" width=800> 
