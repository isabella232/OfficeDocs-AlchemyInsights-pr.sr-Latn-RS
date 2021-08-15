---
title: E-poruke koje nedostaju u karantinu
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 900d5f250846e9a7046f72156c150f4970d91d5ad94cb7fc054952228f4bf257
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54026236"
---
# <a name="missing-emails-in-quarantine"></a>E-poruke koje nedostaju u karantinu"

Administratori mogu da [pregledaju, izbrišu ili izbrišu ove poruke.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Da biste otvorili centar & za usaglašenost, idite na [https://protection.office.com](https://protection.office.com/) . Da biste direktno otvorili stranicu Karantin, idite na [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Možete pretražiti po sledećim vrednostima:  

- **ID poruke:** Globalni jedinstveni identifikator poruke. Ako izaberete poruku sa liste, vrednost  **ID-a**  poruke se pojavljuje u  **oknu**  ileta Detalji koje se pojavljuje. Da bi pronašli poruke i njihove odgovarajuće [vrednosti](/microsoft-365/security/office-365-security/message-trace-scc) ID-a poruke, a mogu da koriste i funkciju "Praćenje poruka".
- **Adresa e-pošte** pošiljaoca: adresa e-pošte jednog pošiljaoca.
- **Adresa e-pošte** primaoca: E-adresa jednog primaoca.
- **Tema:** Koristite celu temu poruke. Pretraga ne osetljiva na velika i velika slova.

Kada unesete kriterijume za pretragu, kliknite na dugme ![ Osveži dugme ](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Osveži da** biste filtrirali rezultate.

Cmdlet grupe koje koristite za prikaz poruka i datoteka i upravljanje datotekama u karantinu su:
- [Delete-QuarantineMessage](/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](/powershell/module/exchange/preview-quarantinemessage)Imajte uvid u to da je ova cmdlet datoteka samo za poruke, a ne za malver datoteke u programu Microsoft zaštitnik za Office 365 za SharePoint Online, OneDrive for Business ili Teams.
- [Release-QuarantineMessage](/powershell/module/exchange/release-quarantinemessage)