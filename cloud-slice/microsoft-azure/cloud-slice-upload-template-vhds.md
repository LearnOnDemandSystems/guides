# Cloud Slice Guide - Upload to Microsoft Azure

[Return to the Cloud Slice guide][back]

This document describes how to upload template virtual hard disks (VHDs) into a Microsoft Azure subscription.

## Uploading template VHDs into a Microsoft Azure subscription

Template VHDs are used as part of the deployment of managed virtual machines in a Cloud Slice lab. You only need to upload your template VHDs into one Microsoft Azure subscription per Cloud Subscription Pool. This subscription is referred to as the master subscription in OneLearn Lab on Demand, and it must be the first subscription that is added to a subscription pool.

There are multiple supported methods that can be used to upload template VHDs into a Microsoft Azure subscription, but the primary methods are using the  <a href="https://portal.azure.com/" target="_blank">Microsoft Azure Portal</a>, using the [Microsoft Azure Storage Explorer](https://go.microsoft.com/fwlink/?LinkId=708343), using Microsoft PowerShell, or using some combination of the three. In this document we will focus on uploading template VHDs using the Microsoft Azure Portal. To upload template VHDs into a Microsoft Azure subscription using the Microsoft Azure Portal, you must perform the following tasks:

1. [Create a resource group where you will store template VHDs][create-resource-group].
2. [Create a storage account inside of your resource group where template VHDs will be stored in a storage blob][create-storage-account].
3. [Create a container inside of the blob service in your storage group][create-container].
4. [Upload each template VHD you want available to your Cloud Slice labs][upload-vhds].

[create-resource-group]: #create-a-resource-group-where-you-will-store-template-vhds "Create a new resource group in Microsoft Azure"
[create-storage-account]: #create-a-storage-account-inside-the-new-resource-group "Create new storage account inside of your new resource group"
[create-container]: #create-a-container-inside-of-the-blob-service-in-your-storage-account "Create a new container in the blog service in your new storage account"
[upload-vhds]: #upload-each-template-vhd-you-want-available-to-your-cloud-slice-labs "Upload one or more template VHDs into the Microsoft Azure subscription blob service container you created"

### Create a resource group where you will store template VHDs

To create a resource group in a Microsoft Azure subscription, open the <a href="https://portal.azure.com/" target="_blank">Microsoft Azure Portal</a>, browse into the **Resource Groups** service, and click on **Add**. 

[Back to top][back-to-top]

### Create a storage account inside the new resource group



[Back to top][back-to-top]

### Create a container inside of the blob service in your storage account

Once you have created a resource group and a storage account within it, you need to create a container inside of the blob service in your storage account. This can be done from within the <a href="https://portal.azure.com/" target="_blank">Microsoft Azure Portal</a>, by following these steps:

1. TBD

[Back to top][back-to-top]

### Upload each template VHD you want available to your Cloud Slice labs



[Back to top][back-to-top]

## Review Checklist

TBD or remove if not necessary

[Back to top][back-to-top]

[Return to the Cloud Slice guide][back]

[back-to-top]: #cloud-slice-guide---upload-to-microsoft-azure "Return to the top of the document"
[back]: ../cloud-slice.md#upload-template-vhds-into-your-cloud-platform "Return to the Cloud Slice guide"

