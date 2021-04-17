---
title: Postavljanje automatskih odgovora za poštansko sanduče
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
- "9000761"
- "3514"
ms.openlocfilehash: 60af581e7fe508ab9644a53873bcd551b3aacff1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820948"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Postavljanje automatskih odgovora za poštansko sanduče korisnika

**Metod 1**

1. Prijavljivanje u Microsoft 365 portal.

2. Idite na stavku **Korisnici > Aktivni korisnici** (ili **Grupe > Deljeni poštanski sandučići** ako ste postavili ovo na deljeno poštansko sanduče).

3. Izaberite korisnika koji ima Microsoft Exchange poštansko sanduče.

4. U dodatnom meniju nadesno idite na **Postavke pošte > Automatski odgovori**(ako je u pitanju deljeno poštansko sanduče, samo kliknite **Automatski odgovori** u dodatnom meniju).

**Metod 2**

1. Prijavite se na Microsoft 365 portal za administraciju pomoću akreditiva administratora.

2. Proširite **Centre za administraciju**, a zatim kliknite na stavku **Exchange**.

3. Kliknite na sliku u gornjem desnom uglu, kliknite na stavku **Još jedan korisnik**, a zatim izaberite korisničko poštansko sanduče koje želite da promenite.

4. Na levoj strani izaberite stavku **Opcije**, kliknite na stavku **Organizovanje e-pošte**, a zatim kliknite na dugme **Automatski odgovori.**

**Metod 3**

Pokrenite sledeće cmdlet komandu u usluzi Exchange Online Windows PowerShell:

PowerShellCopy

```
    Set-MailboxAutoReplyConfiguration
```

Više informacija o ovoj cmdlet komandi potražite u članku [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).
