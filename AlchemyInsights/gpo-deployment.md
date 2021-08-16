---
title: Primena GPO-a
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: 6f9e164713ce36023de954d45031fd4414780e174bf5c7741c4aec274a65b32e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54067854"
---
# <a name="gpo-deployment"></a>Primena GPO-a

Postavke objektima korisnika i računara u Azure Active Directory uslugama domena (Azure AD DS) često se upravlja pomoću objekata smernica grupe (GPO-ove). Azure AD DS uključuje ugrađene GPO-ove za kontejnere AADDC korisnika i AADDC računara. Možete da prilagodite ove ugrađene GPO-ove da biste konfigurisali smernice grupe po potrebi za okruženje. Članovi Azure AD DC grupe administratora imaju privilegije administracije smernica grupe u Azure AD DS domenu i mogu da kreiraju i prilagođene GPO-ove i organizacione jedinice (OU-ove). Dodatne informacije o tome šta su smernice grupe i kako funkcionišu potražite u [temi Pregled smernica grupe.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))

U hibridnom okruženju smernice grupe konfigurisane u okruženju okruženja koje se ne sinhronizuju sa uslugom Azure AD DS ne sinhronizuju se. Da biste definisali postavke konfiguracije za korisnike ili računare u Azure AD DS, uredite neki od podrazumevanih GPO-ova ili kreirajte prilagođeni GPO.

Ovaj članak [Upravljanje](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) smernicama grupe pokazuje vam kako da instalirate alatke za upravljanje smernicama grupe, kako da uredite ugrađene GPO-ove i kako da kreirate prilagođene GPO-ove.
