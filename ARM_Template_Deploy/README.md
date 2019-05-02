# ARM Template Deploy

## Introduction

HERE Maps and Location Services Data Streams Template brings enterprise-grade, SLA backed location services to Azure applications. HERE Maps and location services solve a range of problems from map visualization, navigation and routing, geocoding, time zone look ups to geofencing, custom locations and routing, route matching GPS traces, geospatial, sequencing multiple waypoints, truck routing, positioning, etc.

## Solution Template Overview

HERE Maps & Location Services Data Streams Template deploys HERE's enterprise class SLA backed Maps & Location Services, an EventHub and a CosmosDB for all your Azure Applications.

These services address a range of use cases like Fleet Utilization, Supply Chain Optimization, Urban Movement, etc., and open up new location intelligence opportunities in diverse industries like Automotive, Insurance, Internet and Media, Mobile Payments, Public Sector and Infrastructure, Telecom and Utilities, and Transportation and Logistics.

The function app in this ARM Template consists of the following HERE Location Service APIs:

**Geocoding and Search**

  -	Geocoder: Forward and Reverse
  -	Batch Geocoder
  -	Geocoder Autocomplete
  -	Places
  
**Maps**

  -	Map Image
  -	Map Tile
   
**Navigation and Routing**

  - Routing - Mode (car, truck, public transit, bicycle) and algorithm (matrix, isoline routing)

**Navigation and Routing**

  -	Considering toll costs along a route
  -	Working with geofences
  -	Working with custom locations
  -	Building custom routes
  -	Integrating advanced HERE data sets
  -	Route matching GPS traces
  -	Calculating an optimal sequence of waypoints

**More APIs**

  - Positioning - Provides positioning estimates based on global Wi-Fi and Cell coverage, which includes the latitude and longitude of the position with accuracy.


## Deployment Guide

  1.  Acquiring HERE App ID and HERE App Code
  2.  Deploying Solution Template on Azure Portal
  
## 1. Acquiring HERE App ID and HERE App Code

All users of HERE APIs must obtain authentication and authorization credentials and provide them as values for the parameters HERE App ID and HERE App Code in the HERE Credentials section in Azure’s template deployment page. 

To obtain the credentials for the deployment of HERE Maps & Location Services Data Streams, please visit [here](https://developer.here.com) to register for FREE with HERE.

## 2. Acquiring HERE App ID and HERE App Code

The below steps help you deploy HERE Maps & Locations Services Data Streams Template in your Azure resource group. 

<details>
<summary><strong>Step-by-step instructions (expand for details)</strong></summary><p>
 
 1. Click on **Get it Now** button to start the deployment process.

	![HERE Maps & Location Services for Data Streams in Azure Marketplace](ARM_Deployment/1.png)

1. Read through the Microsoft agreement and click on **Continue** when you are ready.

	![HERE Maps & Location Services Data Streams Pricing Page](ARM_Deployment/2.png)

1. You will be re-directed to template deployment home screen. Click on **Create** button to continue.

	![HERE Maps & Locations Services Data Streams Azure Portal Page](ARM_Deployment/3.png)
	
1. You will now be prompted to provide details specific to deployment. In the **Basics** use any existing resource group you might have or click on **create new** button to create a new resource group. Select your Subscription details and location and click **OK** to continue.

	![Template Deployment Page -  Basic Section](ARM_Deployment/4.png)
	
	
	
	
	![Template Deployment Page – Basic Section – Create new Resource Group](ARM_Deployment/5.png)
	
1. You now need to provide HERE credentials (HERE App ID and HERE App Code) which are pre-requisite to access HERE resources. If you already have HERE credentials available with you, provide the same and click **OK**. If you don’t have HERE credentials, please visit here(https://developer.here.com) to register for FREE with HERE. You also need to select a Storage option, you can either select any existing Storage or continue with a newly created one.

	![Template Deployment Page – HERE Credentials Section](ARM_Deployment/6.png)
	
	
	
	
	
	![Template Deployment Page – Storage Selection](ARM_Deployment/7.png)
	
1. You will see the summary of details, which were provided during the previous steps. Review the values and click **OK** once you are satisfied with all values.

	![Template Deployment Page – Summary Section](ARM_Deployment/8.png)
	
1. Review the master agreement and click the check box at the bottom of agreement. You are now ready for template deployment. Click on **Create** to start template deployment..

	![Template Deployment Page – Create/Buy Section](ARM_Deployment/9.png)
	
1. Deployment should have started, and you will be able to see in the notification tabs deployment in progress. Once deployment is complete, you should receive the notification of the same and be able to see new resources in the resources section of your account.

	![HERE Maps & Location Services Data Streams Template Deployed](ARM_Deployment/10.png)

</p></details>




