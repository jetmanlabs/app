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
  - [Import From Postman Collection](#import-from-postman-collection)
  - [Import Postman Workspace](#import-postman-workspace)
  - [Import Existing Jetman Backup(Project/Suites)](#import-existing-jetman-backup)
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

## Download Jetman App

![Microsoft logo](https://jetmanlabs.com/docs/media/ss/window.png)

[Windows Installer](https://github.com/jetmanlabs/app/releases/download/v23.4.25/jetman-Setup-23.4.25.exe)

![Apple logo](https://jetmanlabs.com/docs/media/ss/mac.png)

[MacOS Installer](https://github.com/jetmanlabs/app/releases/download/v23.4.25/jetman-23.4.25.dmg)

## Send First Request

As you open app, Jetman app creates default project. you can check path from setting icon in bottom right footer.
If you want to create a create a new project with user defined path in your local filesystem to save your suites and requests, refer [Create Project](#create-project).

To send First request

- Select Http method from 'GET' method dropdown.
- Enter request url in 'Enter Request url here' text bar.
- Add headers,auth,body as needed.
- Click on Send button on the right (green color)
- Response will be displayed in right panel and response time and status code on right top side.

Click image below to watch video [click to play]

[![jetman_send_first_request](https://user-images.githubusercontent.com/48234672/165219970-f90896fd-717c-4190-a0f5-cdfa304da408.png)](https://user-images.githubusercontent.com/48234672/165217879-922f4d0c-28ff-45c0-8acd-f875d134a882.mp4)

# Create Project

Jetman app saves all project suites and request data to user defined local filesystem and users can use github to collaborate with ther developers within their organizations. This way user credentials are safe within their premises without worrying about security and their API data on third party cloud providers. This makes Jetman unique and provides users a secure API deevlopment environment and saves all data in your premises.

- Open Jetman app and click on **+New** button (green button on top left)
- Enter the project name and select where to create/save that project in your system.
- After click on "create" button the project will created. Now yo can create suites and requests to save in this project.

Note: As a next step, to save a request, you need to create suite first.

Click image below to watch video [click to play]

[![jetman_create_new_project](https://user-images.githubusercontent.com/48234672/165220954-ad3f75c8-5a38-4f28-8095-450f805f809f.png)](https://user-images.githubusercontent.com/83591484/164969326-b6956d72-bd60-4a33-8c72-b17a24c39df5.mp4)

# Import Project

Jetman allows you to import Jetman projects/suites or Postman WS or collections.

### Import From Postman Collection

- Open Jetman app and click on **Import** Tab (on top left)
- Click on **Postman backup** from left menu.
- Choose file of postman Collection which you want to import. (zip, json)
- After click import button your Postman Collection import should be success.

Click image below to watch video [click to play]

[![Import_postman_WS_collection](https://user-images.githubusercontent.com/48234672/165239787-7e110cdb-e8dd-40ab-8123-85cc4f7e9b06.png)](https://user-images.githubusercontent.com/83591484/164969326-b6956d72-bd60-4a33-8c72-b17a24c39df5.mp4)

### Import Postman Workspace

- Open Jetman app and click on **Import** Tab (on top left)
- Click on **Postman backup** from left menu.
- Choose file of Postman Workspace backup which you want to import. (zip, json)
- For Postman WS file, you will notice new fields to enter new project name and directory path where you want to Import Postman WS in your local system.
- After click import button your Postman Collection import should be success.

Click image below to watch video [click to play]

[![postman_ws_import](https://user-images.githubusercontent.com/48234672/165240287-0f461420-e44a-4076-b317-4389b564ef8c.png)](https://user-images.githubusercontent.com/83591484/164969326-b6956d72-bd60-4a33-8c72-b17a24c39df5.mp4)

### Import Existing Jetman Backup

User can Import shared or existing Jetman project export file (json), exported suite (json) or any cloned Jetman git repo or similar as directory, this option is popular if user use github to save API project to collaborated with other engineer within the organizations.


- Open Jetman app and click on **Import** button (on top left)
- Click on **Jetman backup** from left menu.
- There are two options:
   - Backup button (green button). Select this if importing an Jetman json backup file.
   - Directory button (Blue button). Select if importing from Jetman backup directory. Mostly used if Jetman project is git cloned as directory in your local filesystem. 
- For backup file import, you will be asked for new project name and location to save project data. If importing suites json file, it will be imported in current project.
- After click import button your Jetman backup/directory should be imported with success.

Click image below to watch video [click to play]
[![jetman_backup_import](https://user-images.githubusercontent.com/48234672/165242151-0f6478a5-3ccc-48f6-97cb-476532fd3d85.png)](
https://user-images.githubusercontent.com/83591484/164969326-b6956d72-bd60-4a33-8c72-b17a24c39df5.mp4)



