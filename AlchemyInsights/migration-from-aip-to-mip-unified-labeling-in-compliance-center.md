---
title: Migracija iz programa AIP u MIP/ujedinjavanje u centru za usaglašenost
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674340"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Migracija iz programa AIP u MIP/ujedinjavanje u centru za usaglašenost

Da biste migrirali sa AIP nalepnica do jedinstvenog označavanja u centru za bezbednost i usaglašenost, uradite sledeće:

**Aktivacija zaštite sa Azure portala**

1. Ako to već niste uradili, otvorite novi prozor pregledača i [Prijavite se na Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal). Pređite na oљtricu **Azure zaštite informacija** . Na primer, u meniju čvorište izaberite stavku **sve usluge** i počnite da kucate **informacije** u polju Filter. Izaberite stavku **Azure zaštita informacija**. Ako niste ranije pristupili Azure zaštiti informacija, pogledajte sledeće [korake](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) da biste dodali ovu oљtricu na portal. Da biste otvorili karticu Azure zaštite informacija, morate imati ili [Azure Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) ili Office 365 plan koji uključuje upravljanje pravima. Ako imate jednu od ovih pretplata, ali vidite poruku da nije moguće pronaći važeću pretplatu, obratite se [Microsoft podršci](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) ili koristite standardne kanale podrške.

2. Pronađite opcije **upravljanja** menijima i izaberite stavku **aktivacija zaštite**. Kliknite na dugme **Aktiviraj**, a zatim potvrdite radnju. Kada se aktivacija dovrši, informativna traka prikazuje **Aktiviranje je završeno**.

**Migriranje Azure usluge zaštite informacija u Office 365 Security & centar za usaglašenost**

1. Uverite se da ste prijavljeni kao korisnik sa dozvolom globalnog administratora.

2. Pređite na oљtricu **Azure zaštite informacija** .

3. U opciji **Upravljanje** menijima izaberite stavku **objedinjeno označavanje**.

4. Na **sečivu Azure informacije – objedinjeno označavanje informacija** kliknite na dugme **Aktiviraj** i sledi uputstva na mreži.

**Napomena**: proverite da li imate odgovarajuće dozvole pre nego što aktivirate migraciju centra za usaglašenost &. Pogledajte ove članke za više informacija:

1. [Da li treba da budete globalni administrator da biste konfigurisali Azure zaštitu informacija ili mogu da delegat drugim administratorima?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Važne informacije o administratorskim ulogama posle migriranja u bezbednosni & centru za usaglašenost.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Više informacija o AIP-u za Ujedinjeno označavanje migracije u centar za bezbednost i usaglašenost potražite u članku [Migriranje nalepnica](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).
