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
ms.openlocfilehash: 55b86557ec205dde2c459d76e8e330d2a8271dbec723f079e119ebe409b41c3f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031492"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Primena Microsoft 365 Apps za preduzeće za deljenu upotrebu na sistemima RDS, Terminal Server ili VDI

Da biste primenili Microsoft 365 Apps za preduzeće usluge udaljene radne površine (RDS), ranije imenovane usluge terminala:

- Morate imati plan Microsoft 365 For Business ili Office 365 plan koji obuhvata Microsoft 365 Apps za preduzeće, na primer Office 365 Enterprise E3 ili Enterprise E5.
   > [!NOTE]
   > Planovi Microsoft 365 aplikacije za posao i Microsoft 365 Business Standard ne uključuju Microsoft 365 Apps za preduzeće.
- Morate omogućiti [aktivaciju deljenog računara.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

> [!NOTE]
> Takođe možete da preuzmete i pokrenete [Microsoft Pomoćnik za podršku i oporavak](https://aka.ms/SaRA_OfficeSCA_M365Portal) da biste Microsoft 365 Apps za preduzeće u režimu aktivacije deljenog računara.

Dodatne informacije o preduslovima, uputstvima za podešavanje i uputstvima za prilagođene instalacije pomoću alatke za primenu programskih paketa Kancelarija potražite u Microsoft 365 Apps za preduzeće Primena pomoću usluga udaljene radne [površine.](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)

Da biste otklonili greške u vezi sa aktivacije deljenog računara:

- Pogledajte rešavanje [problema sa aktivaciju deljenog računara za Microsoft 365 Apps za preduzeće.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
- Pogledajte članak [Resetovanje stanja aktivacije usluge Microsoft 365 Apps za preduzeće](https://go.microsoft.com/fwlink/?linkid=2109218).

Ako želite da instalirate operativni Microsoft 365 Apps za preduzeće RDS sa lokacije Microsoft 365 centar administracije, koja koristi podrazumevane postavke ***instalacije,*** koristite sledeće korake:

1. Proverite pretplatu. [Saznajte kako.](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)
2. Ako je potrebno, prebacite se na drugu pretplatu. [Saznajte kako.](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)
3. Ako Kancelarija na RDS serveru pomoću bilo koje druge Microsoft pretplate, deinstaliranje. Na primer, tako što ćete **ići na**  >  **kontrolnu tablu , deinstalujte program**. Deinstalujte [koristeći Microsoft Pomoćnik za podršku i oporavak](https://aka.ms/SARA-OfficeUninstall-Alchemy) ako se naiđete na probleme.
4. Na RDS serveru se prijavite na nalog Microsoft 365 centar administracije administratorskim nalogom i instalirajte [aplikaciju Microsoft 365 Apps za preduzeće.](https://portal.office.com/OLS/MySoftware.aspx)
5. Kada Kancelarija aplikacije, ***ne otvarajte*** aplikacije niti se prijavavajte Kancelarija aplikacijama.
6. Na RDS serveru omogućite aktivaciju deljenog računara tako što će urediti registrator tako što će pratiti ove korake:
   1. Kliknite desnim tasterom miša Windows dugme u donjem levom uglu ekrana i izaberite stavku **Pokreni**. U polju Otvori otkucajte **regedit**, a zatim kliknite na dugme **U redu**.
   2. Kliknite na **dugme Da** kada vam bude zatraženo da dozvolite uređivaču registratora da unosi promene na uređaju.
   3. U uređivaču registratora dodajte vrednost niske **SharedComputerLicensing** sa postavkom 1 u okviru HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Kancelarija\ClickToRun\Configuration.
   4. Na RDS serveru ***se*** prijavite kao krajnji korisnik i potvrdite da je aktivacija deljenog računara omogućena [za Microsoft 365 Apps za preduzeće.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)
