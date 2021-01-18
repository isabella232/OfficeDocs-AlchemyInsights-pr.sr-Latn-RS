---
title: Konfigurisanje usluge domena
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885689"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a>Nije moguće omogućiti AAD-DS ili primenu nije uspeo

Da biste rešili problem usluge Azure AD Domain (AAD-DS) nije omogućeno ili nije primenjeno, obavite sledeće korake:

1. Ako koristite postojeću virtuelnu mrežu, potvrdite NSG za pravila koja blokiraju portove neophodne za sinhronizovanje u AAD-DS-u na portalu https://aka.ms/aadds-networking .
2. Potvrdite izbor u polju za proveru da li se u ovom vodiču za rešavanje problema javlja odgovor na vašu grešku  https://aka.ms/aadds-troubleshoot-enable .
3. Isprobajte usluge Azure A.D. domena u novoj virtualnoj mreži.
4. Izvršite Vodič za prvi koraci kako biste primenili AAD-DS: [Kreirajte i konfigurišite usluge AAD Domain](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Ako imate problema sa primenom Azure AD Domain usluge domena, pogledajte članak [Rešavanje problema sa uslugom AZURE AD Domain](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) da biste rešili uobičajene greške koje vam pomažu da ponovo rešite stvari. 

**Nije moguće onemogućiti AAD-DS**

AAD-DS ne može da se pauzira. Ako želite da prestanete da koristite kontrolisano domen, on mora biti izbrisan.
Da biste izbrisali kontrolisani domen, pogledajte članak [Brisanje usluge AAD Domain](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).



