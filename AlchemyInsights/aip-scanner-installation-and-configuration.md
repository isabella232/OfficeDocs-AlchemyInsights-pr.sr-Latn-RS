---
title: 'AIP skener: instalacija i konfiguracija'
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
- "9002278"
- "5119"
ms.openlocfilehash: c32f3f10e2e17cf67e73ec8404be293eeefb68a3
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821677"
---
# <a name="aip-scanner-installation-and-configuration"></a>AIP skener: instalacija i konfiguracija

**Da biste instalirali AIP skener, pratite preporučena uputstva:**

1. Ako vršite nadogradnju i ne izvršavate čistu instalaciju, proverite da li ste pratili uputstva za nadogradnju [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) skenera, a za klijenta za oznake koji ima više oznaka, pogledajte nadogradnju [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)skenera.
2. Proverite da li ste usavršni sa svim [zahtevima postavki zaštitnih zidova i mrežne infrastrukture.](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)
3. Uverite se [da su smernice podešene na](https://docs.microsoft.com/azure/information-protection/configure-policy) automatsko označavanje ili da imaju podrazumevanu oznaku u smernicama.
4. Proverite da li je odgovarajući tip datoteke konfigurisan za oznaku/zaštitu kao što je opisano u članku Tipovi datoteka koje podržava [Azure Information Protection klijent.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection) Pored toga, ako želite da promenite podrazumevano ponašanje, pratite ova uputstva: Promena podrazumevanog [nivoa zaštite datoteka.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)
5. Proverite da li korisnički nalog konfigurisan za pokretanje usluge skenera ima dozvole za pristup svim konfigurisanim repositovima.
6. Ako i dalje imate problema, izvezite evidencije skenera i dodajte ih u tiket za podršku.

**Izvoz evidencija Azure Information Protection skenera**

1. Pređu na %localappdata%\Microsoft\MSIP u okviru korisničkog konteksta koji koristi uslugu skenera.
2. Zipuj sav sadržaj u fascikli MSIP.
3. Sačuvajte evidencije na svojoj lokaciji i priložite ih zahtevu za uslugom.
4. Možete da koristite [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**Dodatne informacije potražite u:**
- [Primena Azure Information Protection skenera za automatsko klasifikaciju i zaštitu datoteka](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Navođenje i korišćenje parametra tokena za set-AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Pokretanje ciklusa otkrivanja i prikaz izveštaja za skener](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Pregled dokumentacije za Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Zahtevi za Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Preuzimanje Azure Information Protection klijenta](https://www.microsoft.com/download/details.aspx?id=53018)
