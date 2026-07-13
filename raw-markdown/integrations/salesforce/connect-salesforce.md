---
title: "How to connect Salesforce"
description: "This guide provides the steps to connect Salesforce."
---

Ensure you have administrative access to both Salesforce and the portal. Also, verify that you have the necessary permissions in Salesforce to create and manage integrations.

# **Enabling Salesforce Integration**

1. Navigate to the **Integrations** tab in the sidebar.

2. Select the **Enable Salesforce** button.

3. You’ll be prompted to log in to your Salesforce account. Enter your Salesforce credentials and grant the portal access to your Salesforce data.

# **Configuring the Integration**

After successful authentication, follow these steps to configure your integration to map fields between Salesforce and the portal by setting up real-time synchronization and defining lead assignment rules.

Map fields such as lead names, company names, date fields, and pick lists to align with how you want data to flow between the systems.

![](https://downloads.intercomcdn.com/i/o/1156209063/df5db5af81487c30c5241dee/1.png?expires=1778094900&amp;signature=e2082106a35c1d4253f35daa686e18e0ef604c65583b0acd13d1fc21473f7eea&amp;req=dSEiEMt%2BlIFZWvMW1HO4zWTAqQjiAjyL8RboFwUy3by0jdm8EeqL0UOkF8%2FY%0APIwndScC4LEwHRIZwDw%3D%0A)

# Mapping Custom Objects

1. **Mapping Fields**

  1. Map fields between Salesforce and the portal by setting up real-time synchronization and defining lead assignment rules.

  2. Map fields such as lead names, company names, date fields, and pick lists to align with how you want data to flow between the systems.

2. In the mapping section, use the dropdown in the grey box to select the custom objects you'd like to map.

3. Once a custom object is selected, begin mapping various fields. This includes mapping portal objects to Salesforce, such as fields in your lead registration form.

4. To add a new object, select the appropriate box next to or below your latest object.

![](https://downloads.intercomcdn.com/i/o/1156210281/23711edfa0689e76a98fc820/2.png?expires=1778094900&amp;signature=0b604c901ad99e22adfa9769870a3474faa68b23108fb4d2e886a6b8a3764045&amp;req=dSEiEMt%2FnYNXWPMW1HO4zXWVjVitCkimTtBKQYWnrjlK9kgkMOzK2u%2B7%2Fnhw%0Akz%2F5qqa%2BPJ4TKF76gY4%3D%0A)

**Mapping Options:**

- **Type:** Choose between Static Value, Portal Object, or Related Object.

- **Object:** Select from options like Lead or Partner.

- **Field:** Choose any field on your lead registration form.

![](https://downloads.intercomcdn.com/i/o/1156220528/7f9441a185060aad23ab705e/objects+ui.png?expires=1778094900&amp;signature=1b0c5d2529f2717bb320c3bd28eae09f49b6870e91d7978e2cbd19ac3a6e18ec&amp;req=dSEiEMt8nYRdUfMW1HO4zSWOM6eH3HlgeOeSB7JCqxSKR3R9gcv4EaPIodxa%0AtU4DsytYdMqbo5ImdeY%3D%0A)

![](https://downloads.intercomcdn.com/i/o/1156249230/45e9f5ffb7552d17de8a6ccf/mappings.png?expires=1778094900&amp;signature=fa2f29a6bb1ef870e87163f59ecdee58c281694f4d9c5a485ed04b7e5d679edc&amp;req=dSEiEMt6lINcWfMW1HO4zW7RcCzXzOoq6OZiQiApwAXSbJptocX47kRvT3Jg%0AV6oIHBJe%2F2DZ%2B5mDUho%3D%0A)

When mapping lead registrations, select **Portal Object** as the Type, **Lead** as the Object, and then choose the Field you want to map. Use **Static Value** to map the same information consistently.

# Mapping Lead Phases and Opportunity Stages

1. Decide on the visibility you'd like your partners to have during the opportunity cycle.

2. Create the **Opportunity** object and find the **Stage** option.

3. Set the Type to **Portal Object**, the Object to **Lead**, and the Field to **Phase**. Then, click **Map Values**.

4. Map your opportunity stages to the portal phases. You can choose to map them one-to-one or generalize them so that partners don’t see the full details of your sales process.

*For more information on creating custom lead phases, refer to this article.*

![](https://downloads.intercomcdn.com/i/o/1156227004/18c443ef906156bb1fbc6353/map+values.png?expires=1778094900&amp;signature=206cc6626f8ca2f2bca478cb04993dc10acd5ab44ee69da01f0b0f7eab7dacd5&amp;req=dSEiEMt8moFfXfMW1HO4zdOpRjLmINEzrh%2B30iadR2y7JErZ2a9e2Ni09%2Bav%0ADIHHpot%2FCICkzFuYMx0%3D%0A)

![](https://downloads.intercomcdn.com/i/o/1156232416/359631b6f8a9fa0cc8e0eeb3/Screenshot+2024-08-23+at+2_30_51%E2%80%AFPM.png?expires=1778094900&amp;signature=b9b00eb506f2f16ffe3a9c53f634ff9312d34560e80e45fcfbf9782f998279f7&amp;req=dSEiEMt9n4VeX%2FMW1HO4zfVKr8b1YEzJDeU5t%2BNSzEtQotrKpGCG%2FesTxTGr%0A2%2BhT5nro0znFlsLAEJM%3D%0A)

# Lead Conversion

You can customize your lead conversion process:

1. If you prefer to validate leads in Salesforce before converting them into opportunities, configure the integration to create only a lead object initially.

2. To do this, uncheck the **Create on Lead Approval** field for all objects except for the lead.

3. Later, convert leads to accounts, contacts, and opportunities in Salesforce as needed.

![](https://downloads.intercomcdn.com/i/o/1156224213/36c501c8894e84d11ff15e12/configuration+workflow.png?expires=1778094900&amp;signature=a044c45143b96dc56eb54cf5c2642e54a082eddac1117098e2900cae0093743b&amp;req=dSEiEMt8mYNeWvMW1HO4zZSa4N9QKzRobM7jh9w%2Fa117qEGRH4HusFvfPYUK%0AkhsDMpUOTa4zC4aW4IE%3D%0A)

# Other Integration Settings

Before beginning any mapping, you'll want to determine the integration settings.

**Primary Lead Object:**

- Select the Primary Lead object for your integration.

**Duplicate Handling:**

- Choose between **Adopt** or **Error** when mapping.

- **Error:** If a duplicate is detected in Salesforce, an error will occur when trying to create the object.

- **Adopt:** The existing record will be used and tracked going forward.

Our integration will pull all matching and duplicate rules from your Salesforce account.

**Error Handling:**

- **Don’t Cleanup:** If any object fails to be created in Salesforce, any previously created objects in the process will not be deleted.

- **Cleanup:** If an object fails to be created, all objects previously created as part of the process will be deleted.

![](https://downloads.intercomcdn.com/i/o/1156254479/3975e800185197a80ad8b234/other+settings.png?expires=1778094900&amp;signature=d1d78c09af04ea8a4e4d67fed462f477a1ff14b1f4579983751fde55b94aeb60&amp;req=dSEiEMt7mYVYUPMW1HO4zU0hSVF4%2F3Ml7d2FLd5EUUSGm80GpMK5tlyjD5i9%0AA%2Ff2IaesqnlbGU3una0%3D%0A)

For any questions, feel free to reach out to our team at [support@partnerportal.io](mailto:support@partnerportal.io).
