
# Data Setup Producer

## Introduction

In this module, you’ll create a data setup for producer to  produce the data and sends Azure Event Hub. Using the provided command-line, you’ll produce the sensor data of Trucks. Lastly, you’ll use the dashboard to plot Trucks on the map and watch their status in real-time. In subsequent modules you’ll add functionality to analyze and persist this data and plot the Line graph dashboard to analyze the various parameter of the Truck in real-time

## Overview

The architecture for this module involves an Event Hub as a producer. Our producer is a sensor attached to a Truck which currently moving on the track. This sensor emits data for every five second including the truck’s current location, Engine Temperature, Engine RPM, Engine Load and Coolant Temperature. Our operations team can monitor these details using the dashboard.


## Implementation

In our previous module we have created Event hub and Cosmos DB. We assume that you have completed the previous module successfully, in this module we are going to FTP the producer script to emits the data on Every Five seconds
  
## 1. Data Setup for Producer

In this step you will download the script files from the link and then you need to do the required configuration to get connect with EventHub. This script files will produce the current location, Engine Temperature, Engine RPM, Engine Load & Coolant Temperature details of the Truck.

<details>
<summary><strong>Step-by-step instructions (expand for details)</strong></summary><p>
 
 1. Click the [link](https://github.com/iyyappan16/Azure_HereMap/blob/master/Data_Setup_Producer/Producer.zip) and download the zip file (Producer.zip) and extract it to your local machine.

	
1. Open Azure Portal home page, by signing in to your registered account

	![HERE Maps & Location Services Data Streams](Producer/1.png)

1. Click on **Cloud shell** to open the Azure PowerShell command-line.

1. Let’s it open the PowerShell command-line it may take few seconds to open up

	![HERE Maps & Location Services Data Streams](Producer/2.png)
	
1. Ensure that the command-line interface indicates its PowerShell, by default it will be in the Azure directory. We need to set location to execute our Producer script. Execute the below command to set location

                >Set-Location $home 
	
		
6. It changes the directory and it set’s the home location of the user profile

	
1. In menu tab click on Upload/Download files icon then click on upload to upload our zip file 

	![HERE Maps & Location Services Data Streams Pricing Page](Producer/3.png)
	
1. Browse to the directory where you saved the Zip file locally which you have downloaded in step-1. Choose the file and Upload.

	![HERE Maps & Location Services Data Streams Pricing Page](Producer/4.png)
	
1. Once the upload is completed successfully. The you need to extract the file, for extracting it  use the below command

	            >Expand-Archive “Producer.zip”
         
        
      ![HERE Maps & Location Services Data Streams Pricing Page](Producer/5.png)
  
1. It may take few seconds to extract, after successful extraction you can verify the file by using the below command. 

              >ls
              
1. It lists the directories available in the current directory. so, you can find the unzipped/ extracted **Producer** folder. 
  
</p></details>










