---
title: Kontroler domena
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901312"
---
# <a name="domain-controller"></a>Kontroler domena

**Nije moguće omogućiti AAD-DS ili primenu nije uspeo**

Da biste rešili problem usluge Azure AD Domain (AAD-DS) nije omogućeno ili nije primenjeno, obavite sledeće korake:

1. Ako koristite postojeću virtuelnu mrežu, potvrdite NSG za pravila koja blokiraju portove neophodne za sinhronizovanje u AAD-DS-u na portalu https://aka.ms/aadds-networking .
2. Potvrdite izbor u polju za proveru da li se u ovom vodiču za rešavanje problema javlja odgovor na vašu grešku  https://aka.ms/aadds-troubleshoot-enable .
3. Isprobajte usluge Azure A.D. domena u novoj virtualnoj mreži.
4. Izvršite Vodič za prvi koraci kako biste primenili AAD-DS, koji je dostupan u [uputstvu da biste kreirali Azure AD Domain usluge domena](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Ako imate problema sa primenom Azure AD Domain usluge domena, pogledajte članak [Rešavanje problema sa uslugom AZURE AD Domain](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) da biste rešili uobičajene greške koje vam pomažu da ponovo rešite stvari. 

**Nije moguće onemogućiti AAD-DS**

AAD-DS ne može da se pauzira. Ako želite da prestanete da koristite kontrolisano domen, on mora biti izbrisan.

Ako naiđete na probleme, da biste rešili uobičajene poruke o greškama i povezane korake za rešavanje problema, pogledajte članak [Rešavanje problema sa uslugom Azure Active Directory](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).
