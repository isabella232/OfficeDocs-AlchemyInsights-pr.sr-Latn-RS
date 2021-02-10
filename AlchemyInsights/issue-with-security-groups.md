---
title: Problem sa bezbednosnim grupama
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177631"
---
# <a name="issue-with-security-groups"></a>Problem sa bezbednosnim grupama

**Ako dobijate grešku na mreži AADDS104**

Nevažeća pravila mrežne bezbednosne grupe su Najčešći uzroci mrežnih grešaka za usluge Azure Active Directory (AD DS). Bezbednosna grupa za mrežu za virtuelnu mrežu mora da omogući pristup određenim portima i protokolima. Ako su ovi portovi blokirani, Azure platforma ne može da nadgleda niti ažurira kontrolisano domen. Takođe je uključen sinhronizacija između Azure oglasa i Azure oglasa. Uverite se da su podrazumevani portovi otvoreni da biste izbegli prekid u usluzi usluge.

Da biste razumeli i rešili uobičajena obaveštenja za probleme sa konfiguracijom bezbednosti mreže, pogledajte članak [Dodavanje i verifikacija bezbednosnih grupa](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).
