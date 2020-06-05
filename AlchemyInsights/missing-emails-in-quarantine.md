---
title: Nedostajuće e-poruke u karantinu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569558"
---
# <a name="missing-emails-in-quarantine"></a>Nedostaju e-poruke u karantinu "

Administratori mogu da [prikažu, puste ili izbrišu ove poruke.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Da biste otvorili bezbednosni & centar za usaglašavanje, idite na lokaciju [https://protection.office.com](https://protection.office.com/) . Idite na stranicu "karantin" da biste je otvorili direktno [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Možete pretraživati po sledećim vrednostima:  

- **ID poruke**: univerzalni jedinstveni identifikator poruke. Ako izaberete poruku na listi, vrednost **ID poruke** će se pojaviti u oknu " **Detalji** " koji se pojavljuje. Administratori mogu da koriste [praćenje poruka](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) da bi pronašli poruke i njihove odgovarajuće ID vrednosti poruka.
- **E-adresa pošiljaoca**: adresa e-pošte jednog pošiljaoca.
- **E-adresa primaoca**: e-adresa jednog primaoca.
- **Tema**: koristite čitavu temu poruke. Pretraga ne razlikuje mala i velika slova.

Nakon što ste uneli kriterijume pretrage, kliknite na ![ dugme "Osveži" ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Osveži** da biste filtrirali rezultate.  

Cmdlet omogućava korišćenje za prikaz i upravljanje porukama i datotekama u karantinu:
- [Izbriši-Neu karantin](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [EXPORT-u karantin](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [-U Karantinda](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-Ukarantu u karantin](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Imajte na umu da je ova cmdonly samo za poruke, a ne za datoteke MALVERA iz ATP-a za SharePoint online, OneDrive za poslovanje ili timove.
- [Pusti to](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)