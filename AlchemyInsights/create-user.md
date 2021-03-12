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
ms.openlocfilehash: 742ff857141d08031302fdcff7e49b3eef90e0f7
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747025"
---
# <a name="create-user"></a>Kreiranje korisnika

**ЉTEN**

- [Ukidanje podrške za prijavljivanje na WebView iz Google 2021-a počevši od 4](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) . Testiranje da li utiču na aplikacije tako što ćete pratiti [Google Google](https://go.microsoft.com/fwlink/?linkid=2157323) da bi testirao kompatibilnost.
- Uverite se da koristite sistemski Veb prikaz ili pregledač sistema kada prijavljivanjem korisnicima koristite Google Google naloge. Više informacija potražite u članku [problemi sa prijavljivanjem u aplikacije pomoću samo pregledača](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).

**Ne mogu da kreiram novog korisnika u Azure katalogu oglasa**

1. Uverite se da ste ovlašćeni da kreirate novi standardni korisnik. Samo uloga globalnog administratora ili administratora u usluzi Azure Active Directory (AD) može da kreira novi standardni korisnik. Ako niste na jednoj od ovih uloga, zamolite administratora da vas doda na jednu od ovih uloga ili da kreira novi korisnički nalog.
1. Uverite se da je korisničko ime u domenu koji je verifikovan u Azure AD. Ako nemate nijedna verifikovana prilagođena imena domena u Azure AD, možete da koristite Azure AD AD početno domen koji se završava *. onmicrosoft.com.
1. Uverite se da je korisničko ime u domenu koje nije vezano za Azure AD iz lokalnog oglasa. Korisnici ne mogu da se dodaju u oblaku sa imenima domena koje su u lokalnoj organizaciji.
1. Uverite se da nijedan drugi korisnik ili kontakt već nema korisničko ime koje želite da dodelite novom korisniku. Korisnička imena moraju biti jedinstvena u okviru Azure AD.
1. Pogledajte [AZURE AD uloge i administratore](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) za Azure oglas.
1. Pogledajte [imena domena](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) za AZURE oglas.
1. Pregledajte [evidenciju nadzora](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) da biste videli detaljnije informacije o nedavno kreiranom ili izbrisanom korisniku kao ko je izvršio radnju i kada.
1. Više informacija o dodavanju novih korisnika potražite u članku [Korišćenje Azure portala za kreiranje novog korisnika u AZURE AD](/azure/active-directory/active-directory-users-create-azure-portal).
1. [AZURE AD administrativne uloge](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles): dozvole za administratorske uloge u usluzi Azure Active Directory
1. Možete da [koristite Azure AD PowerShell da biste kreirali novi korisnik](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).
