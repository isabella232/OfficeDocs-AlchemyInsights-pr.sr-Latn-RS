---
title: Dodeljivanje grupa ka usluzi Azure AD
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
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885396"
---
# <a name="assigning-groups-to-azure-ad-role"></a>Dodeljivanje grupa ka usluzi Azure AD

Da biste dodelili Azure AD grupu sa izvorom autoriteta u Azure AD u ulozi Azure oglasa, obavite sledeće korake:

1. Kreirajte novu grupu – da biste kreirali novu grupu:

    Neko. Prijavite se u centar za Azure AD administracije sa **privilegiranom administratorom uloge** ili dozvolama za **Opšte administratore** .
    -. Izaberite **Azure Active Directory > grupe > sve grupe > nova grupa**.
    trojku. Kreirajte grupu.

2. Dodelite ulogu grupi ili kada se grupa kreira.

    Neko. Da biste grupi dodelili ulogu u vreme kreiranja grupe, prebacivanje na opciju preklopnika **Azure oglasa može biti dodeljeno grupi** i Kreiranje grupe.
    -. Da biste dodelili ulogu grupi nakon kreiranja, pređite na karticu **dodeljene uloge** za novu grupu i dodelite joj ulogu.  

**Upravljanje članstvom grupe koja je dodeljena usluzi Azure AD**

Da biste sprečili podizanje privilegija, podrazumevano, samo privilegovani administratori uloga i globalni administratori mogu da izmene članstvo grupe koja je dodeljena ulozi. Međutim, oni mogu da izaberu da dodele vlasnika za takvu grupu i delegatu ovaj zadatak.

Više detalja o dodeljivanju grupa oblaka usluzi Azure AD uloge potražite u članku [dodeljivanje uloga u grupi Cloud](https://docs.microsoft.com/azure/active-directory/roles/groups-concept). Da biste saznali više o rešavanju problema sa ulogama u oblaku, pogledajte članak [Rešavanje problema sa grupama u oblaku](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).





