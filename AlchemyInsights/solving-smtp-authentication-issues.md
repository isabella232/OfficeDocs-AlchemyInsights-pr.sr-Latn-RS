---
title: Omogućavanje SMTP potvrde identiteta i rešavanja problema
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
- "3000003"
- "5652"
ms.openlocfilehash: 14f1454ad687b4d76cf419583b442685fa19b5a2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321767"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>Omogućavanje SMTP potvrde identiteta i rešavanja problema

Ako želite da omogućite SMTP potvrdu identiteta za poštansko sanduče ili dobijate "Klijent nije ovlašten", Greška "Potvrda identiteta bezuspešno" ili "SmtpClientAuthentication" sa kodom 5.7.57 ili 5.7.3 ili 5.7.139 kada pokušate da pošaljete e-poštu potvrdom identiteta uređaja ili aplikacije pomoću usluge Microsoft 365, izvršite ove tri radnje da biste rešili problem:

1. Onemogućite [podrazumevane vrednosti bezbednosti za Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) tako što će na vrednost "Omogući **podrazumevane vrednosti bezbednosti" onemogućiti** **vrednost "Ne"**.

    a. Prijavite se na Azure portal kao administrator za bezbednost, administrator uslovnog pristupa ili globalni administrator.<BR/>
    b. Potražite svojstva Azure Active Directory > **.**<BR/>
    c. Izaberite **stavku Upravljanje podrazumevanim vrednostima bezbednosti**.<BR/>
    d. Postavite **opciju Omogući podrazumevane vrednosti bezbednosti** na **Ne**.<BR/>
    e. Izaberite **Sačuvaj**.

2. [Omogućite SMTP prosleđivanje klijenta](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) u licenciranom poštanskom sandučetu.

    a. Na Microsoft 365 centar administracije izaberite stavku **Aktivni korisnici**, a zatim izaberite korisnika.<BR/>
    b. Idite na karticu Pošta i u okviru **Aplikacije za e-poštu** izaberite stavku **Upravljanje aplikacijama za e-poštu**.<BR/>
    d. Proverite **da li je potvrđen potvrđen identitet SMTP** (omogućeno).<BR/>
    e. Izaberite **Sačuvaj promene**.<BR/>

3. [Onemogućite uslugu Multi-Factor Authentication (MFA)](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) na licenciranom poštanskom sandučetu.

    a. Idite na prozor Microsoft 365 centar administracije u meniju navigacije sa leve strane izaberite stavku **Korisnici**  >  **aktivni korisnici.**<BR/>
    b. Izaberite **stavku Multi-Factor Authentication**.<BR/>
    c. Izaberite korisnika i **onemogućite Multi-Factor Auth**.<BR/>
