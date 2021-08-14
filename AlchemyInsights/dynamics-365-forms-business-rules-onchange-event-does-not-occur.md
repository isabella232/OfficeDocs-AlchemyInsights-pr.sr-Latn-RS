---
title: Dynamics 365 Forms Business Rules – Poslovno pravilo ne iseca za obrazac
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 8425918950e1ef6c44f2866e6fa8987fe165536ae21e08ea6a1da880f761d512
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53947313"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Događaj OnChange se ne odvija ako se polje programski menja

Događaj *OnChange* se ne odvija ako se polje programski menja pomoću atributa.  [setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) metod. Ako želite da se rukovaoci događajem pokreću za *događaj OnChange* pošto postavite vrednost, morate da koristite *atribut formContext.data.entity* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) metod u kodu.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
