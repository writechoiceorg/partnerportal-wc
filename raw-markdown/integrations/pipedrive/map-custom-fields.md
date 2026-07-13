---
title: "How to Map Custom Fields to Pipedrive"
description: "This article will walk you through the steps to map custom fields to your Pipedrive CRM."
---

You can map custom fields from your portal to Pipedrive so information submitted through the Lead Registration form syncs correctly to your CRM.

**Note:** Before mapping, ensure that your custom fields exist both in the portal **and** in Pipedrive.

- For adding custom fields to your **Lead Registration Form**, see [How to customize your Lead Form](https://help.partnerportal.io/en/articles/8732193-how-to-customize-the-lead-registration-form).

- For creating custom fields in Pipedrive, see [Pipedrive Custom Fields](https://support.pipedrive.com/en/article/custom-fields).

# Step 1: Access the Integration Mapping

Once your custom fields are ready:

1. Navigate to the **Integrations** tab.

2. Select **Settings** for the **Pipedrive integration**.

3. Click **Configure** to open the integration mapping page.

# Step 2: Mapping Custom Fields

## Single-Line Text Fields

1. In the **object** of your choice (deal, person, organization), select the desired Pipedrive custom field from the dropdown.

  1. **Only** fields already **in** Pipedrive will appear on this drop-down.

  2.

2. Click the **Add** button next to the drop-down to include it in your mapping.

3. Click on the newly added field to configure the mapping. Set the fields as follows:

- **Type:** Portal Object

- **Object:** Lead

- **Field:** Select the corresponding **portal** field (from your lead form)

![](https://downloads.intercomcdn.com/i/o/j01nt7mc/2156023365/77e745bd972edeac3dade34d018e/Screenshot+2026-03-12+at+10_12_47%E2%80%AFAM+%282%29.png?expires=1778100300&amp;signature=ef62aa01fb738dd454f5f18440e8839458d36edf9945695f55f1c8e851d001df&amp;req=diEiEMl8noJZXPMW1HO4zSa1czKjcAfItFgG1qG5oBigLptkR1ws2dJ5YWbm%0AcwLsR81IsxWjueX3H5Q%3D%0A)

Click the **Save Mappings** button once you've finished mapping your fields.

## Picklists (Dropdown Fields)

1. Ensure the picklist field exists in **both** Pipedrive and the Lead Registration Form.

2. Select the custom picklist field from the the **object** dropdown.

3. Click **Add**.

  1.

4. Click the field to configure the mapping as follows:

- **Type:** Portal Object

- **Object:** Lead

- **Field:** Select the corresponding portal field

Next, click **Map Values** to match the dropdown options from your portal lead field with the corresponding Pipedrive dropdown values.

![](https://downloads.intercomcdn.com/i/o/j01nt7mc/2156033814/d14f6b3e712afd8c387ad73fadfa/Screenshot+2026-03-12+at+10_16_43%E2%80%AFAM+%282%29.png?expires=1778100300&amp;signature=f9d1972f327a97464da53629b2915577c3951cc468489196215d3c9929f79da2&amp;req=diEiEMl9noleXfMW1HO4zZj4sQ304Zqo7HDlF5UXZkGcQRAmWLbU9rpzaNKe%0Av5yOZLHhd8F2OqmPoyw%3D%0A)

When mapping values, we recommend the ***Map Manually*** option. This opens the mapping for you to chose which drop-down option you want to map to Pipedrive.

![](https://downloads.intercomcdn.com/i/o/j01nt7mc/2156047393/6ea3d0549053256b01c2e90aca50/Screenshot+2026-03-12+at+10_20_22%E2%80%AFAM+%282%29.png?expires=1778100300&amp;signature=cb3f22a5d85b7af6403a9c34907f738bd2a865d343c69e32fed9ab0ca1b8e5b7&amp;req=diEiEMl6moJWWvMW1HO4zZ41wjqGd3u%2FE4H3Uk0IALp5BO6T479KUQGzaChk%0Ay9R7v%2BOyFfARiMvU9%2FM%3D%0A)

Press the **Save** button in the window when done.

Click the **Save Mappings** button in the main mapping page once you've finished mapping your fields.

## Step 3: Mapping Fields That Are Not on the Lead Form

Some information—such as **partner details**—does not need to appear on the Lead Registration Form.

If the destination field *already* exists in Pipedrive, you can map it directly **without** adding a new portal field:

1. In the **Deal object**, select the Pipedrive field from the dropdown.

2. Click **Add**.

  1. ![](https://downloads.intercomcdn.com/i/o/j01nt7mc/2156066032/7cd19dffd4b2dedcf6baf6553f98/Screenshot%2B2026-03-10%2Bat%2B3_40_09-E2-80-AFPM%2B-282-29.png?expires=1778100300&amp;signature=fe8a78fb743b0c455a42bc8e174e7034f30890e1b0c7887e94b9faa4e4ff0493&amp;req=diEiEMl4m4FcW%2FMW1HO4zSNKycGsjfBG5Bb5yUWC6bkpwMfNZoq26yHQG6wv%0APkjF%0A)

3. Click the field to configure the mapping as follows:

- **Type:** Portal Object

- **Object:** Partner Organization to map Partner Company name or Partner User to map individual information

- **Field:** Select the information you want to map

  - ![](https://downloads.intercomcdn.com/i/o/j01nt7mc/2156078156/f2e8e3112b78f6c3237674960dbd/Screenshot+2026-03-12+at+10_28_35%E2%80%AFAM+%282%29.png?expires=1778100300&amp;signature=9e839dedcdf2defa414f48e8aa4f752f8b0419bd4f8aa0303ad903abcd8ae99f&amp;req=diEiEMl5lYBaX%2FMW1HO4zV7zoxhQOySClBiIlM3DhyuCmgzJjwlmu5UCubA1%0A0CLX%0A)

This allows you to send internal portal data—like **who submitted the lead**—directly to Pipedrive without requiring additional fields on the form.

Click the **Save Mappings** button once you've finished mapping your fields.

For information on connecting your Pipedrive CRM, check out [this article](https://help.partnerportal.io/en/articles/8991922-how-to-connect-to-pipedrive).
