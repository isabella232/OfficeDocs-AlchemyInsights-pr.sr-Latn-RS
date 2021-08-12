---
title: Rešavanje problema sa korisnicima sa goste
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
ms.openlocfilehash: 9e6030919721b4c0805a26ca45d365f31d88894e86ea08225f47576e7d152047
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939393"
---
# <a name="troubleshoot-guest-user-issues"></a>Rešavanje problema sa korisnicima sa goste

1. Uputstvo za upravljanje pristupom gosta aplikacijama možete da vidite u temi Upravljanje [pristupom gosta uz Azure AD preglede pristupa.](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews)
1. Dodajte korisnike sa u goste u direktorijum na [Azure portalu:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal)U ovom brzom startu ćete dodati novog korisnika sa gosta u Azure AD direktorijum putem Azure portala, poslati pozivnicu i videti kako izgleda proces eskanja poziva korisnika sa pozivima.
1. Dodavanje korisnika sa gosta uz [PowerShell:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell)U ovom brzom startu koristićete komandu "New-AzureADMSInvitation" da biste dodali jednog korisnika sa gosta u Azure zakupac.
1. Da biste saznali kako da dodelite korisnike i grupe poslovnim aplikacijama u programu Azure Active Directory (Azure AD), bilo putem Azure portala ili pomoću programa PowerShell, pogledajte upravljanje dodelom korisnika za aplikaciju u [programu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal). 
1. Azure Active Directory (Azure AD) B2B saradnja radi sa većinom aplikacija koje se integriše sa uslugom Azure AD. U ovom [članku](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)ćemo proći kroz uputstva za konfigurisanje nekih popularnih SaaS aplikacija koje će se koristiti sa uslugom Azure AD B2B.
1. Kao organizacija koja koristi mogućnosti Azure Active Directory (Azure AD) B2B saradnje za pozivanje korisnika sa upitom gosta iz partnerskih organizacija u Azure AD, sada možete ovim B2B korisnicima da obezbedite pristup svojim aplikacijama. Ove ugrađene aplikacije mogu da koriste potvrdu identiteta zasnovanu na SAML Windows-u ili integrisanu potvrdu identiteta (IWA) sa kerberos ograničenim delenosom (KCD). Dodatne informacije potražite u temi Odobravanje pristupa B2B korisnicima u [Azure AD aplikacijama.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises)
1. Saznajte kako da lokalno upravljate partnernim nalozima pristup [resursima u oblaku pomoću Azure AD B2B saradnje.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)