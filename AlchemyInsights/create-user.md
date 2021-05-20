---
title: Kreiranje korisnika
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: 800baae2d748708d8cb7a5fb0e73fce5dcf455cb
ms.sourcegitcommit: 2d617ae59eed0ce8b571339ceefce6473c03b94c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 05/19/2021
ms.locfileid: "52569761"
---
# <a name="create-user"></a>Kreiranje korisnika

**OBJAVA:**

- [Ukidanje podrške za prijavljivanje na WebView iz usluge Google od 4. januara 2021.](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) Testirajte da li aplikacija može da utiče tako što ćete pratiti [uputstva](https://go.microsoft.com/fwlink/?linkid=2157323) google za testiranje kompatibilnosti.
- Uverite se da koristite veb pregled sistema ili pregledač sistema kada se prijavljujte korisnicima sa korisničkim Google nalozima. Više informacija potražite u [temi Problemi sa prijavljivanjem u aplikacije samo pomoću pregledača Chrome.](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)

**Ne mogu da kreiram novog korisnika u Azure AD direktorijumu**

1. Uverite se da ste ovlašćeni za kreiranje novog standardnog korisnika. Samo uloga globalnog administratora ili administratora Azure Active Directory (AD) može da kreira novog standardnog korisnika. Ako niste u jednoj od ovih uloga, zatražite od administratora da vas doda u jednu od ovih uloga ili da vam kreira novi korisnički nalog.
1. Uverite se da se korisničko ime nalazi u domenu koji je verifikovan u vašoj Azure AD. Ako nemate verifikovana prilagođena imena domena u Azure AD, možete da koristite početni domen Azure AD koji se završava sa *.onmicrosoft.com.
1. Uverite se da se korisničko ime nalazi u domenu koji nije federan za Azure AD iz vaše bele AD mreže. Korisnici ne mogu da se dodaju u oblak sa imenima domena koja su sačinjena iz izvora iz izvora.
1. Uverite se da nijedan drugi korisnik ili kontakt već nema korisničko ime koje želite da dodelite novom korisniku. Korisnička imena moraju biti jedinstvena u Azure AD- u.
1. Pogledajte [Azure AD uloge i administratore](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) za Azure AD.
1. Pogledajte imena [domena](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) za Azure AD.
1. Pregledajte [evidenciju nadzora](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) da biste videli detaljnije informacije o nedavno kreiranom ili izbrisanom korisniku kao što su ko je izvršio radnju i kada.
1. Više informacija o dodavanju novih korisnika potražite u temi Korišćenje Azure portala za kreiranje novog korisnika [u Azure AD- u](/azure/active-directory/active-directory-users-create-azure-portal).
1. [Azure AD administrativne uloge:](/azure/active-directory/active-directory-assign-admin-roles)Administratorske dozvole za uloge u Azure Active Directory
1. Možete da [koristite i Azure AD PowerShell da biste kreirali novog korisnika.](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)
