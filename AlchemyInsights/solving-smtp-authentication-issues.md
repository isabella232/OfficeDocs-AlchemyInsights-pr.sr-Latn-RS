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
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077665"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>Omogućavanje SMTP potvrde identiteta i rešavanja problema

Ako želite da omogućite SMTP potvrdu identiteta za poštansko sanduče ili dobijate "Klijent nije ovlašten", Greška "Potvrda identiteta bezuspešno" ili "SmtpClientAuthentication" sa kodom 5.7.57 ili 5.7.3 ili 5.7.139 kada pokušate da pošaljete e-poštu potvrdom identiteta uređaja ili aplikacije pomoću usluge Microsoft 365, izvršite ove tri radnje da biste rešili problem:

1. Onemogućite [podrazumevane vrednosti bezbednosti za Azure](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) tako što će na vrednost "Omogući **podrazumevane vrednosti bezbednosti" onemogućiti** **vrednost "Ne"**.

    a. Prijavite se na Azure portal kao administrator za bezbednost, administrator uslovnog pristupa ili globalni administrator.<BR/>
    b. Potražite svojstva  **Azure Active Directory >.**<BR/>
    c. Izaberite **stavku Upravljanje podrazumevanim vrednostima bezbednosti**.<BR/>
    d. Postavite **opciju Omogući podrazumevane vrednosti bezbednosti** na **Ne**.<BR/>
    e. Izaberite **Sačuvaj**.

2. [Omogućite SMTP prosleđivanje klijenta](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) u licenciranom poštanskom sandučetu.

    a. Na Microsoft 365 centar administracije stavku **Aktivni** korisnici i izaberite korisnika.<BR/>
    b. Idite na karticu Pošta i u okviru **Aplikacije za e-poštu** izaberite stavku **Upravljanje aplikacijama za e-poštu**.<BR/>
    d. Proverite da li je potvrđena potvrda identiteta **SMTP** (omogućeno).<BR/>
    e. Izaberite **Sačuvaj promene**.<BR/>

3. [Onemogućite uslugu Multi-Factor Authentication (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) na licenciranom poštanskom sandučetu.

    a. Idite na prozor Microsoft 365 centar administracije u meniju navigacije sa leve strane izaberite stavku **Korisnici**  >  **aktivni korisnici.**<BR/>
    b. Izaberite **stavku Multi-Factor Authentication**.<BR/>
    c. Izaberite korisnika i **onemogućite Multi-Factor Auth**.<BR/>
