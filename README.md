# CKL Advanced Line Recognition #

## Introduction ##
This repository contains an extension for [Continia Document Capture](http://continia.com/documentcapture-for-dynamics-nav.aspx) module, which is a solution for scanning of invoices and other documents directly from Microsoft Dynamics NAV! 

The initial development was done by [CKL Software GmbH (CKL)](https://www.ckl-kore.de "Jump to CKL Website") and the code will be maintained by CKL unregularly based on experiences made in projects. 

**Please note!** 
This is not an official module / add-on and therefor CKL Software does not offer support for implementation, training or is responsible for errors in this module. 
You can use the CKL Advance Line Recognition on your own risk. 

**If you find issues in the code, please report these in the issues list here on Github.**

## Documentation ##
At the moment there is no other documentation than this readme file.

## Implementation of the extension ##
The code will be updated unregularly for new versions of Document Capture.

1. Clone the project / Download all  *.txt files to your client
2. Import all txt files into your database via the development environment 
3. Filter the versionlist for *ALR* and compile all objects

## How to use the extension ##
The concept of the Advanced Line Recognition extension is to identify at least one field per line by Document Capture standard code - we'll call this field "line identification field" (LIF) in this guide.

Based on the position of this field the user will define the "offset" of other fields that he wants to capture. 

![](https://github.com/sradloff/Document-Capture-Advanced-Line-Recognition/blob/master/Documentation/ExampleDocument.png?raw=true)

1. Open Dynamics NAV Client
2. Import open Documents to Document Capture
3. Open the Document Journal
4. Run `Recognize Fields` action from the menu to recognize the fields of the selected document
5. Open the Document Card from the menu
6. Capture the LIF
7. Mark the **values** of the offset fields with left mouse button
8. Link the offset fields to the LIF via line action `Adv. line recognition` ==> `Link to line ident. field`
9. Test your setup by `Recognize Fields`

Still not sure what to do? Watch this click guide:
![](https://github.com/sradloff/Document-Capture-Advanced-Line-Recognition/raw/master/Documentation/UsageOfAdvancedLineRecognition.gif)
