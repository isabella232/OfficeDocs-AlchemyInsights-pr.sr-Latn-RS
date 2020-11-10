---
title: Greška u OneDrive prijavljivanju AADSTS50011
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982544"
---
# <a name="onedrive-login-error-aadsts50011"></a>Greška u OneDrive prijavljivanju AADSTS50011

Ako primite grešku "AADSTS50011: URL adresa odgovora navedena u zahtevu se ne podudara sa odgovorom" kada se prijavite u OneDrive aplikaciji, potražite sledeće:

Vaša OneDrive verzija treba da bude jednaka ili veća od verzije 20.052. XXXX. XXXX. Da biste provjerili verziju, kliknite na ikonu Blue OneDrive na sistemskoj traci poslova, izaberite stavku **pomoć & postavkama > postavkama >**.

Vaša mreža blokira saobraćaj na **g.live.com** i **oneclient.sfx.MS**. Ako je taj saobraćaj blokiran, OneDrive ne može sama da se ažurira. Radite sa administratorom mreže da biste se uverili da imate pristup tim URL adresama. [Ove krajnje tačke](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) treba da se pristupačnu za klijente pomoću Microsoft 365 planova.

Ako treba da ručno nabavite trenutnu verziju usluge OneDrive, posetite [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
