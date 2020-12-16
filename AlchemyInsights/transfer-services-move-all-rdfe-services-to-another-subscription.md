---
title: Prenos usluga – premeštanje svih RDFE usluga na drugu pretplatu
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692175"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Prenos usluga – premeštanje svih RDFE usluga na drugu pretplatu

**Premeštanje resursa**

Azure resursi mogu da se premeštaju u drugu Azure pretplatu ili grupu resursa u okviru iste pretplate pomoću Azure portala, Azure PowerShell, Azure CLI ili OSTATAK API-ja za premeštanje resursa.

Da biste mogli da premestite resurse, pogledajte članak:

- [Kontrolna lista pre premeštanja resursa](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Usluge koje mogu da se premeste](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Kako da proverite valjanost premeštanja](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Premeštanje smernica za usluge](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Da biste premestili postojeće resurse u drugu grupu resursa ili pretplatu, možete da koristite:

- [Azure portal](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Uputstvo: [Premeštanje Azure resursa u drugu grupu resursa ili pretplatu](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Rešavanje problema sa greškama u alatki Azure Manager**

Pogledajte članke ispod da biste saznali više o uobičajenim Azure greškama prilikom raspoređivanja i primite informacije za njih. Ako ne možete da pronađete kôd greške za vašu grešku prilikom primene, pogledajte članak [Pronalaženje kôda greške](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [Rešavanje problema sa ispravkom primene](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Rešavanje problema pri premeštanju Azure resursa u novu grupu resursa ili pretplatu](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Imajte u vidu da ako želite da nadogradite Azure pretplatu, kao što je prebacivanje sa slobodne na Pay-as-go, moraćete da konvertujete pretplatu.

- Da biste nadogradili besplatnu probnu verziju, pogledajte članak [Nadogradnja besplatnog pokušaja ili Microsoft pogledajte Azure pretplatu na "pay-as](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription)".
- Da biste promenili nalog za plaćanje plaćanja, pogledajte članak [Promena Azure Pay-as-you-go pretplate na drugačiju ponudu](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).

**Da biste dodali ili povezali Azure pretplatu na Azure Active Directory stanar:**

1. Prijavite se i izaberite pretplatu koju želite da koristite na stranici " [pretplate" u usluzi Azure](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).
2. Izaberite stavku **Promeni direktorijum**.
3. Pregledajte sva upozorenja koja se pojavljuju, a zatim izaberite stavku **Promeni**.
4. Direktorijum se menja za pretplatu i imaćete poruku o uspehu.
5. Koristite sviščer *direktorijuma* da biste otiљli u novi direktorijum. Može biti potrebno do 10 minuta da se sve dobro pokaže.

**Preporučeni dokumenti**

- [Prebacivanje vlasništva nad Azure pretplatom](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Premeštanje resursa na novu grupu resursa ili pretplatu](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Upravljanje resursima pomoću Azure portala](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
