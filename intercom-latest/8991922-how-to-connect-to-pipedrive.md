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

![](https://downloads.intercomcdn.com/i/o/j01nt7mc/2380643163/29ad52ae8792edeed9bef4a94a70/image.png?expires=1783016100&amp;signature=d9d8d346290ceba66d2cdf4d7c7081dee452c5f14789e7e05bce6033fe684e8f&amp;req=diMvFs96noBZWvMW1HO4zZTjUKLu0qV6fZ2RPiQ9B9%2BzKSpmP7GU1H8DQyfW%0AottKURsU0rWTiOOmqto%3D%0A)

### **Map Stages**

To ensure deals move through the correct phases, you need to map your Pipedrive stages.

- Click on the **Stage** card.

- Click the **Map values** button.

![](https://downloads.intercomcdn.com/i/o/j01nt7mc/2380644473/696f17dc47bd46d7f54a24cef069/image.png?expires=1783016100&amp;signature=01bafdbf0faaa998ec4dbc6242d412562c9b112dea179947c35d84e00e26840d&amp;req=diMvFs96mYVYWvMW1HO4zdVRucsfci894CHF2JWQIwYWpwnxJ%2F9vn7bq%2BxlL%0AMjmPW0PzavFiT82F8cU%3D%0A)

### Choose your mapping method

In **On Create, set Pipedrive CRM Stage to**, choose how new deals created from Portal should enter your Zoho CRM pipeline.

You can either assign every new deal to the same Pipedrive stage, or use your existing mappings to determine the starting stage automatically.

![](https://downloads.intercomcdn.com/i/o/j01nt7mc/2380660588/52fec191786f29d8d45a258ddd4c/image.png?expires=1783016100&amp;signature=b4a652c394b17615f8fbcf02adafd2434238582b131126e0fccded5a1af40bcc&amp;req=diMvFs94nYRXUfMW1HO4zfIMezSzOTRLbeo0SUUZ6IN%2B0d5kvTEU0Z9GY5Zh%0ArWAZs9f5rzIgLO5vJY8%3D%0A)

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

  1. ![](https://downloads.intercomcdn.com/i/o/j01nt7mc/2380661697/bc61aa885a8f272c77f8b7d2f04f/image.png?expires=1783016100&amp;signature=a89d9901f08702473538a982f48a45d7007fb4434f7b6ed121fda554823458f3&amp;req=diMvFs94nIdWXvMW1HO4zWuZDlYWxGMco3uR4nKeiKQSwOw8SpryVrDbMvaO%0AMbxR%0A)

3. Map the **Pipedrive stages** to the corresponding **portal phases**, just as you did for the first pipeline.

  1. [Learn how to customize your led phases ->](https://help.partnerportal.io/en/articles/8065753-how-to-customize-lead-phases-and-deal-stages)

4. Repeat this process for each pipeline you’ve included in the integration.

Once you have finished mapping your stages, click the **Save** button on the Stage card.

## **Step 3: Finalize**

After configuring your pipeline and stages, look for the **Save mappings** button at the bottom of the page (on the main configuration area).

Your Pipedrive integration is now complete! Deals should begin syncing according to the rules you have set.