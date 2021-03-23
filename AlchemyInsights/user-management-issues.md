---
title: Problemi sa upravljanjem korisnika
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037507"
---
# <a name="user-management-issues"></a>Problemi sa upravljanjem korisnika

**Šta se događa sa trenutnim dodeljenim korisnicima aplikacije ako onemogućim nekretninu ' potrebna dodela korisnika ' (postavljanje ovog polja na ne)?**

**Obavezno onemogućavanje dodeljivanja korisnika** ne utiče na trenutno dodeljene korisnike. Onemogućavanje ovog vlasništva dozvoliće svim korisnicima da pristupe aplikaciji. Svi navedeni korisnici i korisnici dodeljeni grupama u aplikaciji i dalje će biti važeći.

- Da biste ograničili aplikaciju na određeni skupa korisnika, pogledajte članak- [ograničavanje aplikacije Azure AD za skupa korisnika – Microsoft Platform identiteta | Microsoft docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).
- Da biste dodelili korisnike i grupe, pomoću poslovnih aplikacija u usluzi Azure Active Directory (Azure AD), iz unutar Azure portala ili pomoću programa PowerShell pogledajte članak [Upravljanje korisničkim zadatkom za aplikaciju u usluzi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).
- Da biste delegirali dozvole za kreiranje aplikacija i upravljanje, pogledajte članak [administratorske dozvole za upravljanje administratorom aplikacije – Azure AD | Microsoft docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).
- **Skrivanje određenih poslovnih aplikacija od korisnika** – koristite sledeće korake da biste sakrili sve Microsoft 365 aplikacije iz panela **myapps** . Aplikacije će i dalje biti vidljive na Office 365 portalu.

 1. Prijavite se na Azure portal kao globalni administrator za vaš direktorijum. 
 2. Izaberite **Azure Active Directory**. 
 3. Izbor **korisnika**. 
 4. Izaberite stavku **korisničke postavke**. 
 5. U okviru **poslovne aplikacije** izaberite stavku **Upravljanje kako krajnji korisnici pokreću i prikazuju njihove aplikacije**. 
 6. **Korisnici mogu da vide samo office 365 aplikacije na office 365 portalu**, kliknite na dugme **da**. 
 7. Kliknite na dugme **Sačuvaj**. 
 8. Više detalja potražite u članku [skrivanje poslovne aplikacije iz korisničkog iskustva u Azure AD | Microsoft docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)

- Ako ponudite softver kao aplikaciju usluge (Seas) za mnoge organizacije, možete da konfigurišete aplikaciju da prihvata prijavljivanje iz bilo kog Azure aktivnog direktorijuma (Azure AD) stanara. Ova konfiguracija se zove "pravljenje multistanara aplikacije". Korisnici u bilo kom Azure AD zakupcu će moći da se prijave u aplikaciju posle saglasnosti da koriste svoj nalog sa aplikacijom. Više informacija potražite u članku [pravljenje aplikacija koje se prijave na lokaciji Azure AD korisnici-Microsoft Platform identiteta | Microsoft docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).

- **Kako krajnji korisnik može da pristupi aplikaciji kada se on/ona dodeli aplikaciji?**

Svaka aplikacija na sečaju poslovne aplikacije ima veze za pristup krajnjim korisnicima. Korisnici takođe mogu da pristupe aplikaciji kroz **Myapps** portal na jednostavan način.

- **Želite da znate koje aplikacije i tipove aplikacija koriste korisnici?**

Izveštaje za prijavljivanje možete da preuzmete za poslednjih 30 dana od **portal.azure.com > Azure Active directory> prijavljivanjem> preuzimanja izveštaja**.

- Saznajte kako da [odobrite pristup širokoj administrativnoj administraciji na aplikaciju](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) i [podesite način na koji će krajnji korisnici pristati na aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent).

- Razumevanje [načina funkcionisanja pristanka](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) i [upravljanja pristajete na aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests).


