---
title: Experience League testing
description: Syntax testing experience league
testing: here
mini-toc-levels: 0
---
# Experience League testing

`mini-toc-levels: 0`

We'll keep using the AdobeDocs repo to write documentation with the same Markdown syntax. However, we're building to a new pipeline and switching the output from `docs.adobe.com` to the `experienceleague.adobe.com` site.

We're now in the testing phase of Experience League output.

## Jenkins validation

During the testing phase, AdobeDocs repos are connected to both the current pipeline (`docs.adobe.com` via AEM) and the upcoming pipeline (`experienceleague.adobe.com` via Git bundle). Content is validated for each pipeline using a different set of rules. In nearly all cases, content that is valid for `docs.adobe.com` will also be valid for Experience League. There are exceptions for both pipelines.

To see the validation status of repos on Experience League, see the `ExL` tab in Jenkins:

* [https://docs.ci.corp.adobe.com/view/exl/](https://docs.ci.corp.adobe.com/view/exl/)

## Output to Experience League

When you commit any change to the main branch on AdobeDocs, validated content is packaged (quickly!) for Experience League and uploaded to a server.

You can check validation for your repo here:

[Jenkins exl validation](https://docs.ci.corp.adobe.com/view/exl/)

Updates to AdobeDocs repos are activated periodically (currently every 6 hours: 5am/11am/5pm/11pm PDT) on `experienceleague.adobe.com`.

### User Guides on ExL

Note that user guides are not yet stitched together properly in doc sets. We're still working on this functionality, which we refer to as work on the "manifest."

>[!TIP]
>
>If your repo is hooked up to EXL, you can change the domain for any docs.adobe.com article to see that page rendered in Experience League.
>
>Change: `https://docs.adobe.com/content/help/en/`
>
>To: `https://experienceleague.adobe.com/docs/`

#### Home

* [AdobeDocs Home](https://%65xperienceleague.adobe.com/docs/)

#### Landing Pages

* [Advertising Cloud Landing](https://%65xperienceleague.adobe.com/docs/advertising-cloud.html)
* [Analytics Landing](https://%65xperienceleague.adobe.com/docs/analytics.html)
* [Audience Manager Landing](https://%65xperienceleague.adobe.com/docs/audience-manager.html)
* [AEM as a Cloud Service Landing](https://%65xperienceleague.adobe.com/docs/experience-manager-cloud-service.html)
* [AEM 6.5 Landing](https://%65xperienceleague.adobe.com/docs/experience-manager-65.html)
* [AEM 6.4 Landing](https://%65xperienceleague.adobe.com/docs/experience-manager-64.html)
* [AEM Tutorials Landing](https://%65xperienceleague.adobe.com/docs/experience-manager-tutorials.html)
* [Campaign Classic Landing](https://%65xperienceleague.adobe.com/docs/campaign-classic.html)
* [Campaign Standard Landing](https://%65xperienceleague.adobe.com/docs/campaign-standard.html)
* [Core Services Landing](https://%65xperienceleague.adobe.com/docs/core-services.html)
* [Experience Platform Landing](https://%65xperienceleague.adobe.com/docs/experience-platform.html)
* [Primetime Landing](https://%65xperienceleague.adobe.com/docs/primetime.html)
* [Target Landing](https://%65xperienceleague.adobe.com/docs/target.html)

#### Additional Guides

* [Adobe Acrobat Learn Hub](https://%65xperienceleague.adobe.com/docs/document-cloud-learn/acrobat-learning/overview.html?lang=en)
* [Adobe Sign Learn Hub](https://%65xperienceleague.adobe.com/docs/document-cloud-learn/sign-learning-hub/overview.html?lang=en)
* [Core Services Landing](https://%65xperienceleague.adobe.com/docs/core-services.html)
* [AEM Main Landing (optional)](https://%65xperienceleague.adobe.com/docs/experience-manager.html) - We're not sure if we'll use this, but it's here if we need it.
* [Customer Intelligence](https://%65xperienceleague.adobe.com/docs/experience-platform/intelligent-services/home.html?lang=en) - Do we need a landing page?
* [Customer Journey Analytics](https://%65xperienceleague.adobe.com/docs/analytics-platform/using/cja-landing.html) - Do we need a landing page?
* [Journey Orchestration](https://%65xperienceleague.adobe.com/docs/journeys/using/journey-orchestration-home.html) - Do we need a landing page?
* [Real-Time Customer Data Platform](https://%65xperienceleague.adobe.com/docs/experience-platform/rtcdp/overview.html) - Do we need a landing page?
* [Release Notes](https://%65xperienceleague.adobe.com/docs/release-notes/experience-cloud/current.html?lang=en)
* [Search&Promote](https://%65xperienceleague.adobe.com/docs/search-promote/using/sp-home.html?lang=en)
* [Software Distribution](https://%65xperienceleague.adobe.com/docs/experience-cloud/software-distribution/home.html?lang=en)

* [Old ad hoc landing page for tutorials](https://%65xperienceleague.adobe.com/docs/experience-cloud/tutorials/home.html#tutorials) - Do we need a new landing page for all tutorials?

<!--

**Advertising Cloud**

* [Advertising Cloud](https://%65xperienceleague.adobe.com/docs/advertising-cloud/all/home.html) (staged)

**AEM**

* [AEM as a Cloud Service](https://%65xperienceleague.adobe.com/docs/experience-manager-cloud-service/landing/home.html)
* [AEM 6.5](https://%65xperienceleague.adobe.com/docs/experience-manager-65/user-guide/home.html)
* [AEM 6.4](https://%65xperienceleague.adobe.com/docs/experience-manager-64/user-guide/home.html)
* [AEM Automated Forms Conversion Service](https://%65xperienceleague.adobe.com/docs/aem-forms-automated-conversion-service/using/introduction.html)
* [AEM Brand Portal](https://%65xperienceleague.adobe.com/docs/experience-manager-brand-portal/using/home.html) 
* [AEM Cloud Manager](https://%65xperienceleague.adobe.com/docs/experience-manager-cloud-manager/using/introduction-to-cloud-manager.html) 
* [AEM Core Components](https://%65xperienceleague.adobe.com/docs/experience-manager-core-components/using/introduction.html) 
* [AEM Desktop](https://%65xperienceleague.adobe.com/docs/experience-manager-desktop-app/using/introduction.html) 
* [AEM Dispatcher](https://%65xperienceleague.adobe.com/docs/experience-manager-dispatcher/using/dispatcher.html)
* [AEM HTL](https://%65xperienceleague.adobe.com/docs/experience-manager-htl/using/overview.html)
* [AEM Screens](https://%65xperienceleague.adobe.com/docs/experience-manager-screens/user-guide/aem-screens-introduction.html)

**Analytics**

* [Analytics](https://%65xperienceleague.adobe.com/docs/analytics.html)
* [Media Analytics](https://%65xperienceleague.adobe.com/docs/media-analytics/using/media-overview.html)
* [Analytics Real-time Customer Data Platform](https://%65xperienceleague.adobe.com/docs/experience-platform/rtcdp/overview.html)
* [Data Workbench](https://%65xperienceleague.adobe.com/docs/data-workbench/using/home.html)
* [Journey Orchestration](https://%65xperienceleague.adobe.com/docs/journeys/using/journey-orchestration-home.html)

* [Analytics Implementation Setup](https://%65xperienceleague.adobe.com/docs/analytics-implementation-setup/implementation-setup/home.html) (not live; stale)

**AAM**

* [Audience Manager](https://%65xperienceleague.adobe.com/docs/audience-manager/user-guide/aam-home.html)
* [Audience Manager Admin](https://%65xperienceleague.adobe.com/docs/audience-manager-admin/admin-guide/admin-home.html)

**Target**

* [Target](https://%65xperienceleague.adobe.com/docs/target/using/target-home.html) 

**Campaign**

* [Campaign Classic](https://%65xperienceleague.adobe.com/docs/campaign-classic/using/campaign-classic-home.html)
* [Campaign Standard](https://%65xperienceleague.adobe.com/docs/campaign-standard/using/campaign-standard-home.html)

**Platform, Core, Misc**

* [Auditor](https://%65xperienceleague.adobe.com/docs/auditor/using/overview.html)
* [Control Panel](https://%65xperienceleague.adobe.com/docs/control-panel/using/control-panel-home.html) (staged)
* [Core Services](https://%65xperienceleague.adobe.com/docs/core-services/interface/marketing-cloud-integrations.html)
* [Customer One](https://%65xperienceleague.adobe.com/docs/customer-one/using/home.html)
* [Debugger](https://%65xperienceleague.adobe.com/docs/debugger/using/experience-cloud-debugger.html)
* [Device Co-op](https://%65xperienceleague.adobe.com/docs/device-co-op/using/home.html)
* [DTM](https://%65xperienceleague.adobe.com/docs/dtm/using/dtm-home.html)
* [Dynamic Media Classic](https://%65xperienceleague.adobe.com/docs/dynamic-media-classic/using/home.html)
* [Dynamic Media Developer Resources](https://%65xperienceleague.adobe.com/docs/dynamic-media-developer-resources/landing/home.html) (staged)
* [Experience Cloud Landing](https://%65xperienceleague.adobe.com/docs/experience-cloud/user-guides/home.html) (links point to docs.adobe.com, so kinda useless)
* [ID Service](https://%65xperienceleague.adobe.com/docs/id-service/using/home.html)
* [Launch](https://%65xperienceleague.adobe.com/docs/launch/using/overview.html)
* [Livefyre](https://%65xperienceleague.adobe.com/docs/livefyre/using/home.html)
* [Magento PAAS](https://%65xperienceleague.adobe.com/docs/magento-paas/paas/overview.html) (staged)
* [Marketo Sky](https://%65xperienceleague.adobe.com/docs/marketo/sky/home.html) (staged)
* [Mobile Services](https://%65xperienceleague.adobe.com/docs/mobile-services/using/home.html)
* [Places](https://%65xperienceleague.adobe.com/docs/places/using/home.html)
* [Platform](https://%65xperienceleague.adobe.com/docs/experience-platform/landing/home.html)
* [Primetime](https://%65xperienceleague.adobe.com/docs/primetime/programming/home.html)
* [Release Notes](https://%65xperienceleague.adobe.com/docs/release-notes/experience-cloud/current.html)
* [Search&Promote](https://%65xperienceleague.adobe.com/docs/search-promote/using/sp-home.html)
* [Social](https://%65xperienceleague.adobe.com/docs/social/using/home.html) (EOL-ignore)
* [Authoring Guide](https://%65xperienceleague.adobe.com/docs/collaborative-doc-instructions/collaboration-guide/home.html?lang=en#collaboration-guide)

**Tech Marketing Tutorials**

* [AEM Learn Tutorials](https://%65xperienceleague.adobe.com/docs/experience-manager-learn/cloud-service/overview.html) 
* [Analytics Learn Tutorials](https://%65xperienceleague.adobe.com/docs/analytics-learn/tutorials/overview.html)
* [Audience Manager Learn](https://%65xperienceleague.adobe.com/docs/audience-manager-learn/tutorials/overview.html)
* [Campaign Standard Learn Tutorials](https://%65xperienceleague.adobe.com/docs/campaign-standard-learn/tutorials/overview.html) 
* [Campaign Classic Learn Tutorials](https://%65xperienceleague.adobe.com/docs/campaign-classic-learn/tutorials/overview.html)
* [Core Services Learn](https://%65xperienceleague.adobe.com/docs/core-services-learn/tutorials/overview.html)
* [Document Cloud Learn](https://%65xperienceleague.adobe.com/docs/document-cloud-learn/sign-tutorials/overview.html)
* [Journey Orchestration Learn](https://%65xperienceleague.adobe.com/docs/journey-orchestration-learn/tutorials/overview.html)
* [Platform Learn](https://%65xperienceleague.adobe.com/docs/platform-learn/comprehensive-technical-tutorial/overview.html)
* [Target Learn Tutorials](https://%65xperienceleague.adobe.com/docs/target-learn/tutorials/overview.html)

-->

>[!NOTE]
>
>Can't find a guide? Check [Jenkins ExL](https://docs.ci.corp.adobe.com/view/exl/) to see if your repo is listed (and passing validation). If it doesn't appear, please file a JIRA issue ([example](https://jira.corp.adobe.com/browse/UGP-2368)) and assign Bob Bringhurst.


## Logging issues

Use Jira to create Experience League issues and link them to the docs migration epic:

[JIRA - Issues with docs migration content](https://jira.corp.adobe.com/browse/UGP-1245)

Click the + sign to add an issue to the Docs Migration epic.

![testing](/help/test-guide/assets/jira-plus.png)

Here's the [ExL Backlog](https://jira.corp.adobe.com/secure/RapidBoard.jspa?rapidView=22918&view=planning&selectedEpic=UGP-1245) for reference.
