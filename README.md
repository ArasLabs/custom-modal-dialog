# Custom Modal Dialog Sample

The Custom Modal Dialog project contains an import package that provides sample code for calling a custom Aras form in a modal dialog. The sample code also shows how data can be passed from the custom form back to the calling method.

## Project Details

**Built Using:** Aras 11.0 SP7
**Browsers Tested:** Internet Explorer 11

## Installation

#### Important!
**Always back up your code tree and database before applying an import package or code tree patch!**

### Pre-requisites

1. Aras Innovator installed (version 11.0 SPx preferred)
2. Aras Package Import tool
3. Custom Modal Dialog import package

### Install Steps

1. Backup your database and store the BAK file in a safe place.
2. Open up the Aras Package Import tool.
3. Enter your login credentials and click **Login**
  * _Note: You must login as root for the package import to succeed!_
4. Enter the package name in the TargetRelease field.
  * Optional: Enter a description in the Description field.
5. Enter the path to your local `..\CustomModalDialog\Import\imports.mf` file in the Manifest File field.
6. Select **aras.labs.CustomModalDialog** in the Available for Import field.
7. Select Type = **Merge** and Mode = **Thorough Mode**.
8. Click **Import** in the top left corner.
9. Close the Aras Package Import tool.

You are now ready to login to Aras and try out a custom modal dialog.

## Usage

1. Login to Aras.
2. Navigate to **Design > Parts** in the table of contents (TOC).
3. Right click on a Part item in the main grid and select **Open Custom Modal Dialog**.
4. Enter some text into the Parameter 1 field.
  * Optional: Select the Parameter 2 checkbox.
5. Click **Submit**.

The modal dialog will close and an alert will appear, showing the values of param1 and param2 that were returned by the modal dialog.

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## License
