---
title: Primena Microsoft 365 Apps za preduzeće za deljenu upotrebu na sistemima RDS, Terminal Server ili VDI
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
ms.openlocfilehash: b8df97c19937a757c1de9865b6c7b8d1cddfd62d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325617"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Primena Microsoft 365 Apps za preduzeće za deljenu upotrebu na sistemima RDS, Terminal Server ili VDI

Da biste primenili Microsoft 365 Apps za preduzeće usluge udaljene radne površine (RDS), koje su se ranije zvale usluge terminala:

- Morate da imate Microsoft 365 for Business plan ili Office 365 plan koji obuhvata Microsoft 365 Apps za preduzeće, na primer Office 365 Enterprise E3 ili Enterprise E5.
   **Napomi:** Microsoft 365 aplikacije za posao i Microsoft 365 Business Standard ne uključuju Microsoft 365 Apps za preduzeće.
- Morate omogućiti [aktivaciju deljenog računara.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

**Napomi:** Microsoft aplikaciju možete i da preuzmete i pokrenete da [biste Pomoćnik za podršku i oporavak](https://aka.ms/SaRA_OfficeSCA_M365Portal) instalirali Microsoft 365 Apps za preduzeće u režimu aktivacije deljenog računara.

Dodatne informacije o preduslovima, uputstvima za podešavanje i uputstvima za prilagođene instalacije [](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)pomoću alatke za primenu programske Kancelarija potražite u Microsoft 365 Apps za preduzeće Primena pomoću usluga udaljene radne površine.

Da biste otklonili greške u vezi sa aktivacije deljenog računara:

- Pogledajte rešavanje [problema sa aktivaciju deljenog računara za Microsoft 365 Apps za preduzeće.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
- Pogledajte članak [Resetovanje stanja aktivacije usluge Microsoft 365 Apps za preduzeće](https://go.microsoft.com/fwlink/?linkid=2109218).

Ako želite da instalirate operativni Microsoft 365 Apps za preduzeće RDS sa lokacije ***Microsoft 365 centar administracije,*** koja koristi podrazumevane postavke instalacije, koristite sledeće korake:

1. Proverite pretplatu. [Saznajte kako.](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)
2. Ako je potrebno, prebacite se na drugu pretplatu. [Saznajte kako.](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)
3. Ako Kancelarija na RDS serveru pomoću bilo koje druge Microsoft pretplate, deinstaliranje. Na primer, tako što ćete **ići na**  >  **kontrolnu tablu , deinstalujte program**. Deinstalujte [koristeći Microsoft Pomoćnik za podršku i oporavak](https://aka.ms/SARA-OfficeUninstall-Alchemy) ako se naiđete na probleme.
4. Na RDS serveru se prijavite u Microsoft 365 centar administracije sa administratorskim nalogom i instalirajte [Microsoft 365 Apps za preduzeće.](https://portal.office.com/OLS/MySoftware.aspx)
5. Kada Kancelarija aplikacije, ***ne otvarajte*** aplikacije niti se prijavite Kancelarija aplikacijama.
6. Na RDS serveru omogućite aktivaciju deljenog računara tako što će urediti registrator tako što će pratiti ove korake:
   1. Kliknite desnim tasterom miša Windows dugme u donjem levom uglu ekrana i izaberite stavku **Pokreni**. U polju Otvori otkucajte **regedit**, a zatim kliknite na dugme **U redu**.
   2. Kliknite na **dugme Da** kada vam bude zatraženo da dozvolite uređivaču registratora da unosi promene na uređaju.
   3. U uređivaču registratora dodajte vrednost niske **SharedComputerLicensing** sa postavkom 1 u okviru HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Kancelarija\ClickToRun\Configuration.
   4. Na RDS serveru ***se*** prijavite kao krajnji korisnik i potvrdite da je aktivacija deljenog računara omogućena [za Microsoft 365 Apps za preduzeće.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)
