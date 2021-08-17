---
title: Pravljenje SharePoint sajta
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: bf9380727fff415357884a5122e633f2254337d3db50e2b8656d94938f76d394
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54080904"
---
# <a name="create-a-sharepoint-site"></a>Pravljenje SharePoint sajta

Kreirajte sajtove iz [aktivnih sajtova](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) ili upravljajte njima u SharePoint centru za upravljanje. Dodatne informacije potražite [u članku Upravljanje sajtovima SharePoint centru za administvene lokacije.](https://docs.microsoft.com/sharepoint/manage-site-creation) 

## <a name="tips"></a>Saveti:

- Ne **možete** da kreirate lokaciju sa istim URL adresom postojeće lokacije. Ako ste izbrisali lokaciju i želite da ponovo koristite URL, moguće je da izbrisana lokacija i dalje postoji u okviru [Izbrisane lokacije.](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true) Lokacija mora biti trajno izbrisana da bi se ponovo koristila URL adresa. Da biste potpuno uklonili lokaciju sa programom PowerShell, pogledajte primer cmdlet stavke [Remove-SPSite.](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)
- Neki korisnici možda neće moći da kreiraju lokaciju. [Pogledajte upravljanje kreiranjem sajta u SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).
- Moguće je da je sajt zaglavljen pri **kreiranju duže nego** što je očekivano. Ako je prošlo više od 24 časa od kada ste prvi put videli ovaj problem, prijavite tiket za podršku. U mnogim slučajevima već radimo na rešenju. Dajte nam najmanje 24 sata da dovršimo rešenje.
