---
title: OneDrive greške pri prijavljivanju AADSTS50011
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
ms.openlocfilehash: 80aafa2aee7213e1b77d274509a7eb9741c20b525ed97f473093ac8c6514f3c7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54112926"
---
# <a name="onedrive-login-error-aadsts50011"></a>OneDrive greške pri prijavljivanju AADSTS50011

Ako dobijete grešku "AADSTS50011: URL odgovora naveden u zahtevu se ne podudara sa odgovorom" prilikom prijave u OneDrive aplikaciju, proverite sledeće:

Vaša OneDrive verzija mora da bude jednaka ili veća od verzije 20.052.XXXX.XXXX. Da biste proverili verziju, kliknite na plavu ikonu OneDrive na sistemskoj traci poslova, izaberite **stavku Pomoć & Postavke > Postavke > O**.

Mreža može da blokira saobraćaj za **g.live.com** i **oneclient.sfx.ms.** Ako je taj saobraćaj blokiran, možete OneDrive ažurirate samu sebe. Radite sa administratorom mreže da biste se uverili da imate pristup tim UL-ama. [Te krajnje tačke treba](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) da budu dostupne klijentima koji koriste Microsoft 365 planove.

Ako treba ručno da nabavite trenutnu verziju sistema OneDrive, posetite [https://aka.ms/getonedrive](https://aka.ms/getonedrive) lokaciju .
