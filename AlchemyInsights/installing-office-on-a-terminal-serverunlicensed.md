---
title: Instaliranje sistema Office na Terminal serveru – nelicencirani
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663131"
---
# <a name="installing-office-on-a-terminal-server"></a>Instaliranje sistema Office na Terminal serveru

Za primenu Microsoft 365 aplikacija za Enterprise na Windows serveru pomoću usluga udaljenog računara (RDS), nekadašnjih imena usluga terminala:
  
- Morate da imate Microsoft 365 pretplatu koja obuhvata Microsoft 365 aplikacije za Enterprise, kao što je Office 365 Enterprise E3 ili Enterprise E5. Microsoft 365 aplikacije za preduzeća i Microsoft 365 aplikacije za preduzeća Premium ne uključujete Microsoft 365 aplikacije za Enterprise.

- Treba da omogućite [aktivaciju deljene računara](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Ako želite da instalirate Microsoft 365 aplikacije za Enterprise na sajtu RDS iz Microsoft 365 centra administracije, ***koje koriste podrazumevane postavke instalacije***, koristite sledeće korake.

> [!TIP]
> Takođe možete da preuzmete i uradite [Microsoft pomoćnik za podršku i oporavak](https://aka.ms/SaRA_OfficeSCA_M365Portal) da biste instalirali Microsoft 365 aplikacije za Enterprise u režimu izvršavanja deljenog računara.
  
1. Potvrdite koje Microsoft 365 imate. [Saznajte kako](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Ako je potrebno, prebacite se na neku drugoj Microsoft 365 pretplatu. [Saznajte kako](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Ako je Office već instaliran na RDS serveru pomoću drugih Microsoft 365 pretplata, deinstalirajte je. Na primer, tako što ćete otići na kontrolnu tablu za \> Deinstaliranje programa. Deinstalirajte pomoću [Microsoft pomoćnika za podršku i oporavak](https://aka.ms/SARA-OfficeUninstall-Alchemy) Ako nailazite na probleme.

4. Na RDS serveru, prijavite se u Microsoft 365 centar administracije pomoću administratorskog naloga i [instalirajte Microsoft 365 aplikacije za Enterprise](https://portal.office.com/OLS/MySoftware.aspx).

5. Kada se Office instalira, ***Nemojte otvarati ili se prijavljivanjem*** u bilo koju Office aplikaciju.

6. Na RDS serveru, omogućite aktiviranje deljenog računara uređivanjem registratora tako što ćete pratiti ove korake:

1. Kliknite desnim tasterom miša na dugme Windows u donjem levom uglu ekrana i izaberite stavku pokrene. U polju otvori otkucajte alatku **rigedit**, a zatim kliknite na dugme u redu.

2. Kliknite na dugme da kada vam bude zatraženo da omogućite uređivaču registratora da napravi promene na uređaju.

3. U uređivaču registratora Dodajte vrednost niske **Sharedkompjuterlicenciranja** sa podešavanjem 1 u okviru HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\clicktorun\url konfiguracione.

7. Na RDS serveru, ***Prijavite se kao krajnji korisnik*** i [Proverite da li je aktivacija deljenog računara omogućena za Microsoft 365 aplikacije za Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Za više detalja o preduslove, uputstva za podešavanje i uputstvo za prilagođene instalacije pomoću alatke za primenu sistema Office pogledajte članak [Primena Microsoft 365 aplikacija za Enterprise pomoću usluga udaljenog računara](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
Da biste rešili greške u vezi sa aktivacijom deljenog računara, pogledajte članak [Rešavanje problema sa aktivacijom deljenih računara za Microsoft 365 aplikacije za Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  