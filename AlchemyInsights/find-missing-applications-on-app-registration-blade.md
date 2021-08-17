---
title: Pronalaženje aplikacija koje nedostaju na blejdu registracije aplikacija
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9654"
ms.openlocfilehash: 0dee7e44a8701e1df924b9657cce6cf9d90160e58277d667f6069a4cbcf87ce5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057116"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>Pronalaženje aplikacija koje nedostaju na blejdu registracije aplikacija

1. Nije moguće pronaći aplikacije na portalu za registraciju aplikacija.

    Ako je aplikacija aplikacija sa više zakupaca i registrovana je u drugom zakupaca, neće se prikazati u okviru Blejd registracije aplikacija. Međutim, možete da ga pronađete u okviru Blejd Enterprise aplikacija kada mu se pristupi (nakon odobrenja) i kada se napravi principal usluge u zakupacu. Dodatne informacije potražite u [temi Aplikacije & u usluzi Azure AD – Microsoft platforma za identitete.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
2. Nije moguće prikazati aplikacije u registracionom bleju aplikacije čak i ako ste apliakcioni.

    Uverite se da ste u pravom direktorijumu na Azure portalu.
3. Moja aplikacija nije navedena u okviru blejda Enterprise aplikacija, ali se prikazuje kada izvršavam upit u PowerShell komandi.

    Ponekad, kada izbrišete aplikaciju sa Azure portala, ona se ne pojavi na portalu, ali možda nije u potpunosti izbrisana. Za više informacija pogledajte:
    - Možete da preuzmete listu prethodno izbrisanih aplikacija i vidite da li se aplikacija pojavljuje na listi pomoću Powershell komande: **Get-AzureADDeletedApplication**. Da biste saznali više, [pogledajte get-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication)
    - Ako u potpunosti želite da uklonite aplikaciju, možete da pokušate sledeće u programu PowerShell: **Remove-AzureADApplication -ObjectId**. Da biste saznali više, [pogledajte Remove-AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication)
    - Druga mogućnost je da pokušate da vratite izbrisanu aplikaciju u prethodno stanje pomoću sledeće Powershell komande: **Restore AzureADDeletedApplication -ObjectId**. Da biste saznali više, [pogledajte Restore-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
4. Ne mogu da pronađem listu svih unapred instaliranih poslovnih aplikacija u novom Azure zakupca.

    U Azure AD podrazumevano nema unapred instaliranih poslovnih aplikacija. Treba da je dodate ručno iz opcije "Nova aplikacija" tako što ćete je potražiti u Azure AD galeriji ili dodati aplikaciju koja nije galerija. Da biste saznali više, pogledajte [brzi start: Dodavanje aplikacije u Azure Active Directory (Azure AD) zakupca.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal)
    Ako ste globalni administrator, aplikacijama možete lako da pristupite pomoću [Microsoft 365 pokretanja aplikacija](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher).
5. Nije moguće pronaći moje aplikacije sa portala "Moje aplikacije".

    Uverite se da aplikacije nisu skrivene na stranici kolekcije "Moje aplikacije". Da biste saznali više, [pogledajte kolekcije (pregled) na portalu "Moje aplikacije" – Azure AD.](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections)
6. Da biste pokrenuli aplikacije sa portala "Moje aplikacije", pogledajte & pronalaženje aplikacija za korišćenje na portalu "Moje [aplikacije" – Azure AD.](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access)
7. Office 365 Aplikacija Mover se ne pojavljuje na blejdu Enterprise aplikacija nakon instalacije.

    Aplikacija "Office 365 Mover" je aplikacija sa više zaku ona koja ne mora da se dodaje u AAD pomoću odeljka Aplikacije galerije u okviru Registracija enterprise aplikacija. Da biste Office 365 aplikaciji Mover, samo se prijavite u aplikaciju i ona će tražiti pristanak korisnika na dozvole. Kada korisnik pruži pristanak, ova aplikacija će se automatski dodati zakupu sa ID-om e-pošte koji ste prijavljeni.

    Kada se prijavite u aplikaciju, trebalo bi da možete da pronađete unos ove aplikacije u okviru blejda Enterprise aplikacija u AAD-u. Morate da potražite tu aplikaciju tako što ćete ukucati puno ime, tj. "Office 365 Mover" ili jednostavno pretražiti "office" i ona bi trebalo da naveli aplikaciju. Da biste saznali više, pogledajte Office 365 Mover kaže da je već instaliran, ali nije naveden u galeriji [Enterprise aplikacije.](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html)
8. Brzi start: Prikaz liste aplikacija koje koriste [vaš Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) za upravljanje identitetom vam pokazuje kako da prikažete aplikacije, poznate i kao aplikacije, koje su već podešene da koriste Azure AD zakupac kao dobavljača identiteta (IdP).
9. [Rešavanje uobičajenih problema prilikom](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) dodavanja ili uklanjanja aplikacije Azure Active Directory pomaže da razumete uobičajene probleme sa kojima se ljudi suočavaju prilikom pregledanja aplikacija Azure Active Directory.
