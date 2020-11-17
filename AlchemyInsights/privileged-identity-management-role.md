---
title: Privilegija upravljanja identitetom
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
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 11/17/2020
ms.locfileid: "49089153"
---
# <a name="privileged-identity-managementpim-role"></a>Privilegija za upravljanje identitetom (PIM)

**Dozvole se ne odobravaju nakon aktiviranja uloge**

Kada aktivirate ulogu u usluzi Azure A.D. za upravljanje identitetom (PIM), aktivacija se možda neće odmah preneti na sve portove koji zahtevaju privilegovanu ulogu. Ponekad, čak i ako se promena produži, Veb keširanje na portalu može dovesti do toga da promena ne stupa na snagu odmah.

Ako je aktivacija odložena, slijedite ove korake:

1. Odjavite se sa Azure portala, a zatim se ponovo prijavite. Kada aktivirate Azure reklamu uloge ili vrednost Azure resursa, videćete faze aktivacije. Kada se sve faze završe, videćete povezanost "odjavljivanje". Možete da koristite ovu povezanost da biste se odjavili. Ovo će rešiti većinu slučajeva za odlaganje aktiviranja.
2. U okviru PIM, proverite da li ste navedeni kao član uloge.
3. Ako aktivirate ulogu administratora Exchange servera, obavezno se odjavite i ponovo prijavite. Ako se problem ponavlja, otvorite karticu podrške i podiћete ovo kao problem. Ako koristite ulogu administratora Exchange servera da biste pristupili centru za bezbednost i usaglašenost, pogledajte sledeći korake.
4. Ako aktivirate ulogu da biste pristupili centru za bezbednost i usaglašenost ili ako aktivirate ulogu SharePoint administratora, nailazite na odlaganje aktiviranja od nekoliko minuta do nekoliko časova. Ovo je poznati problem i aktivno radimo sa tim timovima da rešimo ovaj problem što je pre moguće.

Za više informacija pogledajte članak:

- [Aktiviranje moje Azure OGLASE uloge u PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Aktiviranje moje usluge Azure resursa u PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Dozvole se ne uklanjaju nakon deaktiviranja uloge ili ističe aktivacija uloge**

Kada deaktivirate ulogu u usluzi Azure za upravljanje identitetom ili kada istekne period aktivacije uloge, možda će biti kašnjenje gde i dalje imate pristup.

Ako je vaša deaktivacija odložena, slijedite ove korake:

1. Ako deaktivirate ulogu administratora Exchange servera ili istekne period aktivacije uloge, a primetite značajno odlaganje pre nego što se dozvole uklone, otvorite ulaznicu za podršku i obratite se tehničar za podršku da vam pomogne da uradite kaznu sa ekipom za upravljanje pristupom za ovaj problem.
2. Ako je period aktivacije istekao, ali i dalje imate otvorenu sesiju pregledača, zatvorite pregledač. Možete nastaviti da koristite ulogu dok ne zatvorite tu sesiju. Ovo je poznati problem i tražimo potencijalnu popravku da bismo aktivnu opozvali svaku sesiju kada aktivacija istekne.

Ako je kašnjenje drugačiji od ova dva scenarija, otvorite ulaznicu za podršku.
