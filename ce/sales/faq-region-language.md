---
title: Region and language FAQs
description: Find answers to frequently asked questions about regions and languages.
ms.date: 03/27/2024
ms.topic: troubleshooting
author: udaykirang
ms.author: udag
ms.reviewer: udag
ms.owner: shujoshi
ms.custom:
  - ai-gen-docs-bap
  - ai-gen-desc
  - ai-seo-date:03/11/2024
---

# Region and language FAQs

This article answers frequently asked questions about region and language support in Dynamics 365 Sales, Sales premium, and Sales professional.

## In which region is Sales Premium available? 
  
Sales Premium is only available in the following countries or regions:

- Asia Pacific (APJ)
- Canada (CAN)
- Europe, the Middle East, and Africa (EMEA)
- France (FRA)
- Germany (GER)
- Great Britain (GBR)
- India (IND)
- Japan (JPN)
- North America (NAM)
- Oceania (OCE)
- South Africa (ZAF)
- South America (SAM)
- Switzerland (CHE)  
- United Arab Emirates (UAE)

Sales Premium isn't available in all other regions and Government Community Cloud (GCC), including USG. 

## In which region are Sales Premium features available?

The following table lists the regions in which Sales Premium features are available.

| Feature | NAM | EMEA | GBR | APJ | CAN | IND | JPN | OCE | CHE | FRA | GER | SAM | ZAF | UAE |
|---------|-----|------|-----|-----|-----|-----|-----|-----|-----|-----|-----|-----|-----|-----|
| [Assistant](assistant.md) | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes |
| [Conversation intelligence](dynamics365-sales-insights-app.md) | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes |
| [Notes analysis](notes-analysis.md) | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes |
| [Premium forecasting](configure-premium-forecasting.md) | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | No | No | Yes | Yes | Yes |
| [Predictive lead scoring](work-predictive-lead-scoring.md) | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes |
| [Predictive opportunity scoring](work-predictive-opportunity-scoring.md)  | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes |
| [Sales accelerator](digital-selling-sales-accelerator.md) | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes |
| [Relationship analytics (Basic)](relationship-analytics-overview.md#basic-relationship-insights) | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes |
| [Relationship analytics (Enhanced)](relationship-analytics-overview.md#enhanced-relationship-insights)** | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes |
| [Who knows whom (Basic)](who-knows-whom.md#basic-who-knows-whom-information) | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes |
| [Who knows whom (Enhanced)](who-knows-whom.md#enhanced-who-knows-whom-information) | Yes | Yes | Yes | Yes | Yes | No | No | No | No | Yes | No | No | No | No |

** To use Exchange data for relationship analytics (enhanced), your organization's Office 365 data location must be in one of the [supported locations](#in-which-regions-is-exchange-integration-available). 

## Which version of Exchange is supported for features in Sales Premium?

The following table shows the version of Exchange that's supported for Sales Premium features.

| Feature | Exchange Online | Exchange Server 2013 and above | Is Exchange data mandatory? |
|---------|-----------------|--------------------------------|-----------------------|
| Relationship analytics (Basic) | Yes | No | No |
| Relationship analytics (Enhanced) | Yes | No | No* |
| Who knows whom (Basic)| Yes | No | No |
| Who knows whom (Enhanced)| Yes | No | Yes |
| Assistant | Yes | No | No |
| Email engagement | Yes | Yes | Yes |

** Though Exchange data isn't mandatory for relationship analytics (enhanced), it's recommended to enable Exchange integration to get more accurate and complete relationship information. For example, the response time KPI is generated from the data in Exchange only. If you don't enable Exchange integration, the response time KPI will be blank.

## In which regions is Exchange integration available?

Exchange integration is only available in specific regions. To use Exchange data for who knows whom and relationship analytics, your organization's Office 365 data location must be in one of the following locations and not in your region-specific data canter location:

- Global Geography 1 – EMEA (Austria, Finland, France, Great Britain, Ireland, Netherlands).
- Global Geography 2 – Asia Pacific	(Hong Kong SAR, Japan, Malaysia, Singapore, South Korea).
- Global Geography 3 – Americas (Brazil, Chile, United States).<br>

If your organization's Office 365 data is in any other region, who knows whom won't be available. However, relationship analytics will be available with the data in Dynamics 365.

To learn more on data center locations, see [Data Center Locations](/microsoft-365/enterprise/o365-data-locations?view=o365-worldwide#data-center-locations&preserve-view=true).

## What languages are supported for Sales Premium features?

The following table shows which languages are supported for Sales Premium features.

| Feature | Language supported |
|---------|--------------------|
| Assistant, Assistant studio, Email engagement, Predictive lead scoring, Predictive opportunity scoring, Premium forecasting, Relationship analytics, Sales accelerator, and Who knows whom | Arabic, Basque, Bulgarian, Catalan, Chinese Simplified (PRC), Chinese Traditional (Hong Kong SAR), Chinese Traditional (Taiwan), Croatian, Czech, Danish, Dutch, English, Estonian, Finnish, French, Galician, German, Greek, Hebrew, Hindi, Hungarian, Indonesian, Italian, Japanese, Kazakh, Korean, Latvian, Lithuanian, Malay, Norwegian, Polish, Portuguese (Brazil), Portuguese (Portugal), Romanian, Russian, Serbian (Cyrillic), Serbian (Latin), Slovakian, Slovenian, Spanish, Swedish, Thai, Turkish, Ukrainian, and Vietnamese. |
| Notes analysis | English, French, German, Italian, and Dutch for machine learning models. |
| Exchange insight cards in Assistant | Only English - United States (en-US) for machine learning models. |
| Conversation intelligence | Go to [Languages supported for conversation intelligence](language-support-conversation-intelligence.md) |

[Learn more about infrastructure availability (PDF)](https://aka.ms/dynamics_365_international_availability_deck).
