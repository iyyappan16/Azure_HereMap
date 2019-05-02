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

	![HERE Maps & Location Services for Data Streams in Azure Marketplace](/ARM_Deployment/1.png)

1. Ensure that **Create New Test Event** is selected.

</p></details>

Now choose Kubernetes Service, leave the Dockerfile path with the default value and enter `helm` on the `Path to the Chart folder` textbox.

On the next screen select the appropriate values on:

- Project name: The value of your choice.
- Cluster name: The value of your choice.
- Location: Choose somewhere in Europe (preferably Europe West)

Click on Done.

This is going to create:
- An AKS Cluster
- An Azure Container Registry

The release pipeline will fail but we are going to fix it on the next step.

## Fix Helm Chart path error

By default, Azure DevOps is unable to find out the name of your Chart, on the releases pipeline, update
the value using the explorer to the zip file that the browser shows (helm-0.1.0.zip by default)

## Customize build pipelines to build the three Docker images

Now it is time to adjust the build pipelines to build not one but the three Docker images that the project is composed of.

# Exercises

Now it is time to explore Azure DevOps. Ask as many questions as you need and make sure that you understand what you are doing.

## Customize the release pipeline to use the most recently built images

We have adapted the build pipelines to build and deploy the three images that compose our system into an Azure container registry. Now it is time to customize the release pipeline to use these images instead of the default ones from Docker Hub.


