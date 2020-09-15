---
title: Dynamics 365 Forms pravila za posao – pravilo ne pucajte za obrazac
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
ms.openlocfilehash: 7422b67973f93ce10c1639209cc50206a1016c10
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711505"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Događaj OnChange ne dolazi ako je polje programsko promenjeno

Događaj *Onin* se ne javlja ako se polje promeni programskim korišćenjem *atributa.* metod [SetValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) . Ako želite da se Rukovaoci događajima za događaj *OnChange* pokrenu posle podešavanja vrednosti, morate da koristite *formatrikontekstualni. Data. atribut* [za šifrovanje](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) entiteta u kodu.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
