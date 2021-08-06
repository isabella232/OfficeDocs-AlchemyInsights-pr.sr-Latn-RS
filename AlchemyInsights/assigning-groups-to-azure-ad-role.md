---
title: Dodeljivanje grupa Azure AD ulozi
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
ms.openlocfilehash: 563b1a7c93c9ca64fdea51c57b70fd2132750c4ad8ee15de0c65c9668c9c3c56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036254"
---
# <a name="assigning-groups-to-azure-ad-role"></a>Dodeljivanje grupa Azure AD ulozi

Da biste Azure AD grupi sa izvorom autoriteta u Azure AD dodelili Azure AD ulogu, izvršite sledeće korake:

1. Kreiranje nove grupe – Da biste kreirali novu grupu:

    a. Prijavite se u Azure AD centar administracije sa privilegovanim **administratorom uloga** ili **globalnim administratorskim** dozvolama.
    b. Izaberite **Azure Active Directory > Grupe > Stavku Sve > Nova grupa.**
    c. Kreirajte grupu.

2. Dodelite ulogu grupi tokom kreiranja grupe ili nakon kreiranja grupe.

    a. Da biste dodelili ulogu grupi u trenutku kreiranja grupe, prebacite preklopnik **Azure AD** uloge i kreirajte grupu.
    b. Da biste dodelili ulogu grupi nakon kreiranja, na  kartici Dodeljene uloge za novu napravljenu grupu i dodelite ulogu grupi.  

**Upravljanje članstvom u grupi koja je dodeljena Azure AD ulozi**

Da bi se sprečilo podizanje privilegija, samo privilegovani administratori i globalni administratori podrazumevano mogu da izmene članstvo grupe koja je dodeljena ulozi. Međutim, oni mogu da odaberu da dodele vlasnika za takvu grupu i delegira ovaj zadatak.

Više detalja o dodeljivanju grupa u oblaku Azure AD ulogama možete da vidite u temi Dodela [AD uloga grupi u oblaku.](https://docs.microsoft.com/azure/active-directory/roles/groups-concept) Više detalja o rešavanju problema sa ulogama dodeljenim grupama u oblaku, pogledajte rešavanje problema sa [ulogama dodeljenim grupama u oblaku.](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)





