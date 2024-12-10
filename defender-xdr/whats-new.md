---
title: What's new in Microsoft Defender XDR
description: Lists the new features and functionality in Microsoft Defender XDR
search.appverid: met150
ms.service: defender-xdr
ms.author: diannegali
author: diannegali
ms.localizationpriority: medium
ms.date: 12/03/2024
manager: dansimp
audience: ITPro
ms.collection:
- M365-security-compliance
- tier1
ms.topic: conceptual
---

# What's new in Microsoft Defender XDR

Lists the new features and functionality in Microsoft Defender XDR.

For more information on what's new with other Microsoft Defender security products and Microsoft Sentinel, see:

- [What's new in Microsoft Defender for Office 365](/defender-office-365/defender-for-office-365-whats-new)
- [What's new in Microsoft Defender for Endpoint](/defender-endpoint/whats-new-in-microsoft-defender-endpoint)
- [What's new in Microsoft Defender for Identity](/defender-for-identity/whats-new)
- [What's new in Microsoft Defender for Cloud Apps](/cloud-app-security/release-notes)
- [What's new in Microsoft Sentinel](/azure/sentinel/whats-new)

You can also get product updates and important notifications through the [message center](https://admin.microsoft.com/Adminportal/Home#/MessageCenter).

## December 2024
- (Preview) The [Link to incident](advanced-hunting-defender-results.md#link-query-results-to-an-incident) feature in Microsoft Defender advanced hunting now allows linking of Microsoft Sentinel query results. In both the Microsoft Defender unified experience and in [Defender XDR advanced hunting](advanced-hunting-link-to-incident.md), you can now specify whether an entity is an impacted asset or related evidence.
- (Preview) In [advanced hunting](advanced-hunting-defender-use-custom-rules.md#use-adx-operator-for-azure-data-explorer-queries-preview), Microsoft Defender portal users can now use the `adx()` operator to query tables stored in Azure Data Explorer. You no longer need to go to log analytics in Microsoft Sentinel to use this operator if you are already in Microsoft Defender.
-  New documentation library for Microsoft's unified security operations platform. Find centralized documentation about [Microsoft's unified SecOps platform in the Microsoft Defender portal](/unified-secops-platform/overview-unified-security). Microsoft's unified SecOps platform brings together the full capabilities of Microsoft Sentinel, Microsoft Defender XDR, Microsoft Security Exposure Management, and generative AI into the Defender portal. Learn about the features and functionality available with Microsoft's unified SecOps platform, then start to plan your deployment.

## November 2024

- We've updated the steps to create tenant groups in multitenant management. Learn the new steps in the [content distribution using tenant groups in multitenant management](mto-tenantgroups.md).
- (Preview) **Attack paths** in the incident graph are now available in the Microsoft Defender portal. The attack story now includes potential attack paths that show the paths that attackers can potentially take after compromising a device. This feature helps you prioritize your response efforts. For more information, see [attack paths in the attack story](investigate-incidents.md#attack-paths).
- (Preview) Microsoft Defender XDR customers can now export incident data to PDF. Use the exported data to easily capture and share incident data to other stakeholders. For details, see **[Export incident data to PDF](manage-incidents.md#export-incident-data-to-pdf)**.
- (GA) The **last update time** column in the [incident queue](incident-queue.md#incident-queue) is now generally available.
- (Preview) Cloud-native investigation and response actions are now available for container-related alerts in the Microsoft Defender portal. Security operations center (SOC) analysts can now investigate and respond to container-related alerts in near real-time with cloud-native response actions and investigation logs to hunt for related activities. For more information, see [Investigate and respond to container threats in the Microsoft Defender portal](investigate-respond-container-threats.md).
- (GA) The `arg()` operator in [advanced hunting](advanced-hunting-defender-use-custom-rules.md#use-arg-operator-for-azure-resource-graph-queries) in Microsoft Defender portal is now generally available. Users can now use the *arg()* operator for Azure Resource Graph queries to search over Azure resources, and no longer need to go to Log Analytics in Microsoft Sentinel to use this operator if already in Microsoft Defender.
- (Preview) The [CloudProcessEvents](advanced-hunting-cloudprocessevents-table.md) table is now available for preview in advanced hunting. It contains information about process events in multicloud hosted environments. You can use it to discover threats that can be observed through process details, like malicious processes or command-line signatures.
- (Preview) Migrating custom detection queries to **Continuous (near real-time or NRT) frequency** is now available for preview in advanced hunting. Using the Continuous (NRT) frequency increases your organization's ability to identify threats faster. It has minimal to no impact to your resource usage, and should thus be considered for any qualified custom detection rule in your organization. You can migrate compatible KQL queries by following the steps in [Continuous (NRT) frequency](custom-detection-rules.md#continuous-nrt-frequency).

## October 2024

- [Microsoft Unified RBAC roles](experts-on-demand.md#required-permissions-for-using-ask-defender-experts) are added with new permission levels for Microsoft Threat Experts customers to use Ask Defender experts capability.
- (Preview) In [advanced hunting](advanced-hunting-defender-use-custom-rules.md#use-arg-operator-for-azure-resource-graph-queries), Microsoft Defender portal users can now use the `arg()` operator for Azure Resource Graph queries to search over Azure resources. You no longer need to go to Log Analytics in Microsoft Sentinel to use this operator if you are already in Microsoft Defender.

## September 2024

- (GA) The global search for entities in the Microsoft Defender portal is now generally available. The enhanced search results page centralizes the results from all entities. For more information, see [Global search in the Microsoft Defender portal](microsoft-365-defender-portal.md#global-search).
- (GA) Copilot in Defender now includes the identity summary capability, providing instant insights into a user's risk level, sign in activity, and more. For more information, see [Summarize identity information with Copilot in Defender](security-copilot-defender-identity-summary.md).
- [Microsoft Defender Threat Intelligence](/defender/threat-intelligence/what-is-microsoft-defender-threat-intelligence-defender-ti) customers can now view the [latest featured threat intelligence articles](/defender/threat-intelligence/learn-how-to-access-microsoft-defender-threat-intelligence-and-make-customizations-in-your-portal#featured-threat-intelligence-articles-widget) in the Microsoft Defender portal home page. The **Intel explorer** page now also has an [article digest](/defender/threat-intelligence/learn-how-to-access-microsoft-defender-threat-intelligence-and-make-customizations-in-your-portal#article-digest) that notifies them of the number of new Defender TI articles that were published since they last accessed the Defender portal.
- [Microsoft Defender XDR Unified RBAC permissions](experts-on-demand.md#required-permissions-for-using-ask-defender-experts) are added to submit inquiries and view responses from [Microsoft Defender Experts](experts-on-demand.md). You can also [view responses](experts-on-demand.md#where-to-view-responses-from-defender-experts) to inquires submitted to Ask Defender Experts through your listed email addresses when submitting your inquiry or in the Defender portal by navigating to **Reports** > **Defender Experts messages**.
- (GA) **Advanced hunting context panes** are now available in more experiences. This allows you to access the advanced hunting feature without leaving your current workflow. 
    - For incidents and alerts generated by analytics rules, you can select **Run query** to explore the results of the related analytics rule. 
    - In the analytics rule wizard's *Set rule logic* step, you can select **View query results** to verify the results of the query you are about to set. 
    - In the [query resources report](advanced-hunting-limits.md#find-resource-heavy-queries), you can view any of the queries by selecting the three dots on the query row and selecting **Open in query editor**. 
    - For device entities involved in incidents or alerts, **Go hunt** is also available as one of the options after selecting the three dots on the device side panel.




## August 2024

- (Preview) Microsoft Sentinel data is now available with Defender XDR data in Microsoft Defender multitenant management. Only one Microsoft Sentinel workspace per tenant is currently supported in the Microsoft unified security operations platform. So, Microsoft Defender multitenant management shows security information and event management (SIEM) data from one Microsoft Sentinel workspace per tenant. For more information, see [Microsoft Defender multitenant management](mto-overview.md) and [Microsoft Sentinel in the Microsoft Defender portal](/azure/sentinel/microsoft-sentinel-defender-portal).
- To ensure a smooth experience while navigating the Microsoft Defender portal, configure your network firewall by adding the appropriate addresses to your allow list. For more information, see [Network firewall configuration for Microsoft Defender XDR](m365d-enable.md#configure-your-network-firewall).


## July 2024

- Incidents with alerts where a compromised device communicated with an operational technology (OT) device are now visible in the Microsoft Defender portal through the [Microsoft Defender for IoT license and Defender for Endpoint’s device discovery capabilities](/defender-endpoint/device-discovery#device-discovery-integration). Using Defender for Endpoint data, Defender XDR automatically correlates these new OT alerts to incidents to provide a comprehensive attack story. To filter related incidents, see [Prioritize incidents in the Microsoft Defender portal](incident-queue.md#filters-).  

- (GA) Filtering Microsoft Defender for Cloud alerts by the associated **alert subscription ID** in the Incidents and Alerts queues is now generally available. For more information, see [Microsoft Defender for Cloud in Microsoft Defender XDR](microsoft-365-security-center-defender-cloud.md).

- (GA) The **Microsoft unified security operations platform** in the Microsoft Defender portal is generally available. This release brings together the full capabilities of Microsoft Sentinel, Microsoft Defender XDR, and Microsoft Copilot in Microsoft Defender. For more information, see the following resources:

- Blog post: [General availability of the Microsoft unified security operations platform](https://aka.ms/unified-soc-announcement)
  - [Microsoft Sentinel in the Microsoft Defender portal](https://go.microsoft.com/fwlink/p/?linkid=2263690)
  - [Connect Microsoft Sentinel to Microsoft Defender XDR](microsoft-sentinel-onboard.md)
  - [Microsoft Copilot in Microsoft Defender](security-copilot-in-microsoft-365-defender.md)

- (Preview) You can now customize columns in the **Incidents** and **Alerts** queues in the Microsoft Defender portal. You can add, remove, reorder columns to display the information you need. For more information, see how to customize columns in the [incident queue](incident-queue.md#incident-queue) and [alert queue](investigate-alerts.md).

- (Preview) **Critical assets** are now part of the tags in the incident and alert queues. When a critical asset is involved in an incident or alert, the critical asset tag is displayed in the queues. For more information, see [incident tags](manage-incidents.md#add-incident-tags) and the [alert queue](investigate-alerts.md).

- (Preview) Incidents are now arranged according to the latest automatic or manual updates made to an incident. Read about the **last update time** column in the [incident queue](incident-queue.md#incident-queue).

- (GA) Learning hub resources have moved from the Microsoft Defender portal to [learn.microsoft.com](https://go.microsoft.com/fwlink/?linkid=2273118). Access Microsoft Defender XDR Ninja training, learning paths, training modules and more. Browse the [list of learning paths](/training/browse/?products=m365-ems-cloud-app-security%2Cdefender-for-cloud-apps%2Cdefender-identity%2Cm365-information-protection%2Cm365-threat-protection%2Cmdatp%2Cdefender-office365&expanded=m365%2Coffice-365), and filter by product, role, level, and subject. 

- (GA) The **[UrlClickEvents](advanced-hunting-urlclickevents-table.md)** table in advanced hunting is now generally available. Use this table to get information about [Safe Links](/defender-office-365/safe-links-about) clicks from email messages, Microsoft Teams, and Office 365 apps in supported desktop, mobile, and web apps.

- (GA) You can now **release or move email messages from quarantine** back to the user's inbox directly from [Take actions in advanced hunting](advanced-hunting-take-action.md#take-various-actions-on-emails) and in [custom detections](custom-detection-rules.md#actions-on-emails). This allows security operators to manage false positives more efficiently and without losing context. 



## June 2024

- (Preview) **[Content distribution through tenant groups in multitenant management](mto-tenantgroups.md)** is now available. Content distribution helps you manage content at scale across tenants in multitenant management in Microsoft Defender XDR. In content distribution, you can create tenant groups to copy existing content, like custom detection rules, from the source tenant to the target tenants you assign during tenant group creation. The content then runs on the target tenant's devices or device groups that you set in the tenant group scope.

- (Preview) You can now filter your Microsoft Defender for Cloud alerts by the associated **alert subscription ID** in the Incidents and Alerts queues. For more information, see [Microsoft Defender for Cloud in Microsoft Defender XDR](microsoft-365-security-center-defender-cloud.md).

- (GA) You can now **[filter your results](advanced-hunting-query-results.md#filter-results)** in advanced hunting so you can narrow down your investigation on specific data you want to focus on.

## May 2024

- (Preview) Security analysts can now investigate a user's insider risk in the Microsoft Defender portal with **insider risk severity and insights** available for Microsoft Defender XDR users with provisioned access to Microsoft Purview Insider Risk Management. See the [entity details in the user page](investigate-users.md#entity-details) for more information.

- (GA) The endpoint security policies page is now available in multitenant management in Microsoft Defender XDR. Create, edit, and delete security policies for your tenants' devices from the **Endpoint security policies** page. For more information, see [Endpoint security policies in multitenant management](mto-endpoint-security-policy.md).

- Create alert tuning rules using **Alert severity** and **Alert title** values as conditions. Alert tuning can help you streamline the alert queue, saving triage time by hiding or resolving alerts automatically, each time a certain expected organizational behavior occurs, and rule conditions are met. For more information, see [Tune an alert](investigate-alerts.md#tune-an-alert).
- (Preview) **Turn preview options on in the main Microsoft 365 Defender settings** together with other Microsoft 365 Defender preview features. Customers who aren't using preview features yet will continue to see the legacy settings under **Settings > Endpoints > Advanced features > Preview features**. For more information, see [Microsoft 365 Defender preview features](/defender-xdr/preview).
- (Preview) The **SOC optimizations** page in the Microsoft Defender portal is now available with the [unified security operations platform](https://go.microsoft.com/fwlink/p/?linkid=2263690). Integrate Microsoft Defender XDR and Microsoft Sentinel and use SOC optimizations to optimize both processes and outcomes, without having your SOC teams spend time on manual analysis and research. For more information, see:

  - [Optimize your security operations](https://aka.ms/soc-opt-from-defender)
  - [SOC optimization reference](https://aka.ms/soc-opt-ref)

- (Preview) **Search** in the Microsoft Defender portal now includes the ability to search for devices and users in Microsoft Sentinel. Use the search bar to search for incidents, alerts, and other data across Microsoft Defender XDR and Microsoft Sentinel. For more information, see [Search in Microsoft Defender](microsoft-365-defender-portal.md#global-search).

- (Preview) The **[CloudAuditEvents](advanced-hunting-cloudauditevents-table.md)** table is now available in advanced hunting. This allows you to hunt through cloud audit events in Microsoft Defender for Cloud and to create custom detections to surface suspicious Azure Resource Manager and Kubernetes (KubeAudit) control plane activities.

- (GA) Automatic soft-deletion of sender's copy when *Soft delete* is selected as an action for email messages is now available in the Take actions wizard in advanced hunting. This new feature streamlines the process of managing Sent items, particularly admins who use *Soft delete* and *Move to inbox* actions. Read [Take actions on emails](advanced-hunting-take-action.md#take-various-actions-on-emails) for details.

- (Preview) You can now query Microsoft Sentinel data using the [advanced hunting query API](/graph/api/security-security-runhuntingquery?view=graph-rest-1.0&tabs=http&preserve-view=true). You can use the `timespan` parameter to query Defender XDR and Microsoft Sentinel data that have longer data retention than the Defender XDR default of 30 days.

- (Preview) In the unified Microsoft Defender portal, you can now create custom detections in querying data that spans Microsoft Sentinel and Defender XDR tables. Read [Create custom analytics and detection rules](advanced-hunting-defender-use-custom-rules.md) for more information.

- Updated [troubleshooting steps for Microsoft Defender Experts app permissions in Microsoft Teams](teams-restrictions-dexapp.md).
 
## April 2024

- (Preview) The **unified security operations platform** in the Microsoft Defender portal is now available. This release brings together the full capabilities of Microsoft Sentinel, Microsoft Defender XDR, and Microsoft Copilot in Microsoft Defender. For more information, see the following resources:

  - Blog announcement: [Unified security operations platform ready to revolutionize protection and efficiency](https://aka.ms/unified-soc-announcement)
  - [Microsoft Sentinel in the Microsoft Defender portal](https://go.microsoft.com/fwlink/p/?linkid=2263690)
  - [Connect Microsoft Sentinel to Microsoft Defender XDR](microsoft-sentinel-onboard.md)
  - [Microsoft Security Copilot in Microsoft Defender](security-copilot-in-microsoft-365-defender.md)

- (GA) **[Microsoft Copilot in Microsoft Defender](security-copilot-in-microsoft-365-defender.md)** is now generally available. Copilot in Defender helps you investigate and respond to incidents faster and more effectively. Copilot provides guided responses, incident summaries, and reports, helps you build KQL queries to hunt for threats, provide file and script analyses, and enable you to summarize relevant and actionable threat intelligence.
- Copilot in Defender customers can now export incident data to PDF. Use the exported data to easily share incident data, facilitating discussions with your security teams and other stakeholders. For details, see **[Export incident data to PDF](manage-incidents.md#export-incident-data-to-pdf)**.
- **Notifications in the Microsoft Defender portal** are now available. On the top right-hand side of the Defender portal, select the bell icon to view all your active notifications. Learn more about **[notifications in the Microsoft Defender portal](microsoft-365-defender-portal.md#notifications)**.
- The `AzureResourceId` column, which shows the unique identifier of the Azure resource associated with a device, is now available in the [DeviceInfo](advanced-hunting-deviceinfo-table.md) table in advanced hunting.

## February 2024

- (GA) **Dark mode** is now available in the Microsoft Defender portal. In the Defender portal, on the top right-hand side of the homepage, select **Dark mode**. Select **Light mode** to change the color mode back to the default.

- (GA) **Assigning severity to incidents**, **assigning an incident to a group**, and the ***go hunt*** option from the attack story graph are now generally available. Guides to learn how to [assign or change incident severity](manage-incidents.md#assign-or-change-incident-severity) and [assign an incident to a group](manage-incidents.md#assign-an-owner) are in the [Manage incidents](manage-incidents.md) page. Learn how you can use the *go hunt* option by exploring [attack story](investigate-incidents.md#attack-story).

- (Preview) **[Custom detection rules in Microsoft Graph security API](/graph/api/resources/security-api-overview?view=graph-rest-beta&preserve-view=true#custom-detections)** are now available. Create advanced hunting custom detection rules specific to your org to proactively monitor for threats and take action.

> [!Warning]
> The 2024-02 platform release causes inconsistent results for device control customers using removable media policies with disk/device-level access only (masks that are less of equal to 7). The enforcement might not work as expected.
> To mitigate this issue, rolling back to the previous version of the Defender platform is recommended.

## January 2024

- **Defender Boxed is available for a limited period of time**. Defender Boxed highlights your organization's security successes, improvements, and response actions during 2023. Take a moment to celebrate your organization's improvements in security posture, overall response to detected threats (manual and automatic), blocked emails, and more.

   - Defender Boxed opens automatically when you go to the **Incidents** page in the Microsoft Defender portal.
   - If you close Defender Boxed and you want to reopen it, in the Microsoft Defender portal, go to **Incidents**, and then select **Your Defender Boxed**.
   - Act quickly! Defender Boxed is available only for a short period of time.

- Defender Experts for XDR now lets you [receive managed response notifications and updates using Teams](get-started-xdr.md#receive-managed-response-notifications-and-updates-in-microsoft-teams). You can also chat with Defender Experts regarding incidents where managed response is issued.

- (GA) New functionality in the **incident queue's available filters** is now generally available. Prioritize incidents according to your preferred filters by creating filter sets and saving filter queries. Learn more about incident queue filters in [Available filters](incident-queue.md#available-filters).

- (GA) Microsoft Defender for Cloud alerts integration with Microsoft Defender XDR is now generally available. Learn more about the integration in [Microsoft Defender for Cloud in Microsoft Defender XDR](microsoft-365-security-center-defender-cloud.md).

- (GA) **Activity log** is now available within an incident page. Use the activity log to view all audits and comments, and add comments to the log of an incident. For details, see [Activity log](manage-incidents.md#view-the-activity-log-of-an-incident).

- (Preview) **[Query history](advanced-hunting-query-history.md) in advanced hunting** is now available. You can now rerun or refine queries you have run recently. Up to 30 queries in the past 28 days can be loaded in the query history pane.

- (Preview) Additional features you can use to **[drill down](advanced-hunting-query-results.md#drill-down-from-query-results)** further from your query results in advanced hunting are now available.

## December 2023

- **Microsoft Defender XDR Unified role-based access control (RBAC)** is now generally available. Unified (RBAC) allows administrators to manage user permissions across different security solutions from a single, centralized location. This offering is also available to GCC Moderate customers. To learn more, see [Microsoft Defender XDR Unified role-based access control (RBAC)](manage-rbac.md).

- Microsoft Defender Experts for XDR now lets you [exclude devices](get-started-xdr.md#exclude-devices-and-users-from-remediation) from remediation actions taken by our experts and instead get remediation guidance for those entities.

- The Microsoft Defender portal's incident queue has updated filters, search, and added a new function where you can create your own filter sets. For details, see [Available filters](incident-queue.md#available-filters).

- You can now assign incidents to a user group or another user. For details, see [Assign an incident](manage-incidents.md#assign-an-owner).

## November 2023

- Microsoft Defender Experts for Hunting now lets you generate sample Defender Experts Notifications so you can start experiencing the service without having to wait for an actual critical activity to happen in your environment. [Learn more](onboarding-defender-experts-for-hunting.md#generate-sample-defender-experts-notifications)

- (Preview) Microsoft Defender for Cloud alerts are now integrated in Microsoft Defender XDR. Defender for Cloud alerts are automatically correlated to incidents and alerts in the Microsoft Defender portal and cloud resource assets can be viewed in the incidents and alerts queues. Learn more about the [Defender for Cloud integration](microsoft-365-security-center-defender-cloud.md) in Microsoft Defender XDR.

- (Preview) Microsoft Defender XDR now has built in [deception technology](deception-overview.md) to protect your environment from high-impact attacks that use human-operated lateral movement. Learn more about the deception feature and how to [configure the deception feature](configure-deception.md).

- Microsoft Defender Experts for XDR now lets you perform your own [readiness assessment](get-started-xdr.md#prepare-your-environment-for-the-defender-experts-service) when preparing the environment for the Defender Experts for XDR service.

## October 2023

- (Preview) You can now get email notifications for manual or automated actions done in Microsoft Defender XDR. Learn how to configure email notifications for manual or automated response actions performed in the portal. For details, see [Get email notifications for response actions in Microsoft Defender XDR](m365d-response-actions-notifications.md).

- (Preview) [Microsoft Security Copilot in Microsoft Defender XDR](security-copilot-in-microsoft-365-defender.md) is now in preview. Microsoft Defender XDR users can take advantage of Security Copilot capabilities to summarize incidents, analyze scripts and codes, use guided responses to resolve incidents, generate KQL queries, and create incident reports within the portal. Security Copilot is on an invitation-only preview. Learn more about Security Copilot in the [Microsoft Security Copilot Early Access Program Frequently Asked Questions](/security-copilot/faq-security-copilot).

## September 2023

- (Preview) Custom detections using data from Microsoft Defender for Identity and Microsoft Defender for Cloud Apps, specifically the `CloudAppEvents`, `IdentityDirectoryEvents`, `IdentityLogonEvents`, and `IdentityQueryEvents` [tables](custom-detection-rules.md#tables-that-support-continuous-nrt-frequency) can now be run in near real-time [Continuous (NRT)](custom-detection-rules.md) frequency.

## August 2023

- Guides to responding to your first incident for new users are now live. [Understand incidents](respond-first-incident-365-defender.md) and learn to triage and prioritize, [analyze your first incident](respond-first-incident-analyze.md) using tutorials and videos, and [remediate attacks](respond-first-incident-remediate.md) by understanding actions available in the portal.

- (Preview) [Asset rule management - Dynamic rules for devices](./configure-asset-rules.md) is now in public preview. Dynamic rules can help manage device context by assigning tags and device values automatically based on certain criteria.

- (Preview) The [DeviceInfo](advanced-hunting-deviceinfo-table.md) table in advanced hunting now also includes the columns `DeviceManualTags` and `DeviceDynamicTags` in public preview to surface both manually and dynamically assigned tags related to the device you're investigating.

- The **Guided response** feature in Microsoft Defender Experts for XDR has been renamed to **[Managed response](managed-detection-and-response-xdr.md)**. We have also added a [new FAQ section](faq-incident-notifications-xdr.md#understanding-and-managing-defender-experts-for-xdr-incident-updates) on incident updates.

## July 2023

- (GA) The [Attack story](investigate-incidents.md#attack-story) in incidents is now generally available. The attack story provides the full story of the attack and allows incident response teams to view the details and apply remediation.

- A new URL and domain page is now available in Microsoft Defender XDR. The updated URL and domain page provides a single place to view all the information about a URL or a domain, including its reputation, the users who clicked it, the devices that accessed it, and emails where the URL or domain was seen. For details, see [Investigate URLs in Microsoft Defender XDR](/defender-endpoint/investigate-domain).

## June 2023

- (GA) Microsoft Defender Experts for XDR is now generally available. Defender Experts for XDR augments your security operations center by combining automation and Microsoft's security analyst expertise, helping you detect and respond to threats with confidence and improve your security posture. Microsoft Defender Experts for XDR is sold separately from other Microsoft Defender XDR products. If you're a Microsoft Defender XDR customer and are interested in purchasing Defender Experts for XDR, see [Overview of Microsoft Defender Experts for XDR](dex-xdr-overview.md).

## May 2023

- (GA) [Alert tuning](investigate-alerts.md#tune-an-alert) is now generally available. Alert tuning lets you fine-tune alerts to reduce investigation time and focus on resolving high priority alerts. Alert tuning replaces the Alert suppression feature.

- (GA) [Automatic attack disruption](automatic-attack-disruption.md) is now generally available. This capability automatically disrupts human-operated ransomware (HumOR), business email compromise (BEC), and adversary-in-the-middle (AiTM) attacks.

- (Preview) [Custom functions](advanced-hunting-custom-functions.md) are now available in advanced hunting. You can now create your own custom functions so you can reuse any query logic when you hunt in your environment.

## April 2023

- (GA) The [unified Assets tab in the Incidents page](investigate-incidents.md) is now generally available.

- Microsoft is using a new weather-based naming taxonomy for threat actors. This new naming schema will provide more clarity and will be easier to reference. [Learn more about the new threat actor taxonomy](microsoft-threat-actor-naming.md).

## March 2023

- (Preview) Microsoft Defender Threat Intelligence (Defender TI) is now available in the Microsoft Defender portal.

This change introduces a new navigation menu within the Microsoft Defender portal named **Threat Intelligence**. [Learn more](defender-threat-intelligence.md).

- (Preview) Complete device reports for the [`DeviceInfo` table](advanced-hunting-deviceinfo-table.md) in advanced hunting are now sent *every hour* (instead of the previous daily cadence). In addition, complete device reports are also sent whenever there's a change to any previous report. New columns were also added to the `DeviceInfo` table, along with several improvements to existing data in `DeviceInfo` and [DeviceNetworkInfo](advanced-hunting-devicenetworkinfo-table.md) tables.

- (Preview) Near real-time custom detection is now available for public preview in advanced hunting custom detections. There's a new [Continuous (NRT)](custom-detection-rules.md) frequency, which checks data from events as they're collected and processed in near real-time.

- (Preview) [Behaviors in Microsoft Defender for Cloud Apps](/defender-cloud-apps/behaviors) is now available for public preview. Preview customers can now also hunt for behaviors in advanced hunting using the [BehaviorEntities](advanced-hunting-behaviorentities-table.md) and [BehaviorInfo](advanced-hunting-behaviorinfo-table.md) tables.

## February 2023

- (GA) The [query resources report in advanced hunting](advanced-hunting-limits.md#view-query-resources-report-to-find-inefficient-queries) is now generally available.

- (Preview) The [automatic attack disruption](automatic-attack-disruption.md) capability now disrupts business email compromise (BEC).

## January 2023

- The new version of Microsoft Defender Experts for Hunting report is now available. The report's new interface now lets customers have more contextual details about the suspicious activities Defender Experts have observed in their environments. It also shows which suspicious activities have been continuously trending from month to month. For details, see [Understand the Defender Experts for Hunting report in Microsoft Defender XDR](defender-experts-report.md).

- (GA) Live Response is now generally available for macOS and Linux.

- (GA) Identity timeline is now generally available as part of the new Identity page in Microsoft Defender XDR. The updated User page has a new look, an expanded view of related assets and a new dedicated timeline tab. The timeline represents activities and alerts from the last 30 days. It unifies a user's identity entries across all available workloads: Microsoft Defender for Identity, Microsoft Defender for Cloud Apps, and Microsoft Defender for Endpoint. Using the timeline helps you easily focus on a user's activities (or activities performed on them) in specific timeframes.

## December 2022

- (Preview) The new Microsoft Defender XDR role-based access control (RBAC) model is now available for preview. The new RBAC model enables security admins to centrally manage privileges across multiple security solutions within a single system with a greater efficiency, currently supporting Microsoft Defender for Endpoint, Microsoft Defender for Office 365, and Microsoft Defender for Identity. The new model is fully compatible with the existing individual RBAC models currently supported in Microsoft Defender XDR. For more information, see [Microsoft Defender XDR role-based access control (RBAC)](./manage-rbac.md).

## November 2022

- (Preview) Microsoft Defender Experts for XDR (Defender Experts for XDR) is now available for preview. Defender Experts for XDR is a managed detection and response service that helps your security operations centers (SOCs) focus and accurately respond to incidents that matter. It provides extended detection and response for customers who use Microsoft Defender XDR workloads: Microsoft Defender for Endpoint, Microsoft Defender for Office 365, Microsoft Defender for Identity, Microsoft Defender for Cloud Apps, and Azure Active Directory (Azure AD). For details, refer to [Expanded Microsoft Defender Experts for XDR preview](dex-xdr-overview.md).

- (Preview) The query resource report is now available in advanced hunting. The report shows your organization's consumption of CPU resources for hunting based on queries that ran in the last 30 days using any of the hunting interfaces. See [View query resources report](advanced-hunting-limits.md#view-query-resources-report-to-find-inefficient-queries) to find inefficient queries.

## October 2022

- (Preview) The new automatic attack disruption capability is now in preview. This capability combines security research insights and advances AI models to automatically contain attacks in progress. Automatic attack disruption also provides more time to security operations centers (SOCs) to fully remediate an attack and limits an attack's impact to organizations. This preview automatically disrupts ransomware attacks.

## August 2022

- (GA) [Microsoft Defender Experts for Hunting](defender-experts-for-hunting.md) is now generally available. If you're a Microsoft Defender XDR customer with a robust security operations center but want Microsoft to help you proactively hunt for threats across endpoints, Office 365, cloud applications, and identity using Microsoft Defender data, then learn more about applying, setting up, and using the service. Defender Experts for Hunting is sold separately from other Microsoft Defender XDR products.

- (Preview) [Guided mode](advanced-hunting-modes.md#get-started-with-guided-hunting-mode) is now available for public preview in advanced hunting. Analysts can now start querying their database for endpoint, identities, email & collaboration, and cloud apps data *without knowing Kusto Query Language (KQL)*. Guided mode features a friendly, easy-to-use, building-block style of constructing queries through dropdown menus containing available filters and conditions. See [Get started with query builder](advanced-hunting-query-builder.md).

## July 2022

- (Preview) Microsoft Defender Experts for Hunting public preview participants can now look forward to receiving monthly reports to help them understand the threats the hunting service surfaced in their environment, along with the alerts generated by their Microsoft Defender XDR products. For details, refer to [Understand the Defender Experts for Hunting report in Microsoft Defender XDR](defender-experts-report.md).

## June 2022

- (Preview) The [DeviceTvmInfoGathering](advanced-hunting-devicetvminfogathering-table.md) and [DeviceTvmInfoGatheringKB](advanced-hunting-devicetvminfogatheringkb-table.md) tables are now available in the advanced hunting schema. Use these tables to hunt through assessment events in Defender Vulnerability Management including the status of various configurations and attack surface area states of devices.

- The newly introduced Automated investigation & response card in the Microsoft Defender portal provides an overview on pending remediation actions.

The security operations team can view all actions pending approval, and the stipulated time to approve those actions in the card itself. The security team can quickly navigate to the Action center and take appropriate remediation actions. The Automated investigation & response card also has a link to the Full Automation page. This enables the security operations team to effectively manage alerts and complete remediation actions in a timely manner.

## May 2022

- (Preview) In line with the recently announced expansion into a new service category called [Microsoft Security Experts](https://aka.ms/MicrosoftSecurityExperts), we're introducing the availability of [Microsoft Defender Experts for Hunting](defender-experts-for-hunting.md) (Defender Experts for Hunting) for public preview. Defender Experts for Hunting is for customers who have a robust security operations center but want Microsoft to help them proactively hunt for threats across Microsoft Defender data, including endpoints, Office 365, cloud applications, and identity.

## April 2022

- (Preview) [Actions](advanced-hunting-take-action.md) can now be taken on email messages straight from hunting query results. Emails can be moved to other folders or deleted permanently.

- (Preview) The new [`UrlClickEvents` table](advanced-hunting-urlclickevents-table.md) in advanced hunting can be used to hunt for threats like phishing campaigns and suspicious links based on information coming from Safe Links clicks in email messages, Microsoft Teams, and Office 365 apps.

## March 2022

- (Preview) The incident queue has been enhanced with several features designed to help your investigations. Enhancements include capabilities such as ability to search for incidents by ID or name, specify a custom time range, and others.

## December 2021

- (GA) The `DeviceTvmSoftwareEvidenceBeta` table was added on a short-term basis in advanced hunting to allow you to view evidence of where a specific software was detected on a device.

## November 2021

- (Preview) The application governance add-on feature to Defender for Cloud Apps is now available in Microsoft Defender XDR. App governance provides a security and policy management capability designed for OAuth-enabled apps that access Microsoft 365 data through Microsoft Graph APIs. App governance delivers full visibility, remediation, and governance into how these apps and their users access, use, and share your sensitive data stored in Microsoft 365 through actionable insights and automated policy alerts and actions. [Learn more about application governance](/cloud-app-security/app-governance-manage-app-governance).

- (Preview) The [advanced hunting](advanced-hunting-overview.md) page now has multitab support, smart scrolling, streamlined schema tabs, quick edit options for queries, a query resource usage indicator, and other improvements to make querying smoother and easier to fine-tune.

- (Preview) You can now use the [link to incident](advanced-hunting-link-to-incident.md) feature to include events or records from the advanced hunting query results right into a new or existing incident that you're investigating.

## October 2021

- (GA) In advanced hunting, more columns were added in the [CloudAppEvents](advanced-hunting-cloudappevents-table.md) table. You can now include `AccountType`, `IsExternalUser`, `IsImpersonated`, `IPTags`, `IPCategory`, and `UserAgentTags` to your queries.

## September 2021

- (GA) Microsoft Defender for Office 365 event data is available in the Microsoft Defender XDR event streaming API. You can see the availability and status of event types in the [Supported Microsoft Defender XDR event types in streaming API](supported-event-types.md).

- (GA) Microsoft Defender for Office 365 data available in advanced hunting is now generally available.

- (GA) Assign incidents and alerts to user accounts

  You can assign an incident, and all the alerts associated with it, to a user account from **Assign to:** on the **Manage incident** pane of an incident or the **Manage alert** pane of an alert.

## August 2021

- (Preview) Microsoft Defender for Office 365 data available in advanced hunting

  New columns in email tables can provide more insight into email-based threats for more thorough investigations using advanced hunting. You can now include the `AuthenticationDetails` column in [EmailEvents](./advanced-hunting-emailevents-table.md), `FileSize` in [EmailAttachmentInfo](./advanced-hunting-emailattachmentinfo-table.md), and `ThreatTypes` and `DetectionMethods` in [EmailPostDeliveryEvents](./advanced-hunting-emailpostdeliveryevents-table.md) tables.

- (Preview) Incident graph

  A new **Graph** tab on the **Summary** tab of an incident shows the full scope of the attack, how the attack spread through your network over time, where it started, and how far the attacker went.

## July 2021

- [Professional services catalog](https://sip.security.microsoft.com/interoperability/professional_services)

  Enhance the detection, investigation, and threat intelligence capabilities of the platform with supported partner connections.

## June 2021

- (Preview) [View reports per threat tags](threat-analytics.md#view-reports-by-category)

  Threat tags help you focus on specific threat categories and review the most relevant reports.

- (Preview) [Streaming API](/defender-endpoint/api/raw-data-export)

  Microsoft Defender XDR supports streaming all the events available through Advanced Hunting to an Event Hubs and/or Azure storage account.

- (Preview) [Take action in advanced hunting](advanced-hunting-take-action.md)

  Quickly contain threats or address compromised assets that you find in [advanced hunting](advanced-hunting-overview.md).

- (Preview) [In-portal schema reference](advanced-hunting-schema-tables.md#get-schema-information-in-the-security-center)

  Get information about advanced hunting schema tables directly in the security center. In addition to table and column descriptions, this reference includes supported event types (`ActionType` values) and sample queries.

- (Preview) [DeviceFromIP() function](advanced-hunting-devicefromip-function.md)

  Get information about which devices have been assigned a specific IP address or addresses at a given time range.

## May 2021

- [New alert page in the Microsoft Defender portal](https://techcommunity.microsoft.com/t5/microsoft-365-defender/easily-find-anomalies-in-incidents-and-alerts/ba-p/2339243)

  Provides enhanced information for the context into an attack. You can see which other triggered alert caused the current alert and all the affected entities and activities involved in the attack, including files, users, and mailboxes. See [Investigate alerts](investigate-alerts.md) for more information.

- [Trend graph for incidents and alerts in the Microsoft Defender portal](https://techcommunity.microsoft.com/t5/microsoft-365-defender/new-alert-page-for-microsoft-365-defender-incident-detections/ba-p/2350425)

  Determine if there are several alerts for a single incident or that your organization is under attack with several different incidents. See [Prioritize incidents](incident-queue.md) for more information.

## April 2021

- Microsoft Defender XDR

  The improved [Microsoft Defender XDR](https://security.microsoft.com) portal is now available. This new experience brings together Defender for Endpoint, Defender for Office 365, Defender for Identity, and more into a single portal. This is the new home to manage your security controls. [Learn what's new](microsoft-365-defender-portal.md).

- [Microsoft Defender XDR threat analytics report](threat-analytics.md)

  Threat analytics helps you respond to and minimize the impact of active attacks. You can also learn about attack attempts blocked by Microsoft Defender XDR solutions and take preventive actions that mitigate the risk of further exposure and increase resiliency. As part of the unified security experience, threat analytics is now available for Microsoft Defender for Endpoint and Microsoft Defender for Office E5 license holders.

## March 2021

- [CloudAppEvents table](advanced-hunting-cloudappevents-table.md)

  Find information about events in various cloud apps and services covered by Microsoft Defender for Cloud Apps. This table also includes information previously available in the `AppFileEvents` table.

[!INCLUDE [Microsoft Defender XDR rebranding](../includes/defender-m3d-techcommunity.md)]
