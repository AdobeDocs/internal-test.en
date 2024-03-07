---
title: Deprecated and Removed Features
description: Release notes specific to deprecated and removed features in [!DNL Adobe Experience Manager] as a [!DNL Cloud Service].
exl-id: 34c096e3-8256-4996-95c9-0daee3c94db9
---
# Deprecated and Removed Features {#deprecated-and-removed-features}

<!--
>[!CONTEXTUALHELP]
>id="aem_cloud_deprecated_features"
>title="Deprecated and Removed Features in AEM as a Cloud Service"
>abstract="AEM as a Cloud Service has a cloud-native deployment model. Certain capabilities and features have been repalced by cloud-native counterparts and this tab shows those features." 
-->

Adobe constantly evaluates product capabilities, to over time reinvent or replace older features with more modern alternatives to improve overall customer value, always under careful consideration of backward compatibility. Also, as [!DNL Adobe Experience Manager] as a [!DNL Cloud Service] provides a cloud-native deployment model, certain capabilities and features were replaced by cloud-native counterparts.

To communicate the impending removal/replacement of [!DNL Experience Manager] capabilities, the following rules apply:

1. Announcement of deprecation comes first. Deprecated capabilities remain available but are not enhanced further.
1. Capabilities announced to be deprecated are removed in the subsequent major release, at the earliest. The actual target date for removal is announced.

This process gives customers at least one release cycle to adapt their implementation to a new version or successor of a deprecated capability, before actual removal.

## Deprecated Features {#deprecated-features}

This section lists features and capabilities that have been marked as deprecated in [!DNL Experience Manager] as a [!DNL Cloud Service]. Typically, features to be removed in a future release are set to deprecated first, with an alternative provided.

Customers are advised to review if they use the feature/capability in their current deployment, and make plans to change their implementation to use the alternative provided.

| Capabilities | Deprecated feature | Replacement |
| ------------ | ------------------ | ----------- |
| [!DNL Sites]       | Experience Fragments properties for **Social Media Status**. | The feature will be removed soon. |
| [!DNL Sites]       | Template-based simple content fragments. | [Model-based structured content fragments](newfile.md) now. |
| [!DNL Assets]       | `DAM Asset Update` workflow to process ingested images. | Asset ingestion uses [asset microservices](newfile.md) now. |
| [!DNL Assets]       | Upload assets directly to [!DNL Experience Manager]. See [deprecated asset upload APIs](newfile.md). For technical details, see [direct upload APIs](newfile.md). |
| [!DNL Assets]       | [Certain workflow steps](newfile.md) provide a replacement for many workflows. For custom processing, use [post-processing workflows](newfile.md). |
| [!DNL Assets]       | FFmpeg transcoding of videos. | For FFmpeg thumbnail generation, use [Asset microservices](newfile.md). For FFmpeg transcoding, use [Dynamic Media](newfile.md). |
| [!DNL Foundation]       | Tree replication UI under the replication agent's "Distribute" tab (removal after September 30, 2021) | [Manage publication](newfile.md) or [publish content tree workflow](newfile.md) approaches |

## Removed Features {#removed-features}

This section lists features and capabilities that have been removed from [!DNL Experience Manager] with [!DNL Experience Manager] as a [!DNL Cloud Service].

| Area         | Feature            | Replacement | Target Removal Date |
| ------------ | ------------------ | ----------- | ------------------- |
| User Interface  | Classic UI is removed from the product user interface. A few Classic UI dialogs are available for a few select capabilities, such as Link Checker, Version Purge, and some Cloud Service configurations. Upcoming [product updates](newfile.md) may further remove Classic UI availability. | Standard UI  | Removed |
| [!DNL Dynamic Media] | Previous integrations with [Dynamic Media Classic](https://experienceleague.adobe.com/docs/experience-manager-65/administering/integration/scene7.html#integration) and [Dynamic Media Hybrid mode](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dynamic.html#dynamic) are not available in [!DNL Experience Manager] as a [!DNL Cloud Service]. | Use [Dynamic Media](newfile.md) provided with [!DNL Experience Manager] as a [!DNL Cloud Service]. | Removed |
| [!DNL Sites] | Portal Director and Portlet Component | These capabilities were deprecated in [!DNL Experience Manager] 6.4 and have now been removed from [!DNL Experience Manager].| Removed |
| [!DNL Sites] | Design Importer | This capability has been removed as immutable sections of the [!DNL Experience Manager] repository are not accessible at runtime. | Removed |
| [!DNL Assets] | [!DNL Assets] sharing with Marketing Cloud Assets Core Service and Creative Cloud services is not available. | For integration with [!DNL Adobe Creative Cloud], use [Adobe Asset Link](https://helpx.adobe.com/enterprise/using/adobe-asset-link.html). | Removed |
| [!DNL Foundation]       | Support for Apache Sling datasources (OSGi bundle org.apache.sling.datasource) | N/A | Removed |
| [!DNL Foundation]       | Suppport for JST scripting templates (OSGi bundle org.apache.sling.scripting.jst) | N/A | Removed |
| [!DNL Foundation]       | Support for the Apache Felix Http Whiteboard | OSGi Http Whiteboard | March 2022 |

## Unsupported Versions {#unsupported-versions}

This section lists bundle versions that are unsupported in [!DNL AEM as a Cloud Service].

<table style="table-layout:auto">
<thead>
  <tr>
    <th>Bundle Name(s)</th>
    <th>Unsupported Versions</th>
    <th>Target Enforcement Date</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>com.adobe.acs:acs-aem-commons-bundle<br>com.adobe.acs:acs-aem-commons-ui.content<br>com.adobe.acs:acs-aem-commons-ui.apps</td>
    <td>Versions below <b>5.0.10</b> are unsupported</td>
    <td>Enforced</td>
  </tr>
  <tr>
    <td>org.apache.servicemix.bundles:org.apache.servicemix.bundles.fop</td>
    <td>Versions below <b>2.5.1</b> are unsupported</td>
    <td>2/24/22</td>
  </tr>
</tbody>
</table>

## Java API {#java-api}

See [this page](newfile.md) for any deprecated or removed Java APIs, which are occasionally introduced.

## OSGI Configuration {#osgi-configuration}

See [this article](newfile.md) for any restrictions around configuration of OSGI properties, some of which may be introduced over time.
