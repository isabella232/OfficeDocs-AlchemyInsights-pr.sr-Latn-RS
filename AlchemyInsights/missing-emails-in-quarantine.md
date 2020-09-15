---
title: Nedostaju e-poruke u karantinu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673728"
---
# <a name="missing-emails-in-quarantine"></a>Nedostaju e-poruke u karantinu "

Administratori mogu da [prikažu, oslobode ili izbrišu ove poruke.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Da biste otvorili bezbednosni & centar za usaglašenost, idite na [https://protection.office.com](https://protection.office.com/) . Da biste otvorili stranicu karantina direktno, idite na [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Možete da pretražujete po sledećim vrednostima:  

- **ID poruke**: globalni Jedinstveni identifikator poruke. Ako na listi izaberete poruku, vrednost ID-a  **poruke**  se pojavljuje u oknu "razmeni za  **detalje**  " koji se pojavljuje. Administratori mogu da koriste [praćenje poruka](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) da bi pronašli poruke i ODGOVARAJUĆE vrednosti ID-a poruka.
- **Adresa pošiljaoca**: e-adresa jednog pošiljaoca.
- **Adresa e-pošte primaoca**: e-adresa za primaoca.
- **Tema**: koristite celu temu poruke. Pretraga ne razlikuje mala i velika slova.

Kada unesete kriterijume pretrage, kliknite na dugme ![ Osveži ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **osvežavanje** dugmeta da biste filtrirali rezultate.  

Cmdlet koji koristite za prikazivanje poruka i datoteka u karantinu su:
- [Brisanje iz karantina poruka](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Izvoz-poruka u karantinu](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Poruka u karantinu](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Pregled u karantinu](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Imajte na umu da je ova cmdlet poruka samo za poruke, a ne za datoteke malver sa ATP-a za SharePoint online, OneDrive for Business ili timove.
- [Izdanje-karantin poruka](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)