---
title: Nije moguće aktivirati Office
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
- "2000023"
- "3509"
ms.openlocfilehash: 9a33b7880aff6016ef6df88960d6f59ac9dd50382c7e99d72ca36bc3c9f344ea
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53928383"
---
# <a name="unable-to-activate-office"></a>Nije moguće aktivirati Office

Na primer: Ako koristite stariju verziju programa Windows (na primer, Windows 7), **uverite** se da je TLS 1.2 omogućen kao podrazumevani. Više informacija potražite u temi Ažuriranje da biste omogućili [TLS 1.1 i TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)kao podrazumevane bezbedne protokole u winHTTP-u Windows.

- Proverite da li je istekao status pretplate.
- Proverite da li imate pretplatu koja dozvoljava klijentske licence, kao što su Office 365 Business ili Business Premium, i [proverite da li je korisniku dodeljena licenca](/microsoft-365/admin/manage/assign-licenses-to-users).
- Proverite da li se korisnik prijavljuje u Office sa istim nalogom na kojem ima dodeljenu licencu.
- Posetite [stranicu ispravnosti sistema Office 365](/office365/enterprise/view-service-health) da biste videli da li postoje poznati problemi sa uslugom.
- Proverite zaštitni zid, antivirusni program i postavke proxy servera da biste potvrdili da ne blokiraju pristup Microsoft 365 aplikacija internetu. Pogledajte članak [Opsezi URL i IP adresa sistema Office 365](/office365/enterprise/urls-and-ip-address-ranges "Opsezi URL i IP adresa sistema Office 365").

**Savet** Na računarima sa operativnim sistemom Windows, možemo da dijagnostikujemo nekoliko uobičajenih problema sa prijavljivanjem u Office i da ih automatski otklonimo za vas. Preuzmite i pokrenite aplikaciju  **[Microsoft pomoćnik za podršku i oporavak](https://aka.ms/SaRA-OfficeSignInScenario)** da biste koristili našu automatizovanu alatku.

Koristite sledeće radnje za rešavanju problema:

- Otvorite Office aplikaciju i [odjavite se](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) sa bilo kog postojećeg korisničkog naloga. [Uklonite](/microsoft-365/admin/manage/remove-licenses-from-users) i [ponovo dodelite](/microsoft-365/admin/manage/assign-licenses-to-users) licencu za Office, a zatim [prijavite se u Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) pomoću korisničkog naloga.
- Pokrenite [Alatku za rešavanje problema sa aktivacijom](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Resetovanje stanja aktivacije sistema Office](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Uspostavljanje početne vrednosti stanja aktivacije sistema Office")
- [Obavite popravku na mreži sistema Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

Dodatna rešenja za rešavanje problema potražite u članku:  

- [Greška „Nelicencirani proizvod“ i greška aktivacije u sistemu Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [„Žao nam je, ne možemo da se povežemo sa nalogom. Pokušajte ponovo kasnije“ – greška prilikom aktiviranja sistema Office](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)