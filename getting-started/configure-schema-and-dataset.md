# Setup Schemas & Datasets

To standardize data collection and interoperability, Adobe has created the open and publicly documented Experience Data Model standard, or [XDM](https://experienceleague.adobe.com/docs/experience-platform/xdm/home.html). XDM is the foundational framework that allows [Platform](https://experienceleague.adobe.com/docs/experience-platform/landing/home.html) services and Adobe Experience Cloud solutions, to deliver the right experiences to the right person, on the right channel and at the right time.

{% hint style="info" %}
To learn more about XDM, see [XDM System Overview](https://experienceleague.adobe.com/docs/experience-platform/xdm/home.html)
{% endhint %}

To begin sending XDM data from your mobile application to Adobe Experience Platform, you'll need to do the following:

1. Create & configure your XDM schema\(s\)
2. Create & configure Dataset based on the previously created schema\(s\)

## Create & Configure your XDM Schema

Customers and organizations can configure XDM data schemas to organize and describe data that will be ingested into the Adobe Experience Platform.

{% hint style="info" %}
To learn more about XDM schema creation see [Basics of schema composition](https://experienceleague.adobe.com/docs/experience-platform/xdm/schema/composition.html).
{% endhint %}

To create a basic XDM schema for mobile data collection, follow the steps below to get started:

1. In the browser, navigate to [Adobe Experience Platform](https://experience.adobe.com/platform) and login with your credentials.
2. Create an XDM Schema as follows:
   1. From the left panel, select Schemas
   2. Click **Create schema**
   3. Select **XDM Experience event**
   4. Under **Mixins**, select **Add**; search and add the `Environment Details`,`Application Details`, and other pre-created or custom _mixins_ as needed.
   5. Set a **Display Name** for this schema and click `Save`.

![Schema Creation in Adobe Experience Platform](../.gitbook/assets/AEP_Edge_CreateXDMSchema.png)

## Create & Configure a Dataset

All data ingested into Adobe Experience Platform are stored \(in the Data Lake\) as Datasets that conform to a defined XDM schema\(s\) \(setup in the step above\).

{% hint style="info" %}
To learn more about datasets in Adobe Experience Platform, visit [Datasets overview](https://experienceleague.adobe.com/docs/experience-platform/catalog/datasets/overview.html).
{% endhint %}

To create a Dataset for mobile data collection, follow the steps below to get started:

1. In the browser, navigate to [Adobe Experience Platform](https://experience.adobe.com/platform) and login with your credentials.
2. Create a new Dataset as follows:
   1. From the left navigation panel, under **Data Management**, select **Datasets**
   2. Click **Create dataset from schema**
   3. Select the XDM schema previously created and click **Next**.
   4. Set a name for this Dataset and click **Finish**.

![Dataset Creation in Adobe Experience Platform](../.gitbook/assets/AEP_Edge_CreateDatasetfromSchema.png)
