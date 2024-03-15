---
title: Configure forecasts in your organization
description: Configure forecasts in your organization to predict revenue and track sales performance. Learn how to set up and customize forecast configurations.
ms.date: 03/15/2024
ms.topic: how-to
author: lavanyakr01
ms.author: lavanyakr
searchScope:
  - D365-App-msdynce_saleshub
  - D365-Entity-msdyn_forecastconfiguration
  - D365-UI-*
  - Dynamics 365
  - Sales
  - Customer Engagement
ms.custom:
  - ai-gen-docs-bap
  - ai-gen-desc
  - ai-seo-date:03/12/2024
  - bap-template
---

# Configure forecasts in your organization

A forecast helps your organization predict how much revenue your sales team generates in a given time frame. When done correctly, forecasting can play a significant role in your company's success.  

[!INCLUDE [trial-cta-note](../includes/trial-cta-note.md)]

## License and role requirements

| Requirement type | You must have |
|-----------------------|---------|
| **License** | Dynamics 365 Sales Premium or Dynamics 365 Sales Enterprise  <br>For more information, see [Dynamics 365 Sales pricing](https://dynamics.microsoft.com/sales/pricing/). |
| **Security roles** | System Administrator or Forecast Manager <br> For more information, see [Predefined security roles for Sales](security-roles-for-sales.md).|

## How forecasting helps organizations?

Using forecasts:

- Sellers can track performance against targets and identify pipeline risks that might jeopardize their ability to hit the target.
- Managers can track individual sales performance against quotas to proactively provide coaching.
- Directors can use forecast trends to anticipate departmental sales and reallocate resources if necessary.
- Organization leaders can use the projected estimates to change the product strategy or provide updated projections to investors.

Forecasting isn't supported on Government Community Cloud (GCC) or mobile devices.

## Configure forecasting

You can configure forecasts that are based on revenue or quantity. You define the type of forecast, the hierarchy, access permissions, and the details you want sellers to see in their forecast view. After a forecast is activated, your sales team can view the revenue, or quantity, and pipeline projections.

1. In the Sales Hub app, select the Change area icon ![Icon to change the work area](./media/change-area-icon.png "Icon to change the work area") in the lower-left corner, and then select **App Settings**.  

1. Under **Performance management**, select **Forecast configuration**.

1. Follow the steps to configure a forecast from scratch or use the [sample forecast configuration](#use-the-sample-forecast-configuration) to get started quickly.  

    1. [Select a template](./select-template-forecast.md).  

    1. [Define and schedule a forecast model](define-general-properties-scheduling-forecast.md).

    1. [Provide access permissions](provide-permissions-forecast.md).

    1. [Configure columns and layouts](choose-layout-and-columns-forecast.md).

    1. [Configure and manage drill-down entities](configure-manage-drill-downs.md).

    1. [Configure advanced settings](forecast-configure-advanced-settings.md).

    1. [Activate the forecast and upload data](activate-upload-simple-columns-data-forecast.md).
    
### Use the sample forecast configuration

A ready-to-publish sample forecast configuration is available to you. Use the sample forecast to experiment and discover how forecasting works.  Learn how to tweak  the parameters and filters to suit your organization's needs.  

1. Go to **App Settings** > **Performance management** > **Forecast configuration**.

    You see a sample forecast configuration in your first-run experience. You can directly activate the forecast if you'd like to use the default settings. After the status turns **Active**, you can [view the forecast](view-forecasts.md).

    :::image type="content" source="media/activate-sample-forecast.png" alt-text="Screenshot of the three-dot menu for activating the sample forecast.":::

    If you want to know who has access to the forecast or restrict access to the forecast, continue with the following steps.

1. Select **Sample forecast**.

1. In the **General** step, check the **Preview** section to see the users who are part of the forecast. By default, all these users will have access to view the forecast after you activate it.

    :::image type="content" source="./media/forecast-general-tab-configuration-section.svg" alt-text="A screenshot of the General step of the Forecast configuration page, with a preview of the selected hierarchy shown.":::

1. If you want to limit access, go to the **Permissions** step and select the appropriate security roles.
1. Go to the **Activate & add quotas** step and select **Activate forecast** to make the forecast available to users in the hierarchy.
1. Wait for the status to turn **Active**.
1. [View the forecast](view-forecasts.md) to know the actual and forecasted values for your sales teams.


## Find your forecasts

In the **Sales** site map, find **Forecasts** under **Performance**.

:::image type="content" source="./media/forecast-select-sales-performance-forecasts.png" alt-text="Screenshot of the Sales Hub site map that shows Forecasts under Performance.":::

In the **Opportunity** form, **Forecast Category** appears above **Description**.

:::image type="content" source="./media/capture-forecast-category-opportunity-form.png" alt-text="Screenshot of an opportunity form with the Forecast category expanded.":::

 The categories define the confidence level of closing the opportunity. You can add custom values for your organization if you need to. To learn more, see [Capture forecast category for opportunity](./capture-forecast-category-opportunity.md).

- Forecast category options include **Won** and **Lost**. If an opportunity is closed as **Won** or **Lost**, the **Opportunity Forecast Category Mapping Process** out-of-the-box workflow automatically changes the forecast category to match.

- To view the **Opportunity Forecast Category Mapping Process** workflow, go to **Settings** > **Process Center** > **Processes** and select the **All Processes** view. Search for and open the **Opportunity Forecast Category Mapping Process** workflow. You can customize or deactivate the workflow according to your organization's requirements.

- Are you using a custom option set instead of a forecast category? You need to create a workflow to automatically sync the opportunity status with your option set to make sure that the projection is accurate.
To learn more, see [Create a cloud flow in Power Automate](/power-automate/get-started-logic-flow).

If you don't want to see the forecast category in the opportunity form, you need to customize the form. You can't use the **Visible by default** option to hide it. To learn more, see [Unable to hide forecast category field in opportunity forms](./ts-forecasts.md#hide_forecast_category_field).

>[!IMPORTANT]
>The forecasting feature is intended to help sales managers or supervisors enhance their team’s performance. It is not intended for use in making, and should not be used to make, decisions that affect the employment of an employee or group of employees, including compensation, rewards, seniority, or other rights or entitlements. Customers are solely responsible for using Dynamics 365, this feature, and any associated feature or service in compliance with all applicable laws, including laws relating to accessing individual employee analytics and monitoring, recording, and storing communications with users. This also includes adequately notifying users that their communications with sales persons may be monitored, recorded, or stored and, as required by applicable laws, obtaining consent from users before using the feature with them. Customers are also encouraged to have a mechanism in place to inform their sales persons that their communications with users may be monitored, recorded, or stored.

[!INCLUDE [cant-find-option](../includes/cant-find-option.md)]

<table>
<tr><td>

> [!div class="nextstepaction"]
> [Next step: Select a template](select-template-forecast.md)
</td></tr>
</table>

### See also

[Blog: Tips for setting up sales forecasting in Dynamics 365 Sales](https://cloudblogs.microsoft.com/dynamics365/it/2020/11/23/tips-for-setting-up-sales-forecasting-in-dynamics-365-sales/)  
[System and application users who can push data to Dataverse](/power-platform/admin/system-application-users)  
[Project accurate revenue with sales forecasting](project-accurate-revenue-sales-forecasting.md)  
[View forecasts](view-forecasts.md)  
[About premium forecasting](/dynamics365/ai/sales/configure-premium-forecasting)
[msdyn_ForecastApi action](developer/reference/custom-actions/msdyn_ForecastApi.md)  
[Forecasting FAQs](faqs-sales.md#forecasting)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
