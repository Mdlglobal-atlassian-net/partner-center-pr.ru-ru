---
title: Common billing scenarios for license-based SaaS transactions | Partner Center
ms.topic: article
ms.date: 11/21/2019
description: Common billing scenarios in Partner Center for license-based SaaS transactions.
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
Keywords: billing, payments, one-time purchase, recurring purchase, subscriptions, seats
ms.localizationpriority: medium
ms.openlocfilehash: b808a3bbfc0856e03f1c775d7e3145a29c2239fb
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389612"
---
# <a name="billing-scenarios-for-license-based-saas-transactions"></a>Billing scenarios for license-based SaaS transactions

These example [common billing scenarios](common-billing-scenarios.md) are applicable to license-based software as a service (SaaS) subscriptions in Partner Center.

## <a name="convert-a-free-trial-saas-subscription-to-a-paid-subscription"></a>Convert a free trial SaaS subscription to a paid subscription

This scenario describes billing for the renewal of a license-based free trial SaaS subscription. The renewal converts the free trial to a paid subscription at the end of the free trial period.

In this example, you purchased a free trial of a license-based SaaS (software as a service) subscription on June 10th. This free trial automatically renewed as a paid subscription when the free trial period ends.

The recon files will include the following charges:

| Дата покупки | Charge start date | Charge end date | Цена за единицу | Unit quantity | Total amount | Тип оплаты | Subscription description |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | 0 долл. США | 1 | 0 долл. США | Новый | Бесплатная пробная версия |
| 07/10/2019 | 07/10/2019 | 08/09/2019 | 2 долл. США | 1 | 2 долл. США | "Продлить" | Paid subscription |

## <a name="cancel-a-free-trial-saas-subscription"></a>Cancel a free trial SaaS subscription

> [!TIP]
> You can cancel a license-based free trial SaaS subscription any time, even during the free trial period.

In this scenario, you purchased a license-based free trial SaaS subscription on July 1st, and then canceled it immediately in Partner Center. 

The recon file will include the following charges:

| Дата покупки | Charge start date | Charge end date | Цена за единицу | Unit quantity | Total amount | Тип оплаты | Subscription description |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | 0 долл. США | 11 | 0 долл. США | Новый | Бесплатная пробная версия |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | 0 долл. США | 11 | 0 долл. США | "Отмена" | Бесплатная пробная версия |

## <a name="convert-custom-meter-saas-subscription-to-another-sku"></a>Convert custom meter SaaS subscription to another SKU

This scenario describes how to convert a custom meter SaaS subscription from one stock keeping unit (SKU) to another SKU for the same product, on the same date.

In this scenario, you purchased one SKU (Silver) under a product and converted it to another available SKU (Bronze) under this product on the same date.

The recon file will include the following charges:

| Дата покупки | Charge start date | Charge end date | Цена за единицу | Unit quantity | Total amount | Тип оплаты | Subscription description |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | Уровень Silver | 06/10/2019 | 06/10/2019 | 20 долл. США | 1 | 20 долл. США | Новый | Custom meter SaaS subscription |
| 06/10/2019 | Уровень Silver | 06/10/2019 | 06/10/2019 | 20 долл. США | 1 | -$20 | Преобразование | Prorated rebill for custom meter SaaS subscription |
| 06/10/2019 | Bronze | 06/10/2019 | 06/10/2019 | 10 долл. США | 1 | 10 долл. США | Преобразование | Custom meter SaaS subscription |

## <a name="purchase-and-cancel-a-customer-meter-saas-subscription-on-same-date"></a>Purchase and cancel a customer meter SaaS subscription on same date

This scenario describes billing for a customer meter SaaS subscription that you purchased and cancelled through the Azure portal on the same date.

In this scenario, you purchased a custom meter SaaS subscription on the Azure portal. Then, you canceled the subscription on the same date.

| Дата покупки | Charge start date | Charge end date | Цена за единицу | Unit quantity | Total amount | Тип оплаты | Subscription description |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | Bronze | 06/10/2019 | 06/10/2019 | 10 долл. США | 1 | 10 долл. США | Новый | Custom meter SaaS subscription |
| 06/10/2019 | Bronze | 06/10/2019 | 06/10/2019 | 10 долл. США | 1 | -$10 | CancelImmediate | Custom meter SaaS subscription |
