# How to Use Jetman app
![jetman logo](https://jetmanlabs.com/media/icons/MainPage_jetmanLogo2.png)

* Jetman is an API management platform to allow users to design, develop, test and collaborate with others to accelarate API development. Jetman platform provide secure ecosystem by allowing users to keep all their API data on their local premises and not worry of their data and credentials being shared to any third part cloud provider.
* Jetman saves all data on user premises, and users can use github or similar platform to collaborate within their organizations.


## Jetman Products and Offerings
- Jetman Studio - Manage, Design and develop API's
- Jetman Runner - Run entire project or suites for QA/Testing
- Jetrunner-cli - Run suites in headless mode from CLI for CI integration
- Jetrunner Marketplace - Publish API's to public marketplace for sharing
- Jetrunner Documentation - Generate API documentation from your suites.

## Table of Contents (App and CLI)
- [Getting Started](#getting-started)
- [Create Project](#create-project)
- [Import Project](#import-project)
  - [Import from Postman](#import-from-postman)
  - [Import from Jetman](#import-from-jetman)
- [Manage Suites and Requests](#manage-suites-and-requests)
  - [Create suites and add Requests](#create-suites-and-add-requests)
  - [Modify suites or Requests](#modify-suites-or-requests)
  - [Reorder/Move suites or Requests](#move-suites-or-requests)
- [Response Assertions and Validations](#response-assertions-and-validations)
- [Response Extractor and Run-time Variables](#response-extractor-and-run-time-variables)
  - [Extract and save response fields in runtime-variables](#extract-and-save-response-fields-in-runtime-variables)
  - [How to use runtime-variables in requests](#how-to-use-runtime-variables-in-requests)
  - [Example-Automating Authentication using response extractor](Example-Automating-Authentication-using-response-extractor)
- [Env Variables](#Env-Variables)
  - [Run suites with various env using user defined env](#Run-suites-with-various-env-using-user-defined-env)
- [Switch Projects](#Switch-Projects)
- [Runner Module](#Runner-Module)
  - [How to run all requests using runner](#How-to-run-all-requests-using-runner)
  - [Using Env and Iterations](#Using-Env-and-Iterations)
  - [Understanding Responses and Assertions](#Understanding-Responses-and-Assertions)
- [Share Project/Suites](#Share-Project/Suites)
- [Import and Export from Curl](#Import-and-Export-from-Curl)
  - [Import from Curl](#Import-from-Curl)
  - [Export to Curl](#Export-to-Curl)
- [Publish to Marketplace](#Publish-to-Marketplace)
- [Advance Topics and Debugging](#Advance-Topics-and-Debugging)
  - [Opening Console window](#Opening-Console-window)
  - [Print Response Object in Console](#Print-Response-Object-in-Console)
  - [Select Env and Print Varaibles](#Select-Env-and-Print-Varaibles)
  - [Print Runtime Varaibles](#Print-Runtime-Varaibles)
- [Jetrunner-cli to run suites from CLI](#Jetrunner-cli-to-run-suites-from-CLI)
  - [Installation and Usage](#Installation-and-Usage)
  - [Command Line Options](#Command-Line-Options)
- [Marketplace](#Marketplace)
  - [Publish to Marketplace](#Publish-to-Marketplace)
  - [Import from Marketplace](#Import-from-Marketplace)
  - [Edit Marketplace Published API's](#Edit-Marketplace-Published-API's)
- [FAQ's](#FAQ's)

# Getting Started

[![jetmanlabs video](http://i3.ytimg.com/vi/8pbItxrKSFc/hqdefault.jpg)](https://youtu.be/8pbItxrKSFc)

[Watch the video](https://youtu.be/8pbItxrKSFc)
## Download Jetman App

![Microsoft logo](https://jetmanlabs.com/docs/media/ss/window.png)

[Windows Installer](https://github.com/jetmanlabs/app/releases/download/v23.4.25/jetman-Setup-23.4.25.exe)

![Apple logo](https://jetmanlabs.com/docs/media/ss/mac.png)

[MacOS Installer](https://github.com/jetmanlabs/app/releases/download/v23.4.25/jetman-23.4.25.dmg)

## Send First Request

As you open app, Jetman app creates default project. you can check path from setting icon in bottom right footer.
If you want to create a create a new project with user defined path in your local filesystem to save your suites and requests, refer [Create Project](#create-project).

##### Steps to send your first request
- Select Http method from 'GET' method dropdown.
- Enter request url in 'Enter Request url here' text bar.
- Add headers,auth,body as needed.
- Click on Send button on the right (green color)
- Response will be displayed in right panel and response time and status code on right top side.

watch video

https://user-images.githubusercontent.com/48234672/164884955-2e4efd14-31b8-4538-961b-e70d77d1354d.mp4

# Create Project

Jetman app saves all project suites and request data to user defined local filesystem and users can use github to collaborate with ther developers within their organizations. This way user credentials are safe within their premises without worrying about security and their API data on third party cloud providers. This makes Jetman unique and provides users a secure API deevlopment environment.

#####  Steps create new project with user defined path
- Open Jetman app and click on +New button (green button on top left)
- Enter the project name and select where to create/save that project in your system.
- After click on "create" button the project will created.

watch video

https://user-images.githubusercontent.com/83591484/164969326-b6956d72-bd60-4a33-8c72-b17a24c39df5.mp4

# Import Project

Jetman app provides Import project feature. It also can help to restore the project that was deleted mistakenly or for many purposes. You can import the project with json format.

### Import From Postman

1.Import Postman Collection

#####  Steps Import Postman collection
- Open Jetman app and click on Import button (on top left)
- Click on postman backup from import tab to import postman Collection.
- Choosing file of postman which you want to import.
- After click import button your postman collection successfully imported under you existing jetman project.

watch video

https://user-images.githubusercontent.com/83591484/164969326-b6956d72-bd60-4a33-8c72-b17a24c39df5.mp4

2.Import Postman Workspace

#####  Steps Import Postman Workspace
- Open Jetman app and click on Import button (on top left)
- Click on postman backup from import tab to import postman workspace.
- Choosing file of postman which you want to import which is in Zip format.
- Then enter project name and choose directory where you want to save project in your system.
- After click import button your postman workspace successfully imported.

watch video

https://user-images.githubusercontent.com/83591484/164969326-b6956d72-bd60-4a33-8c72-b17a24c39df5.mp4

### Import From Jetman

1.Import Jetman Backup

#####  Steps Import Jetman Backup
- Open Jetman app and click on Import button (on top left)
- Click on Jetman backup from import tab to import jetman backup.
- There are two buttons shown:
   1.Backup button(which is in green color) use for import jetman backup in json format.  
   2.Directory button(which is in Blue color) use for import jetman backup in directory form.  
- After select button then choose file which you want to import.
- Then enter project name and select target folder where you want to save project in your system.
- Then press import button and your project will successfully imported.

watch video

https://user-images.githubusercontent.com/83591484/164969326-b6956d72-bd60-4a33-8c72-b17a24c39df5.mp4
