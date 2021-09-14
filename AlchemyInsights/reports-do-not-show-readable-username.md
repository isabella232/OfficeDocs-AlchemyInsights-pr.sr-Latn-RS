---
title: Izveštaji u Microsoft 365 centar administracije ne prikazuju čitanje korisničkog imena
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/02/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13809"
- "13810"
- "13812"
- "9008619"
ms.openlocfilehash: 16aa4f052c934421423c73244f03a20aa38e4785
ms.sourcegitcommit: 76c61dec041b93d0039764fae38107108da324aa
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/04/2021
ms.locfileid: "59316197"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Izveštaji u Microsoft 365 centar administracije ne prikazuju čitanje korisničkog imena

Izveštaji u programu Microsoft 365 centar administracije ne prikazuju korisnička imena, već alfanumeričke vrednosti kao što je B2BC6C15BB9FCDEA71E5CD302D228CC8.

Ovo je očekivano ponašanje i objavilo ga je centar za poruke (MC275344, objavljeno u izdanju Aug. 3, 2021). 

Globalni administratori mogu da preusmere ovu promenu za zakupu i prikažu informacije koje mogu identifikovati korisnika ako to dozvoljavaju prakse privatnosti organizacije. Da biste promenili promenu za zakuca, treba da ga promenite:

1. U centru Postavke postavke za org , a zatim  >    >  [](https://admin.microsoft.com/Adminportal/Home#/Settings/Services)izaberite stavku **Izveštaji**. 
1. U **okviru Odaberite kako da se prikažu informacije** o korisniku izaberite stavku Prikaži **informacije** o korisniku koje mogu identifikovati u izveštajima , a zatim ponovo pokrenite izveštaj.