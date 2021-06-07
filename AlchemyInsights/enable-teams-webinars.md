---
title: Omogućavanje Teams veinara
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/04/2021
ms.locfileid: "52793780"
---
# <a name="enable-teams-webinars"></a>Omogućavanje Teams veinara

Velineri su podrazumevano omogućeni. Možete da upravljate ko može da planira i registruje termine za Teams tako što ćete koristiti Teams PowerShell komande.

- Svi korisnici koji mogu da kreiraju sastanak takođe mogu da kreiraju sastanak u veb pregledaču. Ako želite da upravljate ko može da planira Teams na vebinarima, *koristite AllowMeetingRegistration*. 
- Prema podrazumevanim *postavkama, opcija WhoCanRegister* je omogućena i postavljena na **Svi.** Ako želite da isključite registraciju za sastanak, *postavite vrednost AllowMeetingRegistration na* **Netačno.**

Da biste promenili ove postavke, morate da [instalirate Teams PowerShell](/microsoftteams/teams-powershell-install). Takođe, smernice za sastanke primenjene su na Teams velinera. Na primer, ako je anonimno pridruživanje isključeno u postavkama sastanka, anonimni korisnici ne mogu da se pridruže vebinarima.

Da biste saznali više o konfigurisanju ko može da se registruje za vebinar, pogledajte konfigurisanje ko može da se [registruje za vebinare.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars) Dodatne informacije o postavkama za Microsoft liste potražite u [članku Postavke kontrole za Microsoft liste.](/sharepoint/control-lists)