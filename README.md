# HERE Maps & Location Services Data Streams On Azure Workshop

This document introduces the deployment steps for HERE Maps & Location Services Data Streams on Azure. This workshop contains four modules.

### Modules

This workshop is divided into four modules. Each module describes a scenario of
what we're going to build and step-by-step directions to help you implement the
architecture and verify your work.

| Module        | Description |
|:---------------|:-------------:|
| [1. ARM Template Deploy][ARM Template Deploy] | The HERE Location Services Data Streams Template is a Solution Template on Azure  |
| [2. Data Setup Producer][Data_Setup_Producer] | Uploading/Transfering the data's to azure  |
| [3. Data Setup WebApp][Data_Setup_WebApp] | Configuring the requied connection strings of EventHub & CosmosDB  |
| [4. Validation][Validation] | Launch the Web App URL via browser to see the dashboard on a real-time map  |




:warning: These modules are intended to be executed linearly.

After you have completed the workshop you can delete all of the resources that were created by following the [cleanup guide][cleanup].




[ARM Template Deploy]:ARM_Template_Deploy/
[Data_Setup_Producer]:Data_Setup_Producer/
[Data_Setup_WebApp]:Data_Setup_WebApp/
[Validation]:Validation/
[cleanup]: 5_CleanUp/
