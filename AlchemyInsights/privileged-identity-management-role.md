---
title: Privileged Identity Management uloge
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
- "9003230"
- "6825"
ms.openlocfilehash: 358e446192e6b58ace81afa06e0d65ae3a207282351ffc3ec9975a24779951fb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973243"
---
# <a name="privileged-identity-managementpim-role"></a>Privileged Identity Management(PIM) uloga

**Dozvole se ne dodeljuju nakon aktiviranja uloge**

Kada aktivirate ulogu u Azure AD Privileged Identity Management (PIM), aktivacija se možda neće odmah preneti na sve portale koji zahtevaju privilegovanu ulogu. Ponekad, čak i ako se promena prenese, keširanje veba na portalu može da dovede do toga da promena ne stupi odmah na snagu.

Ako je aktivacija odložena, sledite ove korake:

1. Odjavite se sa Azure portala, a zatim se ponovo prijavite. Kada aktivirate ulogu Azure AD ili ulogu Azure resursa, videćete faze aktivacije. Kada se sve faze dovrše, videćete vezu "Odjavi se". Ovu vezu možete da koristite za odjavu. Ovo će rešiti većinu slučajeva za odlaganje aktivacije.
2. U pim kodu potvrdite da ste navedeni kao član uloge.
3. Ako aktivirate ulogu administratora Exchange, odjavite se i ponovo se prijavite. Ako problem potraje, otvorite tiket za podršku i podignite ga kao problem. Ako koristite ulogu administratora Exchange za pristup centru za bezbednost i usaglašenost, pogledajte sledeći korak.
4. Ako aktivirate ulogu za pristup centru za bezbednost i usaglašenost ili ako aktivirate ulogu SharePoint administratora, doživećete neko kašnjenje aktivacije od nekoliko minuta do nekoliko časova. Ovo je poznat problem i aktivno sarađujemo sa ovim timovima da bismo što pre rešili ovaj problem.

Za više informacija pogledajte:

- [Aktiviranje Azure AD uloga u piM kodu](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Aktiviranje Azure uloga resursa u piM kodu](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Dozvole se ne uklanjaju nakon deaktivacije uloge ili isteka aktivacije uloge**

Kada deaktivirate ulogu u Azure AD Privileged Identity Management ili kada istekne period aktivacije uloge, možda postoji kašnjenje kada i dalje imate pristup.

Ako deaktivacija bude odložena, sledite ove korake:

1. Ako deaktivujete ulogu administratora Exchange ili period aktivacije uloge ističe i primećujete znatno odlaganje pre nego što se dozvole uklone, otvorite tiket za podršku i recite inženjeru za podršku da vam pomogne da zakažete tiket sa timom za privileged Access Management (PAM) unutar programa Kancelarija o ovom problemu.
2. Ako je period aktivacije istekao, ali sesija pregledača je i dalje otvorena, zatvorite pregledač. Ulogu možete da nastavite da koristite dok ne zatvorite tu sesiju. Ovo je poznat problem i tražimo potencijalno rešenje za aktivno opoziv svake sesije kada aktivacija istekne.

Ako je vaše odlaganje drugačije od ova dva scenarija, otvorite tiket za podršku.
