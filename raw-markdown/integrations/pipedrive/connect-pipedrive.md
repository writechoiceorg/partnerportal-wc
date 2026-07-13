---
title: "How to connect to Pipedrive"
description: "This article will walk you through the steps to connect your Pipedrive CRM to your portal."
---

Integrating Pipedrive with your portal allows you to sync deals, track pipeline updates, and give your partners visibility into the sales cycle. Follow the steps below to get connected.

# **Step 1: Initial Connection**

1. Navigate to the **Integrations** tab in your sidebar.

2. Click the **Enable Pipedrive** button.

3. You will be redirected to Pipedrive. If you aren't already logged in, enter your credentials. If you are logged in, simply confirm the connection to link your account.

#### Once your accounts are connected:

1. Click on the **Settings** option for Pipedrive.

2. Finally, click the **Configure** button to begin mapping your data.

---

# **Step 2: Mapping the Integration**

Mapping tells the portal how to translate your Pipedrive data into the portal's structure.

## **Select a Pipeline**

1. Locate the Deal object **Pipeline** card.

2. Click on the card to open it.

3. Click on the **Value** dropdown menu and select the specific Pipedrive pipeline you want to sync with your portal.

![](https://downloads.intercomcdn.com/i/o/j01nt7mc/2148612167/f44c985be0478feafcf73be27b14/Screenshot+2026-03-10+at+12_37_28%E2%80%AFPM+%282%29.png?expires=1778100300&amp;signature=819b7e29b16c52c5f20d35a3647139f25b66385e55b18082cb184365bf9b9aa7&amp;req=diEjHs9%2Fn4BZXvMW1HO4zQ45kDxGsCuG8Eq8O9xNhI6PzV2DOHKSWa0RWqMd%0ApNjSIOa5tYmp%2BY5vQ5Y%3D%0A)

### **Map Stages**

To ensure deals move through the correct phases, you need to map your Pipedrive stages.

- Click on the **Stage** card.

- Click the **Map values** button.

![](https://downloads.intercomcdn.com/i/o/j01nt7mc/2148620305/21b987494670a7b80f23ac72c365/Screenshot+2026-03-10+at+3_03_10%E2%80%AFPM+%282%29.png?expires=1778100300&amp;signature=941897260e7a7fd5f5fdd7c3356164f1cadbbccc94794411e4ab6c3efeb3c648&amp;req=diEjHs98nYJfXPMW1HO4zbp2%2BNH7etHaza3XtUj8zrCVxH%2F2cvyA3oZSYSb9%0AsEzRg1qI%2F6tlPytxT88%3D%0A)

### Choose your mapping method

In **On Create, set Pipedrive CRM Stage to**, choose how new deals created from Portal should enter your Zoho CRM pipeline.

You can either assign every new deal to the same Pipedrive stage, or use your existing mappings to determine the starting stage automatically.

![](https://downloads.intercomcdn.com/i/o/j01nt7mc/2148633623/438cebbd982b3835e2399a6a9168/Screenshot+2026-03-10+at+3_06_38%E2%80%AFPM+%282%29.png?expires=1778100300&amp;signature=16842944d0b1d974663e8c0e711fca815df1e653b58757bf6d931b701bb25529&amp;req=diEjHs99noddWvMW1HO4zZoibX1clxZvxyANB5YSe9ELCCMlMMITznXP787B%0Ap9dWN9oiwUe4FGDhC8Q%3D%0A)

- #### Static stage
  - Select a stage from the dropdown if you want all new deals to begin in the same Zoho CRM stage.

    - For example, if you choose **Qualification**, every new deal created from Portal will enter Zoho in **Qualification**, regardless of the Portal phase it came from.

- #### Infer from mappings
  - Select **Infer from mappings** if you want Portal to determine the starting Zoho stage based on your existing phase mappings.

    - Portal will use your configured Portal-to-Zoho stage mappings to determine the initial stage in your CRM.

      - ***Note:*** *When using this option, avoid mapping multiple Portal phases to the same Zoho stage. If multiple phases point to one Zoho stage, the starting stage for new deals may become inconsistent.*

- #### Map manually
  - Select **Map manually** if you want full control over how Portal phases map to Zoho stages.

  - This allows you to define exactly which Zoho stage should be used for each Portal phase.

**NOTE**: You **do not** need to map every stage. We recommend mapping the key stages you want your partner to be able to follow as a deal progresses through the sales cycle.

**Important:** The **Won** and **Lost** stages must be mapped for the integration to function correctly.

## Map Multiple Pipelines (Optional)

If you'd like to sync to more than one pipeline, you’ll also need to map the stages for each additional pipeline.

To do this:

1. In the **Stage mapping window**, locate the **pipeline selector on the left side**.

2. Select the pipeline you want to configure.

  1. ![](https://downloads.intercomcdn.com/i/o/j01nt7mc/2227665841/b09a202fd8084f8054cdc10d9325/Screenshot%2B2026-03-10%2Bat%2B3_13_33-E2-80-AFPM%2B-282-29.png?expires=1778100300&amp;signature=4f34496c6ac76a83eebbd5595fa207fdb7f1003e841d1bb9ba9a85f6ca56d192&amp;req=diIlEc94mIlbWPMW1HO4zcPRhyzJZzRUvrHx2E00bmdhF76s27YeomZZPl7H%0Am%2F5o%0A)

3. Map the **Pipedrive stages** to the corresponding **portal phases**, just as you did for the first pipeline.

  1. [Learn how to customize your led phases ->](https://help.partnerportal.io/en/articles/8065753-how-to-customize-lead-phases-and-deal-stages)

4. Repeat this process for each pipeline you’ve included in the integration.

Once you have finished mapping your stages, click the **Save** button on the Stage card.

## **Step 3: Finalize**

After configuring your pipeline and stages, look for the **Save mappings** button at the bottom of the page (on the main configuration area).

Your Pipedrive integration is now complete! Deals should begin syncing according to the rules you have set.
