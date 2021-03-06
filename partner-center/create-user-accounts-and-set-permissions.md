---
title: Создание учетных записей пользователей и определение разрешений | Центр партнеров
ms.topic: article
ms.date: 02/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Узнайте, как создавать учетные записи пользователей и назначать роли в Центре партнеров для каждого сотрудника, которому требуется доступ. Это могут делать пользователи с определенными правами администратора.
ms.assetid: 75D805AE-9922-4CFD-9427-196047D70963
author: LauraBrenner
ms.author: labrenne
Keywords: роли, разрешения, добавление пользователя, назначение роли, администратор, агент,
ms.localizationpriority: high
ms.openlocfilehash: f163e37f537f537b6eae086e355c87d892d1a745
ms.sourcegitcommit: faf7b1ac1653497f963b428bbfafcd821378adaa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2020
ms.locfileid: "82798492"
---
# <a name="create-user-accounts-and-assign-permissions"></a>Создание учетных записей пользователей и назначение разрешений

**Соответствующие роли**

- Администратор учетных записей
- Глобальный администратор
- Администратор управления пользователями

Создайте учетные записи пользователей для сотрудников, которым требуется доступ к Центру партнеров. Эти задачи должны выполняться администратором управления пользователями, администратором учетных записей или глобальным администратором. Пользователю, выполняющему эти задачи, нужно назначить роль администратора или глобального администратора Azure Active Directory (AAD). См. сведения о [разрешениях ролей администратора в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles).


## <a name="add-a-new-user"></a>Добавление нового пользователя

1. Щелкните значок **Параметры** в правом верхнем углу Центра партнеров и выберите **Управление пользователями**.

2. Выберите **Добавить пользователя**.

3. Введите полное имя пользователя и уникальный адрес электронной почты.

4. Выберите тип агента и (или) тип администратора, который требуется назначить пользователю. Доступ в Центре партнеров зависит от ролей, поэтому можно назначить разрешения, чтобы настроить представление пользователя на отображение только функциональных возможностей, необходимых пользователю для выполнения определенных задач.  Если пользователь хочет, чтобы ему назначили роль, ему нужно найти глобального администратора, перейдя в раздел **Управление пользователями** и выполнив фильтрацию по этой роли.

5. Выберите **Добавить** для создания учетной записи пользователя. Подтвердите сведения пользователя на следующей странице.

> [!IMPORTANT]  
> Запомните или запишите данные для входа нового пользователя, отображаемые на этой странице. Не забудьте скопировать и отправить эти сведения для новых пользователей, так как вы не сможете получить к нему доступ позже. 


Пользователь должен войти в Центр партнеров с помощью имени пользователя и временного пароля. Когда пользователь входит в Центр партнеров в первый раз, будет предложено изменить свой пароль. 


### <a name="find-your-global-admin"></a>Поиск глобального администратора

Иногда может потребоваться изменить роль имеющего пользователя или назначить определенную роль новому пользователю.  
Чтобы найти глобального администратора, который может вносить изменения в роль или назначать роли новому пользователю, щелкните значок **Параметры** в правом верхнем углу Центра партнеров, выберите **Управление пользователями** и выполните фильтрацию по роли глобального администратора. 


### <a name="new-global-admin"></a>Новый глобальный администратор

Если ваш глобальный администратор покидает организацию и кому-то нужно занять его место, вы можете отправить запрос в команду Azure или Office 365. Чтобы узнать, как это сделать, выберите один из вариантов ниже:

[Новый глобальный администратор Azure](https://support.microsoft.com/help/4505981/what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company)

[Новый глобальный администратор Office 365](https://admin.microsoft.com/)


## <a name="assign-user-roles"></a>Назначение ролей пользователей

Чтобы пользователь мог работать в Центре партнеров, ему должна быть назначена роль.  В настоящее время роли включают в себя роли клиента Azure Active Directory, роли поставщика облачных решений (CSP) и роли компании, не связанные с AAD. Отдельная компания может нуждаться во всех этих ролях.

>[!Important]
>Чтобы пользователи могли получить доступ к Центру партнеров, они должны быть указаны в вашем клиенте. Назначения ролей обеспечивают дополнительный доступ.


**Роли клиента AAD**:
- Глобальный администратор
- администратор пользователей.

**Роли CSP**:
- Агент по администрированию
- Администратор выставления счетов
- Агент по продажам
- Агент службы технической поддержки

**Роли, управляющие членством в MPN и организацией (не связанные с AAD)** :
- Администратор партнера MPN
- Администратор учетных записей
- администратор рекомендаций;
- Администратор бизнес-профиля
- администратор поощрений и пользователь.

**Роль поставщика панели управления (это CSP и роль, не связанная с AAD)** :
- Глобальный администратор

**Гостевой пользователь** должен быть частью клиента AAD и может иметь любые роли, не связанные с AAD.

Более подробные сведения о ролях и возможностях каждой из них см. в статье [Назначение пользователям ролей и разрешений](permissions-overview.md).

## <a name="associate-a-users-microsoft-learn-account-in-partner-center"></a>Связывание учетной записи пользователя Microsoft Learn с Центром партнеров

Чтобы увидеть пути обучения, которые ваши пользователи проходят для получения компетенций, им необходимо связать свой идентификатор MCP с учетной записью Центра партнеров. При добавлении новых пользователей вам, как глобальному администратору, нужно напомнить им о необходимости связать идентификатор MCP с их учетной записью. 

### <a name="how-to-associate-your-mcp-id-to-your-partner-center-account"></a>Связывание идентификатора MCP с учетной записью Центра партнеров

1. В правом углу Панели мониторинга Центра партнеров щелкните значок **Your account** (Ваша учетная запись), а затем выберите **My profile** (Мой профиль).

2. В разделе **Your learning** (Ваше обучение) вы сможете привязать свою учетную запись Microsoft Learning, а также подключить учетную запись Майкрософт к Partner University.







