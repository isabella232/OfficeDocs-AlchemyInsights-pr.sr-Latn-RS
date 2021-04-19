---
title: Automatska klasifikacija se ne ponaša kao što se očekuje sa AIP klijentom
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
- "4373"
ms.openlocfilehash: b7ab09fe8430a54dacf2cd1ba076414a5f562541
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820912"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Automatska klasifikacija se ne ponaša kao što se očekuje sa AIP klijentom

Automatska klasifikacija nije očekivana, koristite sledeća preporučena uputstva:

1. Ako imate problema sa automatskom oznakom, pogledajte kako da konfigurišete uslove za automatsku i preporučenu klasifikaciju za [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) i Šta tipovi osetljivih [informacija potraže.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
2. Proverite da li koristite određivane smernice koje nisu ispravno konfigurisane: Kako se konfiguriše [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)smernica za određene korisnike pomoću proširenih smernica.
3. Ako automatsko označavanje ne funkcioniše za Outlook kada prilažete označeni dokument, proverite da to nije definisano kao što je opisano ovde: Postavke `DRMEncryptProperty` [IRM registratora](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)za bezbednost.
4. Ako ste koristili [ugrađene tipove](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) informacija za Azure Information Protection smernice, proverite da li se sadržaj podudara sa očekivanim formatom.
5. Proverite da li je nalepnica na odgovarajući način konfigurisana **za Automatski** ili **Preporučeno.** (**Automatsko** označavanje je dostupno za sve Microsoft 365 aplikacije, dok je preporučeno dostupno za sve Microsoft 365 aplikacije osim za Outlook.) 
6. Ne možete da koristite automatsku klasifikaciju za dokumente i e-poruke koje su prethodno ručno obeležene ili prethodno označene višom klasifikacijom.  Dodatne informacije potražite u: [kako se primenjuju automatske ili preporučene oznake.](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied)
7. Ako i dalje imate problema, prikupite evidencije Azure Information Protection klijenta i priložite izvezene evidencije tiketu za podršku. Da biste izvezli Azure Information Protection evidencije:
    - Otvorite Office dokument ili kreirajte novu e-poruku u programu Outlook.
    - Izaberite **stavku Pomoć i povratne informacije o**  >  **zaštiti/osetljivosti.**
    - Izaberite **stavku Izvoz evidencija**.
    - Sačuvajte evidencije na svojoj lokaciji i priložite ih zahtevu za uslugom.

Dodatne informacije potražite u:

- [Konfigurisanje uslova za automatsku i preporučenu klasifikaciju za Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Uputstva za uobičajene scenarije koji koriste Azure Information Protection](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Pregled dokumentacije za Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Pregled pretplata i funkcija za Azure Information Protection](https://azure.microsoft.com/pricing/details/information-protection)
- [Zahtevi za Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Uputstvo za brzi početak za Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Preuzimanje Azure Information Protection klijenta](https://www.microsoft.com/download/details.aspx?id=53018)
