---
title: Kako se dodaju i upravljaju administratorima koji se preporučuju
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
ms.openlocfilehash: ed3aa5defabdd4f505ee4f74570023d990910dcb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755849"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>Kako se dodaju i upravljaju administratorima koji se preporučuju

Na osnovu opisa problema, našli smo rešenje za vas. Većina klijenata mogla je samostalno da rešava svoj problem nakon praćenja dokumentacije.

**Uređivanje administratora pretplate ili Koadministratora**

- Administrator naloga može da uredi obe uloge dok administrator pretplate može da promeni samo Koadministratore na [Azure portal](https://ms.portal.azure.com/#home).
- [Dodavanje ili promena Azure administratora pretplate](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Ažuriranje administratora pretplate ili Co-Administrator za interne (EMITNE) pretplate**

Administrator usluge ili koadministrator može samouslužiti ovu radnju pomoću sledećih koraka:

1. Prijavite se na [Azure portal](https://ms.portal.azure.com/#home) i izaberite stavku **Upravljanje troškovima + naplata** u levom Blejku.
2. Kliknite na stavku predmeta sa pretplatom. Otvoriće se pregled pretplate.
3. Na oštrici **pretplate** kliknite na dugme **Svojstva**. 
4. Kliknite na dugme **administratora usluge** .
5. Unesite e-poruku korisnika koju želite da postaviљ kao administrator usluge i kliknite na dugme **u redu**.

**Dodavanje/promena/uklanjanje Koadministratora**

1. Prijavite se na [Azure portal](https://ms.portal.azure.com/#home) kao administrator usluge.
2. Otvorite [pretplate](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) i izaberite pretplatu. (Saradnici se mogu dodeliti samo na nivou pretplate.)
3. Pređite na **Access Control (iam)**  >  **Classic administratori**  >  **dodaju**  >  **programski koadministrator** da bi otvorili okno " **Dodavanje koadministracije** " (ako je opcija "Dodaj koadministrator" onemogućiti, označava da nemate dozvole).
4. Izaberite korisnika kojeg želite da dodate i kliknite na dugme **Dodaj**.

**uči više:**
- [Dodavanje Koadministratora](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Uklanjanje koadministratora](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Promena administratora usluge](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Prikaz administratora naloga](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Upravljanje pristupom koristeći RBAC i Azure portal](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Dodavanje/brisanje korisnika pomoću usluge Azure Active Directory (AD)**

Možete da dodate nove korisnike ili da izbrišete postojeće korisnike iz usluge Azure Active Directory (Azure AD):

1. Da biste dodali novog korisnika, prijavite se na [Azure portal](https://ms.portal.azure.com/#home) kao korisnički administrator za organizaciju.
2. Izaberite stavku **Azure Active Directory**, izaberite stavku **Korisnici** , a zatim stavku **novi korisnik**.
3. Na stranici **korisnik** popunite potrebne informacije. Kliknite na dugme **Kreiraj**. Korisnik se kreira i dodaje u vaš Azure AD stanar.

**Saznajte više**:

- [Dodavanje novog korisnika](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Brisanje korisnika](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Dodavanje ili ažuriranje informacija o profilu pomoću usluge Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Preporučeni dokumenti**

- [Šta je to Kontrola pristupa zasnovan na ulozi (RBAC)?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Razumevanje raznih uloga u Azure](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Dozvole za administratorske uloge u usluzi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Uputstvo: dodelite pristup korisniku koji koristi RBAC i Azure portal](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Rešavanje problema sa RBAC u Azure](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Organizovanje resursa pomoću usluge Azure Management](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Kako tražiti kopiju Azure fakture putem e-pošte](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [Kako da dodate, ažurirate ili uklonite kreditnu ili debitnu karticu sa lokacije Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Upravljanje pretplatom (ponovo Aktiviraj/Otkaži/zameni)](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



