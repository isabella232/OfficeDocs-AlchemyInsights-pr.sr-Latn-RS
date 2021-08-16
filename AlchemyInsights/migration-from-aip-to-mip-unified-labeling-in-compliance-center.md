---
title: Migracija iz AIP u MIP/unified Labeling u centru za usaglašenost
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
- "5114"
ms.openlocfilehash: 378c3f58f77db8b23682432c942cd4f9c3a392651ca6564528a635724ad66a25
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54000370"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Migracija iz AIP u MIP/unified Labeling u centru za usaglašenost

Da biste migrirani iz AIP nalepnica u "Ujedinjeno označavanje" u centru za bezbednost i usaglašenost, uradite sledeće:

**Aktiviranje zaštite sa Azure portala**

1. Ako to već niste uradili, otvorite novi prozor pregledača i [prijavite se na Azure portal.](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal) Prešli na **Azure Information Protection** blejd. Na primer, u meniju Čvorište izaberite stavku **Sve usluge** i počnite da kucate **informacije** u polju Filter. Izaberite **stavku Azure Information Protection**. Ako ranije niste pristupili Azure Information Protection bleju, [](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) pogledajte jedno vreme dodatne korake da biste dodali ovaj blejd na portal. Da biste otvorili blejd Azure Information Protection, morate da imate [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) ili Office 365 plan koji obuhvata Rights Management. Ako imate jednu od ovih pretplata, ali vidite poruku da nije moguće pronaći važeću pretplatu, obratite se [Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) podršci ili koristite standardne kanale podrške.

2. Pronađite **opcije menija** "Upravljanje" i izaberite **stavku Aktivacija zaštite.** Kliknite na **aktiviranje**, a zatim potvrdite radnju. Kada se aktivacija dovrši, traka sa informacijama prikazuje **da je Aktivacija uspešno završena.**

**Migracija Azure Information Protection oznaka Office 365 centru & za usaglašenost**

1. Proverite da li ste prijavljeni kao korisnik sa dozvolom globalnog administratora.

2. Prešli na **Azure Information Protection** blejd.

3. U opciji **menija** Upravljanje izaberite stavku **"Ujedinjena oznaka"**.

4. Na **bleju Azure Information Protection – unified labeling** blade kliknite na **Aktiviraj** i pratite uputstva na mreži.

**Na primer: Uverite** se da imate odgovarajuće dozvole pre aktivacije migracije centra za & usaglašenost centra za usaglašenost. Pogledajte ove članke za više informacija:

1. [Da li treba da budete globalni administrator da biste konfigurisali Azure Information Protection ili mogu da delegiram drugim administratorima?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Važne informacije o administrativnim ulogama posle migracije u centar & za usaglašenost.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Dodatne informacije o migraciji AIP-a u centar za bezbednost i usaglašenost potražite u temi [Migracija nalepnica.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)
