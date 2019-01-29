# Adobe-Sign-custom-button

Add custom button in Adobe Sign extension

 
1. Click the Settings Icon(Setup) -> Customization -> Modules -> Select the Module to which the Custom Button have to be create -> Layout -> Links and Buttons -> Create New Button.
2. Give the Name of the Button.
3. Add Description if you want.
4. Select the button to be placed.
5. Select "Invoke a URL" to perform the action.
6. Given the below URL in Construct Your URL :
 
 https://extensions.zoho.com/plugin/esign/handler?action=createAgreement&module=ModuleName&rec_id=${Module.Module_Id}&rec_name=${Module.Module_Name}

For Ex : https://extensions.zoho.com/plugin/esign/handler?action=createAgreement&module=Lead&rec_id=${Lead.Lead_Id}&rec_name=${Lead.Last_Name}
 
7. Select the button on Where to show the content of the button action.
8. Select Which Profiles to show this action.
9. Click Save.


To auto-populate the recipient's email id or name:
1. Create the following fields:
   1.1 Email field - Email Field type
   1.2 Contact Name field - LookUp field type to Contact module
   1.3 Recipient Type field - Pick list type with values Email and Contact Name(the ones created now)
2. Once these fields are created, when you click on the 'Send for Signature' button, you can find the fields you have chosen automatically populated.
3. You can select which field you want to be populated by choosing in the 'Recipient Type' field pick list.
