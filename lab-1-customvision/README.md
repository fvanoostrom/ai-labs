
# Lab 1 - Classifying images using Azure Custom Vision

## Introduction

This lab covers classifying images. A classification algorithm is able to seperate objects into multiple categories. An algorithm could classify different kind of objects, like numbers, text or even sounds and images. Within this lab we will classify an image into one of three categories of fruit: an apple, orange or banana.

A Classification is a supervised learning problem. This means that we provide a training set with a label for each object. 

## Step 1 - Setting up the Custom Vision environment
Go to [portal.azure.com](https://portal.azure.com) and click on Create Resource.

 ![Azure Portal](./images/Lab01A_azureportal.png)

 Type in the searchbox 'Custom Vision' and hit enter. 
 Select 'Custom Vision' and hit 'create'
 
 ![Azure Portal](./images/Lab01B_create_customvision.png)

Now you are able to configure the resource.
First of all you have to select a subscription and resource group. You can select a resource group you previously created, or create a new one.

For the region select 'West Europe'. For the name follow the naming convention. I named my custom vision 'dv-we-MY_OWN_INITIALS-ailabs'.

Select the Free pricing tiers.

Click Review + create, and if the validation was passed, click 'Create'.


 ![Azure Portal](./images/Lab01C_configure_customvision.png)
 
  It will take a few minutes until the resource is created. After the resource has been created you can click on 'Go to resource group'

 ![Azure Portal](./images/Lab01D_deployment.png)

## Step 2 - Preparing the images
Download the files from [here](files/fruit-images-for-object-detection.zip) (click on the url and hit the download button) or the original [dataset on kaggle](https://www.kaggle.com/mbkinaci/fruit-images-for-object-detection)

Afterwards unzip the images to a location on your device.

## Step 3 - Creating the model in Custom Vision

 The custom vision resource should be created by now. You can click the link to the resource group from step 1. Afterwards click on the name in the resource. From here information is shown that can help you make use of this service. You can either use this service in multiple ways. One way is to use it within your python code in for example databricks or Azure Machine Learning. Another way is to use the portal of Custom Vision. Within this lab we will use the portal. You can access this portal by 
  ![Lab01E_access_CustomVision](./images/Lab01E_access_CustomVision.png)
 
 
 You can also access it directly by going to the [customvision-portal](https://www.customvision.ai/)  and sign in.

## Step 4 - Testing the created model

You can try out a few images yourself to see what custom vision thinks it sees in the image



## Step 5 - Deleting the resources
You can clean up the resources by going to the resource group in portal.azure.com, selecting the created resources and hitting delete.

![Delete resources](./images/Lab01Z_Delete_resources.png)

More information about custom vision can be found here:

https://azure.microsoft.com/en-us/services/cognitive-services/custom-vision-service/#overview

https://docs.microsoft.com/en-us/azure/cognitive-services/Custom-Vision-Service/overview