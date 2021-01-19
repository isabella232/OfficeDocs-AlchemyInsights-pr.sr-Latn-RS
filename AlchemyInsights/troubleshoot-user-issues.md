---
title: Rešavanje problema sa korisnicima
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7813"
- "9004358"
ms.openlocfilehash: d9964e50bdea0c41ac14ab3783b579034b5f2c8c
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901336"
---
# <a name="announcements"></a>Avu

Sledi Google Google na testiranje kompatibilnosti da biste testirali da li utiču na aplikacije. Vodič Google-a je dostupan https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support .

Uverite se da koristite sistemski Veb prikaz ili pregledač sistema prilikom prijavljivanja korisnicima pomoću korisnika Google naloga. Više informacija potražite u članku [problemi sa prijavljivanjem u aplikacije pomoću samo pregledača](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).


**Ne mogu da kreiram novog korisnika u Azure katalogu oglasa**

Da biste rešili problem da ne možete da kreirate novog korisnika u usluzi Azure AD, obavite sledeće korake:

1. Uverite se da ste ovlašćeni da kreirate novi standardni korisnik. Samo uloga globalnog administratora ili administratora u usluzi Azure Active Directory (AD) može da kreira novi standardni korisnik. Ako niste na jednoj od ovih uloga, zamolite administratora da vas doda na jednu od ovih uloga ili da kreira novi korisnički nalog.
2. Uverite se da je korisničko ime u domenu koji je verifikovan u Azure AD. Ako nemate nijedna verifikovana prilagođena imena domena u Azure AD, možete da koristite Azure AD AD početno domen koji se završava *. onmicrosoft.com.
3. Uverite se da je korisničko ime u domenu koje nije vezano za Azure AD iz lokalnog oglasa. Korisnici ne mogu da se dodaju u oblaku sa imenima domena koje su u lokalnoj organizaciji.
4. Uverite se da nijedan drugi korisnik ili kontakt već nema korisničko ime koje želite da dodelite novom korisniku. Korisnička imena moraju biti jedinstvena u okviru Azure AD.
5. Pogledajte [AZURE AD uloge i administratore](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) za Azure oglas.
6. Pogledajte [imena domena](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Domains) za AZURE oglas.
7. Pregledajte [evidenciju nadzora](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Audit) da biste videli detaljnije informacije o nedavno kreiranom ili izbrisanom korisniku kao ko je izvršio radnju i kada.
8. Više informacija o dodavanju novih korisnika potražite u članku [Korišćenje Azure portala za kreiranje novog korisnika u AZURE AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory) .
9. Više informacija o dozvolama za uloge administratora u usluzi Azure AD potražite u članku [AZURE AD administracije](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference).
10. Detalje o kreiranju korisnika pomoću usluge Azure AD PowerShell potražite u članku [AZURE AD PowerShell za kreiranje novog korisnika](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser).

**Problem sa prijavom samouuslugom**

Da biste rešili probleme u vezi sa samouslužnim prijavljivanjem, obavite sledeće korake:

1. Da biste koristili samouslužno prijavljivanje pomoću aplikacija, prvo omogućite samouslužno prijavljivanje za zakupca. 
2. Da biste aplikaciji omogućili da podržava samouslužno prijavljivanje, dodajte ga u protok korisnika. Kada sledeći put odete na stranicu za prijavljivanje za tu aplikaciju, videćete opciju **_bez naloga? Kreiraj jednu!_* _. Tako će započeti proces prijavljivanja.
3. Informacije o tome kako se koristi samouslužni prijavljivanje za popunjavanje organizacije u usluzi Azure AD potražite u članku [Samouslužno prijavljivanje za AZURE AD](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-self-service-signup).
4. Kada korisnički protok povežete sa jednom ili više aplikacija, korisnici koji posećuju aplikaciju moći će da se prijave i steknu nalog gosta pomoću opcija koje su podešene u toku korisnika. Više informacija o prijavljivanju i dobianju naloga gosta, korisnici mogu da vide [samouslužni prijavljivanje za korisnike gosta](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow).

*Problem pozivanjem spoljnog korisnika**

Da biste rešili probleme u vezi sa pozivanjem spoljnog korisnika, uradite sledeće:

Uverite se da ste poslali korisničku pozivnicu na e-adresu koja se podudara sa imenom sa kojom se korisnik prijavljuje. Ako pošaljete poziv na proxy e-adresu korisnika, korisnik ne može da je iskoristi. Više informacija potražite u članku [Azure AD B2B dokumentacija](https://docs.microsoft.com/azure/active-directory/external-identities/).

**Ne mogu da dodeljujemo licence korisniku**

Da biste rešili probleme sa dodeljivanjem licenci korisniku, obavite sledeće korake:

1. Da biste upravljali korisničkim licencama, uverite se da koristite nalog sa jednom od potrebnih administratorskih uloga: globalni administrator, administrator licenci ili administrator korisnika. Ulogu korisnika možete da potvrdite na kartici **uloga direktorijuma** na korisničkom Blejku.
2. Ako koristite Azure portal i dodela licenci se ne primenjuju, kliknite na obaveštenje u gornjem desnom uglu. Ovo otvara nož sa detaljima o tome šta nije u redu. U većini slučajeva to je dovoljno da shvati i reši problem.
3. Da bi licenci mogla da se dodeli korisnik, uverite se da je postavljeno **mesto upotrebe** za korisnika. Proverite da li je taj objekat postavljen tako što ćete prikazati karticu **profil** na korisničkom Blejku.
4. Uverite se da postoje dovoljne licence za proizvod koji pokušavate da dodelite. Možete da vidite broj dostupnih licenci na sajtu Azure, na lokaciji [Azure Active Directory-> licence – > sve proizvode](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/LicensesMenuBlade/Products).
5. Korisnik možda već ima drugu licencu čije usluge su neusaglašene sa onima u novoj licenci koju pokušavate da dodelite. Na primer, ako je korisnik omogućio Exchange Online (plan 1), nećete moći da dodelite licencu pomoću usluge Exchange Online (plan 2). Onemogućite jednu od usluga da biste omogućili novu dodelu licenci. Ako koristite Azure portal ili PowerShell cmdlet, stranica sa detaljima o **problemu** navodi određene usluge koje uzrokuju neusaglašenost.
6. Ako pokušavate da uklonite licencu, a to ne uspe, korisnik može imati druge licence sa uslugama koje zavise od usluga koje pokušavate da uklonite. Ako koristite Azure portal ili PowerShell cmdlet stavku, poruka o grešci navodi specifične usluge koje imaju zavisne stavke.
7. Ako želite da razumete zašto je licenca dodata/uklonjena od korisnika (na primer, ko je još u organizaciji možda napravio promene), potvrdite izbor u polju za evidenciju nadzora. Postavljanje filtera na **aktivnosti licenciranja** za prikazivanje svih izmena, uključujući "glumca" koji ih je izvršio.
8. Ako koristite Exchange online, neki korisnici u zakupcu mogu biti nepravilno konfigurisani sa istom vrednošću proxy adrese. U takvim slučajevima možete videti opšte poruke o grešci kada operacija licenciranja ne uspe. [Ovaj članak](https://docs.microsoft.com/exchange/troubleshoot/administration/proxy-address-being-used) sadrži više informacija o ovom problemu, uključujući informacije o tome [Kako da se povežete sa uslugom Exchange online pomoću udaljenog PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell). Da biste identifikovali korisnike u zakupcu, sadrže istu proxy adresu, uradite ovo Exchange online cmdlet:

Beћati

Get-Recipient | Gde je {$/. E-adrese – podudaranje <user principal name> } | for name, RecipientType, e-adrese





