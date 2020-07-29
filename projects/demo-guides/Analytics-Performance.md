---
layout: default
---

# Demo Guide – Citrix Performance Analytics

**Author:** Russell Peters

**Date:** 24/07/20

## Overview



Secure Workspace & Improve user experience, machine learning will pull data from CVAD, CEM, Content & Collaboration & Networking & Access Control
Providing a user centric experience score

  >Note : This is a Citrix Cloud service, but can monitor an on prem Citrix Environment

  ![Performance Analytics Principles](/media/demo-guide-performace-analytics_1.png)

  ![Performance Analytics](/media/demo-guide-performace-analytics_2.png)




Pulling information in from multiple locations & processed by ML to issue a performance score based on other users & historic data
Broken down into users or infrastructure.
Site based & also different aspects of the user session
- User Experience
- User Sessions
- Session Failures
- Session Responsiveness
- Session Logon Duration

## Benefits
- Accurate Capacity Management
- Cost Savings by enabling customers to right size their environment
- Improved productivity by ensuring resource availability
- Continually evolving & learning to improve the whole ecosystem



>Note: Especially valuable in these times of home working & distributed workforce. Enabling insights into where capacity is needed & where performance issues for specific users may lie

## Citrix Differentiators
- Multiple different sources go to make up one user experience score
  - All Citrix Services
  - Azure AD
  -  Microsoft Security Graph
- ICA Traffic visibility
- E2E visibility
- Actionable insights
- Turnkey Easy to setup for Citrix Customers

## User Experience

Talk through the different metrics making up the user score.

  ![Performance Analytics](/media/demo-guide-performace-analytics_2.png)

How these can be viewed looked back on over a period of time if required

  ![Performance Analytics](/media/demo-guide-performace-analytics_3.png)

Or viewed based on site

  ![Performance Analytics](/media/demo-guide-performace-analytics_4.png)

> Note: Important point to note is that the score threshold is recalibrated every week based on the last 30 days of data

  ![Performance Analytics](/media/demo-guide-performace-analytics_5.png)

Drill into users with poor UX

  ![Performance Analytics](/media/demo-guide-performace-analytics_6.png)

### Factors affecting UX
- Session Availability
- Session Logon Duration
- Session Reliability
- Session Responsiveness

For each classification, select the drop down & talk through the different contributing factors
Example, session logon duration
- GPO
- Profile Load
- Logon script
- ETC…

### Prescriptive RCA
Drill into Profile load for possible reasons
Large profile causing logon to slow down

  ![Performance Analytics](/media/demo-guide-performace-analytics_7.png)

## User Sessions

  ![Performance Analytics](/media/demo-guide-performace-analytics_8.png)

Drill into session failures
Talk through the filters on the left hand side
- Endpoint OS
- Workspace App Version
- Delivery Group
- ETC…

  ![Performance Analytics](/media/demo-guide-performace-analytics_9.png)

Endpoint OS & Workspace App Version can be useful metrics to isolate version issues & report on client side updates

## Session Responsiveness  & Session Logon Duration

  ![Performance Analytics](/media/demo-guide-performace-analytics_10.png)

  ![Performance Analytics](/media/demo-guide-performace-analytics_11.png)

Drill into Poor Sessions

  ![Performance Analytics](/media/demo-guide-performace-analytics_12.png)

Identify a user with a poor experience & select the drop down to show mor information on what would be causing the issue

  ![Performance Analytics](/media/demo-guide-performace-analytics_13.png)

## Requirements

Outbound Connection over 443
- Citrix Cloud Account
- At least a trial or entitlement to the Analytics service
- The trial request is auto approve & should be instant

> Note: No Extra Infrastructure is required to implement Analytics

## More Info & Documentation

Citrix Performance Analytics
https://www.citrix.com/products/citrix-analytics-performance/

Citrix Analytics for Performance (Performance Analytics)
https://docs.citrix.com/en-us/performance-analytics.html

Data Governance
https://docs.citrix.com/en-us/performance-analytics/data-governance.html

Onboarding
https://docs.citrix.com/en-us/performance-analytics/onboarding.html

Citrix Analytics: Demystifying Data Source On-boarding
https://www.citrix.com/blogs/2018/08/10/citrix-analytics-demystifying-data-source-on-boarding/


