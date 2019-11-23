---
title: Daily-rated usage reconciliation files | Partner Center
ms.topic: article
ms.date: 11/21/2019
description: Understand daily-rated usage reconciliation files in Partner Center.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 896f81b3a51e234065af7779d287b4023dd7163c
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389702"
---
# <a name="daily-rated-usage-reconciliation-files"></a>Daily-rated usage reconciliation files

Область применения

- Центр партнеров
- Центр партнеров для Microsoft Cloud for US Government

This topic explains how to read daily-rated usage reconciliation files.

## <a name="fields-in-daily-rated-usage-reconciliation-files"></a>Fields in daily-rated usage reconciliation files

| Column | Описание |
| ------ | ----------- |
| PartnerId | Partner identifier in GUID format. |
| PartnerName | Partner name. |
| CustomerId | Unique Microsoft identifier for the customer in GUID format. |
| CustomerCompanyName | Имя организации клиента, указанное в Центре партнеров. *This column is very important for reconciling the invoice with your system information.* |
| CustomerDomainName | The customer's domain name. Not available for current activity. |
| Customer country | Страна, в которой находится клиент. |
| MPNID | MPN identifier of the CSP partner. |
| Reseller MPNID | MPN identifier of the reseller of record for the subscription. Not available for current activity. |
| InvoiceNumber | Номер счета-фактуры, содержащего указанную транзакцию. Not available for current activity. |
| ProductID | The identifier for the product. |
| SkuId | The identifier for a particular SKU. |
| AvailabilityId | The identifier for a particular SKU's availability. This shows whether the SKU is available for purchase in the given country, currency, industry segment, etc. |
| SKU Name | Название для определенного номера SKU. |
| PublisherName | The name of the publisher. |
| PublisherID | The identifier of the publisher in GUID format. Not available for current activity. |
| Subscription Description | Имя предложения службы, приобретенной клиентом, как указано в прейскуранте. (This is an identical field to **OfferName**). |
| Код подписки | Уникальный идентификатор подписки в платформе выставления счетов Майкрософт. Not used for reconciliation. *This identifier is not the same as the **Subscription ID** on the partner admin console.* |
| ChargeStartDate | Start date of the billing cycle (except when presenting dates of previously uncharged latent usage data from the previous billing cycle). Временем всегда является начало дня, 0:00. |
| ChargeEndDate | End date of billing cycle (except when presenting dates of previously uncharged latent usage data from the previous biling cycle). Временем всегда является конец дня, 23:59. |
| Usage Date | Date of service usage. |
| Meter Type | The type of meter. |
| Meter Category | The top-level service for the usage. |
| Meter Id | The identifier for the meter being used. |
| Meter Sub-category | The type of Azure service, which can affect the rate. |
| Meter Name | The unit of measure for the meter being consumed. |
| Meter Region | Этот столбец определяет местоположение центра обработки данных региона для служб, где это применимо и заполняется. |
| Unit | The unit of the resource **Name**. |
| Consumed Quantity | The amount of service consumed (such as *hours* or *GB*) during the reporting period. Includes any unbilled usage from previous reporting periods. |
| Resource Location | >The data center where the meter is running. |
| Consumed Service | The Azure platform service that you used. |
| Resource URI | The URI of the resource being used. |
| Тип оплаты | Тип оплаты или корректировки. Not available for current activity. |
| Цена за единицу | Price per license, as published in the price list at the time of purchase. Make sure this price matches the information stored in your billing system during reconciliation. |
| Количество | Number of licenses. Make sure this price matches the information stored in your billing system during reconciliation. |
| Unit type | The type of unit the meter is charged in. Not available for current activity. |
| Billing pre tax | Total billing amount before taxes. |
| Billing currency | The currency in the customer's geographic region. |
| Pricing pretax total | The pricing before taxes are added. |
| Pricing currency | The currency in the price list. |
| Service Info 1 | The number of Service Bus connections that were provisioned and utilized on a given day. |
| Service Info 2 | A legacy field that captures optional service-specific metadata. |
| Additional Info | Any additional information not covered in other columns. |
