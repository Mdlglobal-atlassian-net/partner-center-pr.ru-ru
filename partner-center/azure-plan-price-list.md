---
title: Прейскурант планов Azure | Центр партнеров
ms.topic: article
ms.date: 10/15/2019
description: Как просмотреть прейскурант на подписки в плане Azure
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: high
ms.openlocfilehash: 64f7b6930f31afc63397ae3ed0e0dba2357b0f1e
ms.sourcegitcommit: cd90a59ff0ea81197b603abcb7bf462c4fb1edbe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2019
ms.locfileid: "72171277"
---
# <a name="price-list-for-the-new-commerce-experience-in-csp-for-azure"></a>Прейскурант для новой коммерческой модели в CSP для Azure 

Прейскурант для нового интерфейса Azure Commerce в CSP опубликован в Центре партнеров. Прейскурант динамически в режиме реального времени формируется в виде файла, цены в котором отображаются только в долларах США. Однако выставление счетов осуществляется в поддерживаемой валюте, действующей в расположении для валюты клиента. Дополнительные сведения о выставлении счетов в валюте клиента см. в статье [План Azure. Выставление счетов](azure-plan-billing.md).

## <a name="see-pricing-for-subscriptions-under-the-azure-plan-pricing"></a>Цены на подписки см. в разделе цен на план Azure.

1. В меню центра партнеров слева выберите **Sell** (Продажа), а затем выберите **Marketplace**.

2. Рядом с полем **Export type** выберите **Azure plan consumption pricing** (Цены на использование плана Azure).

3. Рядом с полем **Pricing for date** (Цены на дату) выберите нужную дату, например, **Current** (Текущая дата). Примечание. Вы также можете выбрать **FX rates** (Валютный курс) для экспорта текущего курса валют.

![Цены на Azure 2](images/azure/pricelist2.jpg)

4. В разделе **Marketplace** выберите параметры **Type** (Тип) и **Category** (Категория) продукта или выполните поиск продукта. Отобразятся доступные продукты в результатах поиска.

![pricing](images/azure/Azurepricelist1.jpg)

5. Выберите **Export Azure plan price list** (Экспортировать прейскурант для планов Azure), чтобы загрузить цены на планы Azure для выбранных продуктов.


![экспорт прейскуранта](images/azure/pricelist1.png)



## <a name="azure-price-list-specifics"></a>Характеристики прейскурантов для Azure

- Цены на план Azure будут доступны на странице Marketplace в Центре партнеров в разделе **Sell** (Продажа).

- Функция экспорта будет доступна для служб использования плана Azure, резервирования Azure и курса валют.

- Параметры экспорта:

    - **Цены на сегодняшний день**: Сюда входят все счетчики и цены с 1-го числа месяца до текущей даты текущего месяца. Сюда входят новые цены, измененные цены или удаленные цены. Для всех цен будут указаны даты начала и окончания, чтобы показать, являются ли они новыми или удаленными.

    - **Цены за предыдущий месяц**: Загрузка ресурсов каждого типа будет выполняться по месяцам. Файлы цен будут содержать все счетчики, которые были доступны в течение этого месяца. Если новый счетчик появился в середине месяца, он будет показан как счетчик с действующей датой, отражающей его доступность. Аналогично цены, которые не поддерживаются, отображаются с указанием эффективной датой окончания, когда они становятся недоступны.

    - **Валютный курс**. Валютные курсы будут доступны для загрузки за день до 1-го дня месяца, в 18:00 по тихоокеанскому стандартному времени. Например, если вы хотите получить сведения о курсах за ноябрь, загружайте курсы 31 октября. Курсы валют за предыдущий месяц также доступны.

    - **Соответствующие службы**. Полученный от партнера кредит действует для служб, перечисленным в документе **Azure plan consumption pricing** (Цены на использование плана Azure), которые партнеры могут экспортировать на странице цен на планы Azure. Обратите внимание на то, что существуют исключения, включая, помимо прочего, резервирования сторонних поставщиков и резервирование Azure.

- Цены в прейскурантах являются прямыми ценами. Некоторые партнеры могут иметь право на кредиты, полученные от партнеров. Сведения о том, как рассчитывается кредит, полученный от партнера, читайте в статье [How the partner earned credit is calculated and paid](partner-earned-credit-explanation.md) (Как рассчитывается и оплачивается кредит, полученный от партнера).


## <a name="price-list-data"></a>Данные прейскуранта

|**Поле**   |**Описание**   |
|--------------------------|:---------------------------|
|ProductTitle  |Название или имя продукта|
|ProductID   |Идентификатор продукта|
|SKuId|Идентификатор номера SKU|
|SkuTitle|Название или имя номера SKU|
|Издатель|Первой стороной всегда будет корпорация Майкрософт|
|SkuDescription|Описание номера SKU|
|UnitOfMeasure|Единицы, которые будут оплачиваться или за которые будут выставляться счета|
|TermDuration|Для продуктов во временном использовании — продолжительность времени, применимая к резервированиям.|
|Рынок|Рынок цен|
|Валюта|Валюта цен|
|UnitPrice|Цена за единицу|
|PricingTierRangeMin|Для многоуровневых цен применяется минимальная цена|
|PricingTierRangeMax|Для многоуровневых цен применяется максимальная цена|
|EffectiveStartDate|Дата начала действия цены|
|EffectiveEndDate|Дата окончания действия цены|
|MeterIds|Идентификатор счетчика номера SKU продукта|
|MeterType|Тип счетчика|
|Теги|Свойства продукта. Для цен на план Azure это будет "Azure" или "Azure и Резервирования" (в частности, для резервирований).|

Подробные сведения о прейскуранте см. [здесь](https://partner.microsoft.com/commerce/sales?type=Any&category=Any).  