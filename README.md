# Custom-File-Upload

## Purpose:
HTML provides an easy input button to load file in web server via scripting language. 
But once file is uploaded, and user want to see the file at same time or later, there is no standard free library available. 
This small script helps to make file upload handy to use.

It Provides custom file upload button for html page to capture file and display a preview in a modal.It also supports multiple 
input file button on single page.

## Requirement :
### 1. JQuery
### 2. Bootstrap
### 3. Support - scripting language (php)

## Process:
### 1. Download custom-file-upload.js &  add to your page.

### 2. modify your input statement
input type = "file" class="form-control custom-file-upload" filetype = "pdf" defaultValue = "path of src file" 

Only changes are :
#### 2.1 Add class custom-file-upload
It calls javascript on specific input element type

#### 2.2 filetype = "type of file you are uploading example: pdf, txt " 
You can remove this feature from js. It restrict to pick up other type of files here.

#### 2.3 deafultvalue = "put path of your file stored in web server". 
You can use php & mysql to echo stored file path from db. If this element value is empty, it will work as normal file upload button.
Otherwise it will capture file from this path & show in modal.

## Background

### Script capture path from defaultValue attribute at input div. If it is empty then , normal file upload overrides. After file upload creates 2 button (Preview & Remove) to preview & remove uploaded file respectively.

### If there is a path of exisitng file available at defVal element, it converts the input type to text & update name of file in value field. Creates 2 button (Preview & Change) to view & change respectively.

# Voila ! Thats done!

Enjoy & feel free to customize.

 

