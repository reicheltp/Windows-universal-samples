<!---
  category: IdentitySecurityAndEncryption
  samplefwlink: http://go.microsoft.com/fwlink/p/?LinkId=620031&clcid=0x409
--->

# Enterprise data protection sample

This sample demonstrates Enterprise Data Protection (EDP) scenarios: File and buffer protection, clipboard protection,
data protection under lock, and protected access to network resources.
All APIs except File and Buffer protection APIs require Enterprise data policy to be set for a specific identity.

If you have EDP policy set for a specific identity, you should expect the IsIdentityManaged API to return true. If the API returns false, all APIs except the File and Buffer APIs will not work as expected. Each API has a detailed scenario description that describes the purpose and behavior of the API.

You need to add a [special-use capability](https://msdn.microsoft.com/en-us/library/windows/apps/hh464936.aspx#special_capabilities)
capability called EnterpriseDataPolicy into your application manifest file to mark your app enlightened.
This sample will not pass WACK because it uses a special-use capability.

## Related Topics

[Enterprise Data Protection Overview](https://msdn.microsoft.com/en-us/library/Dn985838(v=VS.85).aspx)

## System requirements

Windows 10

## Build the sample

1. If you download the samples ZIP, be sure to unzip the entire archive, not just the folder with the sample you want to build. 
2. Start Microsoft Visual Studio 2015 and select **File** \> **Open** \> **Project/Solution**.
3. Starting in the folder where you unzipped the samples, go to the Samples subfolder, then the subfolder for this specific sample, then the subfolder for your preferred language (C++, C#, or JavaScript). Double-click the Visual Studio 2015 Solution (.sln) file.
4. Press Ctrl+Shift+B, or select **Build** \> **Build Solution**.

## Run the sample

The next steps depend on whether you just want to deploy the sample or you want to both deploy and run it.

## Deploying the sample

1.  Select **Build** \> **Deploy Solution**.

## Deploying and running the sample

1.  To debug the sample and then run it, press F5 or select **Debug** \> **Start Debugging**. To run the sample without debugging, press Ctrl+F5 or select**Debug** \> **Start Without Debugging**.

