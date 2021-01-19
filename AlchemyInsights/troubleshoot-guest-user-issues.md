---
title: Rešavanje problema sa korisničkim problemima
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004358"
- "7822"
ms.openlocfilehash: 0f2a10b918fee067b167ab58ac2544a89e0c8ea1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901588"
---
# <a name="troubleshoot-guest-user-issues"></a>Rešavanje problema sa korisničkim problemima

1. Za uputstva o upravljanju pristupom gostu aplikacije pogledajte članak [Upravljanje pristupom gostu sa Azure AD Access ocenama](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews).
1. [Dodajte korisnike gosta u direktorijum na Azure portalu](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal): u ovom novom početku ćete dodati novog gosta korisnika u vaš Azure katalog usluge putem Azure portala, poslati pozivnicu i videti kako izgleda proces iskupljenja korisnika gosta.
1. [Dodajte korisnika gosta sa PowerShell](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell): u ovom jaskom ћivotu, koristite komandu New-AzureADMSInvitation da biste dodali jednog korisnika gosta u vaš Azure stanar.
1. Da biste saznali kako da dodelite korisnike i grupe, preduzećima aplikacijama u usluzi Azure Active Directory (Azure AD), u okviru Azure portala ili pomoću programa PowerShell pogledajte [članak Upravljanje korisničkim zadatkom za aplikaciju u programu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal). 
1. Azure Active Directory (Azure AD) B2B saradnja radi sa većini aplikacija koje se integrišu pomoću usluge Azure AD. U ovom [članku](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)hodamo kroz uputstva za konfigurisanje nekih popularnih aplikacija sahas za korišćenje sa uslugom AZURE AD B2B.
1. Kao organizacija koja koristi Azure Active Directory (Azure AD) B2B mogućnosti za saradnju za pozivanje gostiju korisnika sa partnerskih organizacija na Azure AD, sada možete da pružite pristup ovim B2B korisnicima. Ove aplikacije u lokalnoj aplikaciji mogu da koriste potvrdu identiteta zasnovanu na SAML-u ili integrisanu Windows potvrdu identiteta (IWA) sa delegiranom delegacijom ograničenja (KCD). Više informacija potražite u članku [dodeljivanje B2B korisnika u usluzi Azure AD pristup lokalnim aplikacijama](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises).
1. Saznajte kako da [dodelite lokalno kontrolisanim partnerima pristup resursima oblaka pomoću usluge Azure AD B2B Collaboration](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud).