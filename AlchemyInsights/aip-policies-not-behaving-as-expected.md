---
title: 'AIP: Smernice se ne ponašaju kao što se očekuje'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 90448bf57297ce59ba222efd1927b5de588bfbfdb1206b6403764d7f43fed690
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934307"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: Smernice se ne ponašaju kao što se očekuje

Azure Information Protection: Smernice koje se ne ponašaju kao što se očekuje, pogledajte sledeće da biste dobili preporučena uputstva za različite probleme sa smernicama:

1. Ako imate problema sa vizuelnim oznakama, pregledajte kada [se primenjuju vizuelne oznake.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)
2. Ako imate problema sa automatskom oznakom, pogledajte kako da konfigurišete uslove za automatsku i preporučenu klasifikaciju za [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) i Šta tipovi osetljivih [informacija potraže.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
3. Ako imate problema sa zaštitom native/Pfile, pregledajte [konfiguraciju API-ja datoteke.](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)
4. Proverite da li koristite određivane smernice koje nisu ispravno konfigurisane: Kako se konfiguriše [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)smernica za određene korisnike pomoću proširenih smernica.
5. Ako automatsko označavanje ne funkcioniše za Outlook prilaganje označenog dokumenta, proverite da DRMEncryptProperty nije definisan kao što je opisano ovde: Postavke [IRM registratora](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)za bezbednost.

Ako i dalje imate problema, prikupite evidencije Azure Information Protection klijenta i priložite izvezene evidencije ovom tiketu.

1. Otvorite dokument Kancelarija ili kreirajte novu e-poruku u programu Outlook.
2. Izaberite **stavku Pomoć i povratne informacije o**  >  **zaštiti/osetljivosti.**
3. Izaberite **stavku Izvoz evidencija**.
4. Sačuvajte evidencije na svojoj lokaciji i priložite ih ovom zahtevu za uslugom.

Dodatni resursi:

- [Konfigurisanje oznake za vizuelne oznake za Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Pregled dokumentacije za Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Korišćenje oznaka osetljivosti u Microsoft 365 aplikacijama](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

