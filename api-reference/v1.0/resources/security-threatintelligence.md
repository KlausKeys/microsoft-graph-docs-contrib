---
title: "threatIntelligence resource type"
description: "Provides APIs to retrieve threat intelligence information, such as about a host or an article on a threat."
author: "joerattazzi-microsoft"
ms.localizationpriority: medium
ms.prod: "security"
doc_type: resourcePageType
---

# threatIntelligence resource type

Namespace: microsoft.graph.security

[!INCLUDE [threatintelligence-api-disclaimer](../../includes/threatintelligence-api-disclaimer.md)]

Provides APIs to retrieve threat intelligence information, such as about a host or an article on a threat.

The Microsoft Graph threat intelligence API delivers world-class threat intelligence to help protect your organization from modern cyber threats. Using threat intelligence APIs, you can identify adversaries and their operations, accelerate detection and remediation, and enhance your security investments and workflows.

The threat intelligence API allows you to operationalize intelligence found within the user interface. This includes finished intelligence in the forms of articles and intel profiles, machine intelligence including indicators of compromise (IoCs) and reputation verdicts, and finally, enrichment data including passive DNS, cookies, components, and trackers.

## Methods

| Method                                                                            | Return type                                                                                                               | Description                                                                                |
| :-------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------ | :----------------------------------------------------------------------------------------- |
| [List articles](../api/security-article-list.md)                                  | [microsoft.graph.security.article](../resources/security-article.md) collection                                           | Get a list of **article** objects, including their properties and relationships.           |
| [List intelProfiles](../api/security-intelligenceprofile-list.md)                 | [microsoft.graph.security.intelligenceProfile](../resources/security-intelligenceprofile.md) collection                   | Get a list of **intelligenceProfile** resources.                                           |
|[List sslCertificates](../api/security-sslcertificate-list.md)|[microsoft.graph.security.sslCertificate](../resources/security-sslcertificate.md) collection |Get a list of [sslCertificate](../resources/security-sslcertificate.md) objects and their properties.|
| [List whoisRecords](../api/security-whoisrecord-list.md)                     |[microsoft.graph.security.whoisRecord](../resources/security-vulnerability.md) |Get a list of [whoisRecord](../resources/security-whoisrecord.md) objects.|

## Properties

None.

## Relationships

| Relationship           | Type                                                                                                                      | Description                                                                                                                                                                                                    |
|:---|:---|:---|
|articleIndicators|[microsoft.graph.security.articleIndicator](../resources/security-articleindicator.md) collection|Refers to indicators of threat or compromise highlighted in an [article](../resources/security-article.md).<br/>**Note**: List retrieval is not yet supported.|
| articles               | [microsoft.graph.security.article](../resources/security-article.md) collection                                           | A list of **article** objects.                                                                                                                                                                                 |
|hostComponents|[microsoft.graph.security.hostComponent](../resources/security-hostcomponent.md) collection|Retrieve details about [hostComponent](../resources/security-hostcomponent.md) objects.<br/>**Note**: List retrieval is not yet supported.|
|hostCookies|[microsoft.graph.security.hostCookie](../resources/security-hostcookie.md) collection|Retrieve details about [hostCookie](../resources/security-hostcookie.md) objects.<br/>**Note**: List retrieval is not yet supported.|
|hostPairs|[microsoft.graph.security.hostPair](../resources/security-hostpair.md) collection|Retrieve details about [hostTracker](../resources/security-hostpair.md) objects.<br/>**Note**: List retrieval is not yet supported.|
|hostSslCertificates| [microsoft.graph.security.hostSslCertificate](../resources/security-hostsslcertificate.md) collection |Retrieve details about [hostSslCertificate](../resources/security-hostsslcertificate.md) objects.<br/>**Note**: List retrieval is not yet supported.|          
|hostTrackers|[microsoft.graph.security.hostTracker](../resources/security-hosttracker.md) collection|Retrieve details about [hostTracker](../resources/security-hosttracker.md) objects.<br/>**Note**: List retrieval is not yet supported.|
|hosts|[microsoft.graph.security.host](../resources/security-host.md) collection|Refers to [host](../resources/security-host.md) objects that Microsoft Threat Intelligence has observed.<br/>**Note**: List retrieval is not yet supported.|
|intelProfileIndicators|[microsoft.graph.security.intelligenceProfileIndicator](../resources/security-intelligenceprofileindicator.md) collection|Refers to indicators of threat or compromise highlighted in an [intelligenceProfile](../resources/security-intelligenceprofile.md).<br/>**Note**: List retrieval is not yet supported.|
| intelProfiles          | [microsoft.graph.security.intelligenceProfile](../resources/security-intelligenceprofile.md) collection                   | A list of **intelligenceProfile** objects.                                                                                                                                                                     |
|passiveDnsRecords|[microsoft.graph.security.passiveDnsRecord](../resources/security-passivednsrecord.md) collection|Retrieve details about [passiveDnsRecord](../resources/security-passivednsrecord.md) objects.<br/>**Note**: List retrieval is not yet supported.|
|sslCertificates| [microsoft.graph.security.sslCertificate](../resources/security-sslcertificate.md) collection |Retrieve details about [sslCertificate](../resources/security-sslcertificate.md) objects.<br/>**Note**: List retrieval is not yet supported.|         
|subdomains|[microsoft.graph.security.subdomain](../resources/security-subdomain.md) collection|Retrieve details about the [subdomain](../resources/security-subdomain.md).<br/>**Note**: List retrieval is not yet supported.|
|vulnerabilities|[microsoft.graph.security.vulnerability](../resources/security-vulnerability.md) collection|Retrieve details about [vulnerabilities](../resources/security-vulnerability.md).<br/>**Note**: List retrieval is not yet supported.                                                                       |
|whoisHistoryRecords|[microsoft.graph.security.whoisHistoryRecord](../resources/security-whoishistoryrecord.md) collection|Retrieve details about [whoisHistoryRecord](../resources/security-whoishistoryrecord.md) objects.<br/>**Note:** List retrieval is not yet supported.|
|whoisRecords|[microsoft.graph.security.whoisRecord](../resources/security-whoisrecord.md) collection|A list of [whoisRecord](../resources/security-whoisrecord.md) objects.|

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.threatIntelligence",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.security.threatIntelligence"
}
```
