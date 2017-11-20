---
title: Lab  - Exposing IIB Through API Connect
toc: false
sidebar: labs_sidebar
folder: labs/iib
permalink: /iib_overview.html
applies_to: [consumer]
---

## Lecture PDF

 <iframe style="overflow:hidden;height:500;width:100%" height="500" width="100%" src="/assets/lectures/Lecture-IIB-Slides.pdf"> </iframe>



## Objective

In this lab, you will get some experience working with IIB.  Although there are many different potential exciting integrations we can make with this software, we will be focusing on the use case to generate REST APIs that we will consume through API Connect. 

 
## Assignment

Please follow the two guides below to complete the lab.  The first will go over creating a sample IIB Flow and the second will walk through how to expose that through API Connect. 

## Generating REST APIs

 Let's walk through the process of using IIB V10 to create a REST API using the Loopback Request Node. 

1. Start by opening the IIB application.  It should open the Quickstart Tutorials.  Let's start a REST API definition.

    ![](./images/captures/iib-1-quickstart.png)

1. Enter a name for this API.  This will also be used to fill in the base path. 

    ![](./images/captures/iib-2-quickmenu-2.png)

1. After this you will have an interface to build your API endpoints.

    ![](./images/captures/iib-3-buildapi-2.png)

1. Enter a model which refers to the format of the returning object. 

    ![](./images/captures/iib-4-model.png)

1. Create a path and attach the model to the return object. 

    ![](./images/captures/iib-5-resourcepath-2.png)

1. Click this icon to now make a flow to process what it should do when this endpoint is requested. 

    ![](./images/captures/iib-6-createflow-2.png)

1. Collapse the Loopback Panel and drag the Loopback Request onto the pallette.  Connect the input and output as shown. 

    ![](./images/captures/iib-7-dragloopback.png)

1. Double click the Loopback Request icon and you will get a Property window to enter the details. Fill in the information as shown.

    ![](./images/captures/iib-8-loopbackdetails.png)

1. We entered the details, but we need to import some information so IIB will know how to execute the connector and model.  We need to copy the datasources.json and model from our existing Loopback Project. Find the IIB config folder and mimic this format. 

    ![](./images/captures/iib-9-datasources-2.png)

1. Now let's go back to the project and we need to deploy the application before it's available.  Right click on the project name and hit Deploy. 

    ![](./images/captures/iib-10-deploy.png)

1. Confirm that we want to publish this application to the Integration Node. 

    ![](./images/captures/iib-10-deployit-2.png)

1. In order to check the status of the Integration Node, let's deploy the web interface.  The panel is in the lower left corner. 

    ![](./images/captures/iib-deploywebserver.png)

1. Collapse the server node and view the REST APIs.  View the Deployment URL.  Click the link and let's add the path to confirm the results. 

    ![](./images/captures/iib-13-testinbrowser02.png)

That's it, now you are ready to go to IBM Cloud and setup the Secure Gateway to connect to this service we just created. 


## Connecting IIB to API Connect

+ [Pushing REST APIs to IBM API Connect provisioned on Bluemix and accessing them through a Secure Gateway service](https://developer.ibm.com/integration/blog/2016/06/06/pushing-rest-apis-to-ibm-api-connect-provisioned-on-bluemix-and-accessing-them-through-a-secure-gateway-service/){:target="_blank"}


## Continue

Leverage this lab to create more exciting connections in the future. 
