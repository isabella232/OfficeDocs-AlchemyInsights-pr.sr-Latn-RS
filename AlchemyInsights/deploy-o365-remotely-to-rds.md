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
ms.openlocfilehash: 9d928a3bf58dedc3aaf231c8a051f87b0bbdf438
ms.sourcegitcommit: 391052026a6ce7646926d233d0fd9ba135088f79
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 10/01/2021
ms.locfileid: "60041020"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Primena Microsoft 365 Apps za preduzeće za deljenu upotrebu na sistemima RDS, Terminal Server ili VDI

Da biste Microsoft 365 aplikacije primenili usluge udaljene radne površine (RDS), ranije usluge terminala, morate da:

- Koristite jednostavnu popravku da biste omogućili TLS 1.2 kao podrazumevanu ako koristite stariju verziju sistema Windows (tj. Windows 7 SP1, Windows Server 2008 R2). Za jednostavnu popravku i više informacija pogledajte "Ažuriranje" da biste omogućili [TLS 1.1 i TLS 1.2](https://support.microsoft.com/en-us/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392#bkmk_easy)kao podrazumevane bezbedne protokole u winHTTP-u Windows. 
- Imate plan koji uključuje Microsoft 365 Apps za preduzeće (ranije Office 365 Plus). Na primer, Office 365 E3 ili Microsoft 365 E5 ili bilo koji plan koji obuhvata verziju programa Project ili Visio za računare, kao što su Project Plan 3 ili Visio Plan 2 ili Microsoft 365 Business Premium plan koji obuhvata i Microsoft 365 aplikacije za posao.
- Omogućite aktivaciju deljenog računara. Dodatne informacije potražite [u pregledu aktivacije deljenog računara za Microsoft 365 aplikacije.](https://docs.microsoft.com/deployoffice/overview-shared-computer-activation)

**Napomi:** Da biste Microsoft 365 aplikacije datoteke u režimu aktivacije deljenog računara, preuzmite [i pokrenite Microsoft Pomoćnik za podršku i oporavak.](https://docs.microsoft.com/alchemyinsights/deploy-o365-remotely-to-rds) Detalje o preduslovima, uputstvima za podešavanje i uputstvima za prilagođavanje instalacija pomoću [](https://docs.microsoft.com/deployoffice/deploy-microsoft-365-apps-remote-desktop-services)alatke za primenu programske Kancelarija, možete da vidite Microsoft 365 aplikacije primenom usluga udaljene radne površine.

Da biste otklonili greške u vezi sa aktivacije deljenog računara, pogledajte:

- [Rešavanje problema sa aktivaciju deljenog računara za Microsoft 365 aplikacije](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation)
- [Resetuj Microsoft 365 Apps za preduzeće aktivacije](https://docs.microsoft.com/office/troubleshoot/activation/reset-office-365-proplus-activation-state)

Ako želite da instalirate operativni Microsoft 365 aplikacije RDS sa lokacije Microsoft 365 centar administracije, koja koristi podrazumevane postavke instalacije, pratite ove korake:

1. Proverite koji Microsoft 365 plana imate. Dodatne informacije potražite [u temi Koju pretplatu imam?](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).

1. Ako je potrebno, prebacite se na Microsoft 365 plana. Više informacija potražite u [temi Nadogradnja na drugi plan.](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan)

1. Ako Microsoft 365 aplikacije na RDS serveru pomoću drugih nekopatibilnih planova, deinstaliranje možete da ga deinstaliranjem tako što ćete ići na kontrolnu tablu Deinstaliranje  >  **programa.** Ako naiđete na probleme, deinstalujte tako što ćete preuzeti [Microsoft Pomoćnik za podršku i oporavak.](https://aka.ms/SARA-OfficeUninstall-Alchemy)

1. Na RDS serveru se prijavite na Microsoft 365 centar administracije administratorskog naloga i [instalirajte](https://portal.office.com/OLS/MySoftware.aspx)Kancelarija.

   Kada Kancelarija aplikacije, ne otvarajte aplikacije niti se prijavite Kancelarija aplikacijama.

1. Na RDS serveru, omogućite aktivaciju deljenog računara uređivanjem registratora:

   1. Kliknite desnim tasterom miša Windows dugme "Start" u donjem levom uglu ekrana i izaberite stavku **Pokreni**. U polju Otvori otkucajte **regedit**, a zatim kliknite na dugme **U redu**.

   1. Kada budete upitani da dozvolite uređivaču registratora da unosi promene na uređaju, izaberite **da.**

   1. U uređivaču registratora, u okviru HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Kancelarija\ClickToRun\Configuration dodajte vrednost niske **SharedComputerLicensing** sa postavkom **1.**

1. Na RDS serveru se prijavite kao krajnji korisnik i potvrdite da je aktivacija deljenog računara omogućena za Microsoft 365 aplikacije. 

   Za detalje pogledajte [verifikaciju da je aktivacija deljenog računara omogućena za Microsoft 365 aplikacije.](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation#verify-that-shared-computer-activation-is-enabled-for-microsoft-365-apps)