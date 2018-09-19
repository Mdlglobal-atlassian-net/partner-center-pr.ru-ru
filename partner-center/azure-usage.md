---
title: Размеры виртуальных Машин Microsoft Azure для максимального использования резервирования | Информационная панель центра партнеров
Description: Information on purchasing and managing Azure reservations
author: v-petand
keywords: azure, резервирования, виртуальная машина, управление, использование, размеры
ms.localizationpriority: medium
ms.openlocfilehash: bb7d022ba45462db313a9f4e16cc47e4550dbef6
ms.sourcegitcommit: 92629114d5081103bfe555081f69997af4ed56f2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2018
ms.locfileid: "2875784"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a>Размеры виртуальных машин Microsoft Azure для максимального использования резервирования 

**Область применения**

-  Информационная панель центра партнеров
-  Портал Azure
-  Партнеры по программе CSP

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>Определение размера виртуальных машин для резервирования Azure клиента 

При приобретении резервирований Microsoft Azure для клиентов необходимо выбрать размер виртуальной машины (VM), соответствующий требованиям клиента к вычислительной мощности. Эту информацию можно получить одним из следующих способов:

-   API использования Azure
-   Портал Azure
-   Azure PowerShell
-   API для Azure Resource Manager (ARM)

Ниже приведены инструкции по каждому из этих методов. После приобретения резервирования скидка на резервирование автоматически применяется к виртуальным машинам, которые соответствуют атрибутам и количеству резервирования. Назначать резервирование виртуальной машине не требуется.

>[!NOTE]
>Скидки на резервирование не распространяются на классические и рекламные виртуальные машины.

>[!IMPORTANT]
>Чтобы правильно определить тип и размер виртуальной машины, приобретаемой от лица клиента, воспользуйтесь одним из указанных методов. Помните, что тип серии виртуальной машины неправильно отображается в файлах выверки в Центре партнеров.


**Получение сведений о размере виртуальной машины с помощью API использования Azure**

1.  Используйте значение атрибута ServiceType из additionalInfo в ответе API, чтобы определить нужный размер виртуальной машины. 

2.  Дополнительные сведения см. в разделе [Получение статистики клиента для Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) на [информационной панели центра партнеров API](https://docs.microsoft.com/partner-center/develop/). 

**Получение сведений о размере виртуальной машины на портале Microsoft Azure**

1.  В информационной панели для партнеров перейдите к странице " **Клиенты** ".

2.  Найдите клиента, желающего приобрести резервирования Azure, затем выберите стрелку вниз, чтобы посмотреть сведения о клиенте. Выберите **Портал управления Microsoft Azure**, чтобы открыть запись клиента на портале Azure. 

3.  Выберите пункт **Виртуальные машины** в меню портала, затем выберите виртуальную машину, для которой требуется приобрести резервирование. 

4.  На странице сведений о виртуальной машине найдите информацию о размере и регионе (см. рисунок ниже) и используйте эту информацию для приобретения резервирования в Центр партнеров.  

    ![](images/usage1.png)

**Получение сведений о размере виртуальной машины с помощью Microsoft Azure PowerShell**

Чтобы определить местоположение и размер виртуальной машины, для которой нужно приобрести резервирование, используйте данные, показанные на рисунке ниже. 

![](images/usage2.png)

**Получение сведений о размере виртуальной машины с помощью API для Azure Resource Manager (ARM)**

1.  С помощью ARMClient или API-интерфейсов ARM вызовите клиент ARM для виртуальной машины, для которой требуется приобрести резервирование.

2.  /subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01

3.  Вызов возвращает значения для параметров **vmSize** и **location**, как показано ниже.

    ![](images/usage3.png)
    ![](images/usage4.png)
 

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>Проверка использования виртуальной машины Azure и скидки на резервирование

После приобретения Azure Reserved VM Instance от имени клиента скидка на предоплату пространства на виртуальной машине автоматически применяется к виртуальным машинам, которые соответствуют атрибутам и количеству резервирования клиента. 

Вы можете проверить использование резервирования клиента и посмотреть, к каким виртуальным машинам применены скидки на резервирование. Это можно сделать следующими способами:   

-   Портал Azure
-   API использования Azure

Ниже приведены инструкции по каждому из этих методов.

>[!NOTE]
>Только API использования Azure показывает, к какой виртуальной машине применяется скидка.  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>Проверка использования резервирования клиента на портале Microsoft Azure

1.  В информационной панели для партнеров перейдите к странице " **Клиенты** ".

2.  Найдите клиента, для которого необходимо проверить использование резервирования и скидку, затем выберите стрелку вниз, чтобы посмотреть сведения о клиенте. Выберите **Портал управления Microsoft Azure**, чтобы открыть запись клиента на портале Azure. 

3.  Выберите пункт **Резервирования** в меню портала, затем выберите резервирование, чтобы проверить его использование. 

4.  На странице **Обзор** отображается график использования резервирования, который показывает, какой объем резервирования применен к виртуальным машинам. 

    >[!NOTE]
    >Данные об использовании могут отображаться с задержкой до 8 часов.
    
    а.  Если резервирование используется на 100%, клиент получает максимально возможную экономию, которую может обеспечить приобретенное резервирование. 
    
    б.  Если использование резервирования составляет 0%, скидка не применяется ни к одной виртуальной машине. 
    
    в.  Если использование резервирования составляет от 1% до 99%, у клиента есть неиспользуемые преимущества. 

5.  Во избежание подобных ситуаций перед покупкой необходимо правильно определить размер виртуальной машины в соответствии с требованиями клиента к вычислительной мощности.

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a>Проверка использования резервирования клиента с помощью API использования Azure

>[!NOTE]
>Только API использования Azure показывает, к какой виртуальной машине применяется скидка.  

Вы можете получить данные об использовании резервирования с помощью API использования Azure. Так можно проверить, получает ли клиент скидку за резервирование, и посмотреть, к каким виртуальным машинам применяется эта скидка. Сравните проверку использования резервирования в примерах А и Б. 

![](images\usage5.png)

-   Идентификатор reservationId определяет резервирование Azure, которое использовалось для применения скидки к виртуальной машине.
-   consumptionMeter — это MeterId для виртуальной машины, к которой применена скидка за резервирование.
-   ReservationMeter отображает стоимость $0, так как применена скидка за резервирование. 

Дополнительные сведения см. в разделе [Получение статистики использования Azure для клиента](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) в документе [API Центра партнеров](https://docs.microsoft.com/partner-center/develop/).

>[!IMPORTANT]
>Стоимость программного обеспечения, например Microsoft Windows Server, в настоящее время не входит в цену резервирования виртуальных машин и отображается в отдельных строках заказа и счета. Тем не менее, если у клиента есть преимущества гибридного использования Azure, стоимость программного обеспечения не учитывается. Дополнительные сведения см. в разделе [Затраты на программное обеспечение Windows, не включенные в зарезервированные экземпляры](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).  

## <a name="azure-reservations-resources"></a>Ресурсы о резервированиях Azure
|**Для получения информации о**   |**Прочтите этот документ**    |
|:-----------------------------|:-----------------|
|Обзор резервирований Azure в программе CSP  | [Продажа Microsoft Azure Reserved VM Instances](azure-reservations.md)
|Приобретение резервирований Azure для клиентов с помощью панели мониторинга центра партнеров   |[Приобретение резервирований Azure](azure-reservations-buying.md)
| Управление резервированиями Azure на информационной панели для партнеров | [Управление резервированиями Azure на информационной панели для партнеров](azure-reservations-manage.md)
|Приобретение резервирований Azure на портале Azure | [Предоплата за виртуальные машины с Azure Reserved VM Instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) в справке Azure |
|Управление резервированиями Azure на портале Azure   |[Управление зарезервированными экземплярами виртуальных машин](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) в справке Azure  |
|Приобретение резервирований Azure с помощью API Центра партнеров | [Приобретение услуги Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) в документации для разработчиков в Центре партнеров


