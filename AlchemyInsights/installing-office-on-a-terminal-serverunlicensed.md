---
title: Installing office on a Terminal Server - Unlicensed
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
ms.openlocfilehash: 35ef317ea87fedd01c08fee5b370e3c81e515c27
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/13/2021
ms.locfileid: "58322013"
---
# <a name="installing-office-on-a-terminal-server"></a>Instaliranje Kancelarija na terminalnom serveru

Za primenu Microsoft 365 Apps za preduzeće na Windows serveru pomoću usluga udaljene radne površine (RDS), ranije imenovanih usluga terminala:
  
- Morate imati pretplatu na Microsoft 365 koja uključuje Microsoft 365 Apps za preduzeće, na primer Office 365 Enterprise E3 ili Enterprise E5. Planovi Microsoft 365 aplikacije za posao i Microsoft 365 aplikacije za posao Premium ne uključuju Microsoft 365 Apps za preduzeće.

- Morate da omogućite [aktivaciju deljenog računara.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

Ako želite da instalirate operativni Microsoft 365 Apps za preduzeće RDS sa lokacije ***Microsoft 365 centar administracije,*** koja koristi podrazumevane postavke instalacije, koristite sledeće korake.

    **Tip**: You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.
  
1. Proverite Microsoft 365 pretplatu. [Saznajte kako](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Ako je potrebno, prebacite se Microsoft 365 na drugu pretplatu. [Saznajte kako](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Ako Kancelarija na RDS serveru pomoću bilo kojih drugih pretplata na Microsoft 365, deinstaliranje. Na primer, tako što ćete ići na \> kontrolnu tablu, deinstalujte program. Deinstalujte [koristeći Microsoft Pomoćnik za podršku i oporavak](https://aka.ms/SARA-OfficeUninstall-Alchemy) ako se naiđete na probleme.

4. Na RDS serveru se prijavite u Microsoft 365 centar administracije sa administratorskim nalogom i instalirajte [Microsoft 365 Apps za preduzeće.](https://portal.office.com/OLS/MySoftware.aspx)

5. Kada Kancelarija instalirate, ***ne otvarajte aplikacije*** niti se prijavavajte u Kancelarija aplikacije.

6. Na RDS serveru omogućite aktivaciju deljenog računara tako što će urediti registrator tako što će pratiti ove korake:

1. Kliknite desnim tasterom miša Windows dugme u donjem levom uglu ekrana i izaberite stavku Pokreni. U polju Otvori otkucajte **regedit**, a zatim kliknite na dugme U redu.

2. Kliknite na dugme Da kada vam bude zatraženo da dozvolite uređivaču registratora da unosi promene na uređaju.

3. U uređivaču registratora dodajte vrednost niske **SharedComputerLicensing** sa postavkom 1 u okviru HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Kancelarija\ClickToRun\Configuration.

7. Na RDS serveru ***se*** prijavite kao krajnji korisnik i potvrdite da je aktivacija deljenog računara omogućena [za Microsoft 365 Apps za preduzeće.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)

Više detalja o preduslovima, uputstvima za podešavanje i uputstvima za prilagođene instalacije [](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)pomoću alatke za primenu programske Kancelarija, pročitajte u Microsoft 365 Apps za preduzeće Primena pomoću usluga udaljene radne površine.
  
Da biste otklonili greške u vezi sa aktivacijama deljenog računara, pogledajte rešavanje problema sa aktivaciju deljenog računara [za Microsoft 365 Apps za preduzeće.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
  