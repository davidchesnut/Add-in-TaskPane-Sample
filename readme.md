      _____         _      ____                       _       _     _       _
     |_   _|_ _ ___| | __ |  _ \ __ _ _ __   ___     / \   __| | __| |     (_)_ __  
       | |/ _` / __| |/ / | |_) / _` | '_ \ / _ \   / _ \ / _` |/ _` |_____| | '_ \
       | | (_| \__ \   <  |  __/ (_| | | | |  __/  / ___ \ (_| | (_| |_____| | | | |
       |_|\__,_|___/_|\_\ |_|   \__,_|_| |_|\___| /_/   \_\__,_|\__,_|     |_|_| |_|


This sample showcases a simple add-in for Office that lets you get data from a document.

The easiest way to run this sample is to open it in the playground for Office Add-ins: http://aka.ms/Fb7hmn (only works for Excel Online at the moment; if you're using PowerPoint: read on). Click the Run Project icon to launch the sample in Excel Online (you will need to login using a Microsoft account).

====================================================================================

If you're not using the playground for Office Add-ins, follow these steps to run the sample:

If you have Office 2013 or later on Windows:

1. Host these files on a local network share.

2. Open up an Office app (Excel, Word or PowerPoint), open a document, and then select File > Options > Trust Center > Trust Center Settings > Trusted App Catalogs.

3. Type the location of the directory on your local network share into the Catalog Url text field, and click Add Catalog. Make sure the Show in Menu check box is selected.

4. Click OK. Close the Office app and launch it again so the changes take effect.

5. Go to Insert > My Apps > Shared Folder and select My First TaskPane Add-in, and then click Insert. If you don't see the add-in, click Refresh.

6. The add-in TaskPane opens next to your document.

For more information, please read: https://msdn.microsoft.com/EN-US/library/office/fp123503.aspx

====================================================================================

If you are using Office Online:

1. Host these files locally (on localhost) or online (e.g. AWS, Azure, Heroku, etc). In the manifest.xml file, change the DefaultValue of the SourceLocation to point to the URL where the index.html file is hosted.

2. Go to the Office 365 portal (https://portal.office.com) and click on Admin in the app launcher on the top left hand corner.

Note: You need to already have a subscription to Office 365. If you don't have one, obtain a free account for 30 days from https://portal.microsoftonline.com/Signup/MainSignUp.aspx?OfferId=6881A1CB-F4EB-4db3-9F18-388898DAF510&DL=DEVELOPERPACK

3. Select SharePoint > apps > App Catalog > Apps for Office.

4. Select the "+" button to add a new add-in, and choose the manifest.xml file from your local directory. Press OK and the add-in will install.

5. Open the app launcher on the top left hand corner and select an Office app (Excel or Word).

6. When the Office app opens, go to Insert > Apps for Office and select My First Content Add-in under My Organization. If you don't see the add-in, press Refresh. Press Insert and the add-in should appear.

For more information on publishing Office Add-ins, please read: https://msdn.microsoft.com/EN-US/library/office/fp123517.aspx
