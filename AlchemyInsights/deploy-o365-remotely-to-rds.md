---
title: Primena Microsoft 365 aplikacija za preduzeća za zajedničku upotrebu na RDS, Terminal serveru ili VANDI
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: a57be7fcf9d8236a51dc4b38e33ad1c2ac717f11
ms.sourcegitcommit: 2eab0980268e08a58014459d44a08a1cc34a17d4
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200687"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Primena Microsoft 365 aplikacija za preduzeća za zajedničku upotrebu na RDS, Terminal serveru ili VANDI

Da biste primenili Microsoft 365 aplikacije za Enterprise pomoću usluga udaljenog računara (RDS), nekada nazvane usluge terminala:

- Morate da imate Microsoft 365 za posao plan ili Office 365 plan koji uključuje Microsoft 365 aplikacije za Enterprise, kao što je Office 365 Enterprise E3 ili Enterprise E5.
   > [!NOTE]
   > Microsoft 365 aplikacije za preduzeća i Microsoft 365 poslovni planovi ne uključujući Microsoft 365 aplikacije za Enterprise.
- Morate omogućiti [Aktiviranje deljene računara](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> Takođe možete da preuzmete i uradite [Microsoft pomoćnik za podršku i oporavak](https://aka.ms/SaRA_OfficeSCA_M365Portal) da biste instalirali Microsoft 365 aplikacije za Enterprise u režimu izvršavanja deljenog računara.

Više informacija o preduslovima, uputstvima za podešavanje i smernicama za prilagođene instalacije pomoću alatke za primenu sistema Office potražite u članku [Primena Microsoft 365 aplikacija za preduzeća pomoću usluga udaljenog računara](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

Da biste rešili greške u vezi sa aktivacijom deljenog računara:

- Pogledajte članak [Rešavanje problema sa aktivacijom deljenog računara za Microsoft 365 aplikacije za Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Pogledajte članak [Resetovanje stanja aktivacije usluge Microsoft 365 Apps za preduzeće](https://go.microsoft.com/fwlink/?linkid=2109218).

Ako želite da instalirate Microsoft 365 aplikacije za Enterprise na sajtu RDS iz Microsoft 365 centra administracije, ***koje koristi podrazumevane postavke instalacije***, koristite sledeće korake:

1. Potvrdite koju pretplatu imate. [Saznajte kako](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2. Ako je potrebno, prebacite se na drugačiju pretplatu. [Saznajte kako](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3. Ako je Office već instaliran na RDS serveru pomoću drugih Microsoft pretplata, deinstalirajte ga. Na primer, tako što ćete otići na **kontrolnu tablu** za  >  **Deinstaliranje programa**. Deinstalirajte pomoću [Microsoft pomoćnika za podršku i oporavak](https://aka.ms/SARA-OfficeUninstall-Alchemy) Ako nailazite na probleme.
4. Na RDS serveru, prijavite se u Microsoft 365 centar administracije pomoću administratorskog naloga i [instalirajte Microsoft 365 aplikacije za Enterprise](https://portal.office.com/OLS/MySoftware.aspx).
5. Kada se Office instalira, ***Nemojte otvarati ili se prijavljivanjem*** u bilo koju Office aplikaciju.
6. Na RDS serveru, omogućite aktiviranje deljenog računara uređivanjem registratora tako što ćete pratiti ove korake:
   1. Kliknite desnim tasterom miša na dugme Windows u donjem levom uglu ekrana i izaberite stavku **pokrene**. U polju otvori otkucajte alatku **rigedit**, a zatim kliknite na **dugme u redu**.
   2. Kliknite na dugme **da** kada vam bude zatraženo da omogućite uređivaču registratora da napravi promene na uređaju.
   3. U uređivaču registratora Dodajte vrednost niske **Sharedkompjuterlicenciranja** sa podešavanjem 1 u okviru HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\clicktorun\url konfiguracione.
   4. Na RDS serveru, ***Prijavite se kao krajnji korisnik*** i [Proverite da li je aktivacija deljenog računara omogućena za Microsoft 365 aplikacije za Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).
