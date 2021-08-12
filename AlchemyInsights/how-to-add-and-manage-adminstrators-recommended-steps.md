---
title: Kako da dodate administratore i upravljate im – preporučeni koraci
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: 5aa6f11d31ed62078fdd05090af5722289544c5ab2244a369182f4e0f9214183
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963801"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>Kako da dodate administratore i upravljate im – preporučeni koraci

Na osnovu opisa problema, pronašli smo rešenje za vas. Većina klijenata je sama rešila problem nakon što su pratili dokumentaciju.

**Uređivanje administratora pretplate ili koaumenata**

- Administrator naloga može da uređuje obe uloge, dok administrator pretplate može da promeni samo administratore za koautore na [Azure portalu.](https://ms.portal.azure.com/#home)
- [Dodavanje ili promena administratora pretplate na Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Ažuriranje administratora pretplate ili Co-Administrator za unutrašnje (AIRS) pretplate**

Administrator usluge ili administrator koautora mogu sami da služe ovoj radnji na sledeći način:

1. Prijavite se na [Azure portal i kliknite](https://ms.portal.azure.com/#home) na upravljanje **troškovima + naplata na** levom blejdu.
2. Kliknite na stavku reda sa pretplatom. To otvara pregled za pretplatu.
3. Na **bleju pretplate izaberite** stavku **Svojstva.** 
4. Kliknite na **dugme "Administ za** uslugu".
5. Unesite adresu e-pošte korisnika koga želite da postavite za administratora usluge i kliknite na dugme **U redu.**

**Dodavanje/promena/uklanjanje koad administratora**

1. Prijavite se na [Azure portal](https://ms.portal.azure.com/#home) kao administrator usluge.
2. Otvorite [pretplate i](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) izaberite pretplatu. (Koadministratori mogu da se dodele samo u e-pošti pretplate.)
3. Pređite na klasičnu kontrolu pristupa **(IAM)** Klasični administratori Dodajte koadmini administratore da biste otvorili okno Dodavanje koadminimenata (Ako je onemogućena opcija Dodavanje  >    >    >   koadministira,  ona vam saoseća da nemate dozvole).
4. Izaberite korisnika koga želite da dodate i kliknite na **dugme Dodaj**.

**uči više:**
- [Dodavanje koadmenata](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Uklanjanje koad administratora](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Promena administratora usluge](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Prikaz administratora naloga](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Upravljanje pristupom pomoću RBAC i Azure portala](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Dodavanje/brisanje korisnika pomoću Azure Active Directory (AD)**

Možete da dodate nove korisnike ili izbrišete postojeće korisnike iz Azure Active Directory (Azure AD) organizacije:

1. Da biste dodali novog korisnika, prijavite se na [Azure portal](https://ms.portal.azure.com/#home) kao administrator korisnika za organizaciju.
2. Izaberite **Azure Active Directory**, izaberite stavku **Korisnici, a** zatim stavku **Novi korisnik.**
3. Na stranici **Korisnik** popunite potrebne informacije. Izaberite **stavku Kreiraj.** Korisnik se kreira i dodaje u Azure AD zakupca.

**Saznajte više:**

- [Dodavanje novog korisnika](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Brisanje korisnika](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Dodavanje ili ažuriranje informacija o korisničkom profilu pomoću Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Preporučeni dokumenti**

- [Šta je kontrola pristupa zasnovana na ulogama (RBAC)?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Razumevanje različitih uloga u programu Azure](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Administratorske dozvole za uloge u Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Uputstvo: Odobravanje pristupa korisniku pomoću RBAC i Azure portala](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Rešavanje problema sa RBAC u Azure](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Organizovanje resursa sa Azure grupama za upravljanje](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Kako da zatražite kopiju Azure fakture putem e-pošte](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [Dodavanje, ažuriranje ili uklanjanje kreditne ili debitne kartice iz usluge Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Upravljanje (ponovo aktiviraj/otkaži/promeni) pretplatom](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



