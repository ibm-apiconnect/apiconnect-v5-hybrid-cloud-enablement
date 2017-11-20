---
title: Testing Service Through Secure Gateway Client
toc: false
sidebar: labs_sidebar
folder: labs/lab6
permalink: /lab6_testing.html
summary: It is time to test our connection now.  We should see the same results as if we were accessing this service locally. 
applies_to: [developer]
---
 

## Creating an API in DRAFT MODE

1. First we go into the Drafts mode and select the APIs tab. Then click the “Add” link and select “Import an existing OpenAPI” from the drop down.

    ![](./images/captures/cloud-import-api.png)

1. Import the yaml definition for your local loopback inventory app. 

    ![](./images/captures/import-swagger.png)

1. Make sure to add a Product. 

    ![](./images/captures/import-addproduct.png)

1. Set a Catalog for the Product to be Published. 

    ![](./images/captures/import-publishing.png)

1. Ensure that Invoke has the proper URL http://localhost:4001 and check box is checked. 

    ![](./images/captures/verify-sg-cloud-2.png)


## Continue

Proceed to [oAuth & JWT](lab7_overview.html).