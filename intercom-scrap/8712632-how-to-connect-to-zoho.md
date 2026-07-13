Integrating Zoho with your portal allows you to sync deals, track pipeline updates, and give your partners visibility into the sales cycle. Follow the steps below to get connected.

# Step 1: Initial Connection

1. Navigate to the **Integrations** tab in your sidebar.

2. Click the **Enable Zoho** button.

3. You will be redirected to **Zoho**. If you aren't already logged in, enter your credentials. If you are logged in, simply confirm the connection to link your account.

#### Once your accounts are connected:  Click on the **Settings** option for **Zoho**.

Finally, click the **Configure** button to begin mapping your data.

---

# Step 2: Mapping the Integration

Mapping tells the portal how to translate your **Zoho** data into the portal's structure.

## Select a Pipeline

- Locate the **Deal object Pipeline** card.

- Click on the card to open it.

- Click on the **Value** dropdown menu and select the specific **Zoho** pipeline you want to sync with your portal.

![](https://downloads.intercomcdn.com/i/o/j01nt7mc/2227646698/3e0ec3e80ed3e01711d0f02fa6f1/Screenshot+2026-04-01+at+3_37_30%E2%80%AFPM.png?expires=1783016100&amp;signature=1d1e9aaaa32a0f90bb298eeb5c8cdb61761a427ad52fff87bc54badcedd1cdcf&amp;req=diIlEc96m4dWUfMW1HO4zQmaHuxClFDftGDyJpUTA9GIf6YRUbDnZjCi3llp%0AOqowsIhljKYtBH9OQrY%3D%0A)

### Map Stages

To ensure deals move through the correct phases, you need to map your **Zoho** stages.

- Click on the **Stage** card.

- Click the **Map values** button.

![](https://downloads.intercomcdn.com/i/o/j01nt7mc/2227649885/bcf77e5794e86c9e708f14f78eca/Screenshot+2026-04-01+at+3_37_53%E2%80%AFPM.png?expires=1783016100&amp;signature=339774c139f4565678b7cc582aee87ccdfefd4e505eb85ed5fe7636095307255&amp;req=diIlEc96lIlXXPMW1HO4zUK9tLbp681r9WZOwIVH22goT8EV9jGIubb2W9xS%0A4Wt7s403wvP1nQMwg1o%3D%0A)

### Choose your mapping method

In **On Create, set Zoho CRM Stage to**, choose how new deals created from Portal should enter your Zoho CRM pipeline.

You can either assign every new deal to the same Zoho stage, or use your existing mappings to determine the starting stage automatically.

![](https://downloads.intercomcdn.com/i/o/j01nt7mc/2227652862/483afce81f4cb6e4bafa64b9a1e3/Screenshot+2026-04-01+at+3_49_07%E2%80%AFPM+%282%29.png?expires=1783016100&amp;signature=9dd3f24ce57f2d3e3d08e9b909856c2d5eaf2f36fecfcca1cde8784c7f8b5131&amp;req=diIlEc97n4lZW%2FMW1HO4zcpKAGDtTDEnVwKtu21T2i2i3q46mJvqbchtVGHm%0ACcYivmug4KiwsiVUBzw%3D%0A)

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

**NOTE**: You *do not* need to map every stage. We recommend mapping the key stages you want your partner to follow as a deal progresses through the sales cycle.

**Important:** The *Won* and *Lost* stages **must** be mapped for the integration to function correctly.

# Map Multiple Pipelines (Optional)

If you'd like to sync to more than one pipeline, you’ll also need to map the stages for each additional pipeline.

To do this:

- In the **Stage mapping** window, locate the pipeline selector on the left side.

- Select the pipeline you want to configure.

![](https://downloads.intercomcdn.com/i/o/j01nt7mc/2227657468/aa5d44438c4f02e23ea8cd794000/Screenshot+2026-04-01+at+3_48_37%E2%80%AFPM+%282%29.png?expires=1783016100&amp;signature=8a4f1fe7f518d5ddb53ac0fe5ddd0683848b91273ab74519a37e03831edddb59&amp;req=diIlEc97moVZUfMW1HO4zYD0CaJ1CZKdvzbJZc3ekC%2BMWNr2xOdpI5ThalIR%0AHiKSj9gdAPpsAd1LxYc%3D%0A)

- Map the **Zoho** stages to the corresponding portal phases, just as you did for the first pipeline.

  - [Learn how to customize your led phases](https://help.partnerportal.io/en/articles/8065753-how-to-customize-lead-phases-and-deal-stages)

- Repeat this process for each pipeline you’ve included in the integration.

Once you have finished mapping your stages, click the **Save** button on the **Stage** card.

# Step 3: Finalize

After configuring your pipeline and stages, look for the **Save mappings** button at the bottom of the page (on the main configuration area).

Your **Zoho** integration is now complete! Deals should begin syncing according to the rules you have set.

For more information on how to Customize your Lead Registration Form, check out this [article](https://help.partnerportal.io/en/articles/8732193-how-to-customize-the-lead-registration-form).