---
title: Rešavanje problema savet o bezbednosti otkrivanja prevara
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: c7ee1fcc887a3221b5f2acda1aa6ae6beb03cb96686d4ecb7828a02f8ff48302
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955980"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Rešavanje problema savet o bezbednosti otkrivanja prevara

Ako dobijate e-savet o bezbednosti sa natpisom "Pošiljalac nije uspeo da proveri otkrivanje prevare i možda nije onaj ko izgleda kao da jeste", pošiljalac nije uspeo da prosledi DKIM ili SPF provere identiteta. Najbolji metod da to rešite jeste da pošiljalac ovlasti sebe. Ako pošiljalac šalje u vaše ime, morate da ga ovlastite tako što ćete dodati IP adresu pošiljaoca u SPF zapis.
  
Više [informacija potražite u članku Rešavanje problema savet o bezbednosti otkrivanju](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) prevara u crvenim savet o bezbednosti otkrivanju prevara.
  
Evo još nekih veza koje vam mogu pomoći:
  
- [Kako Microsoft koristi spominjanje smernica za pošiljaoca (SPF) za sprečavanje predstavljanja](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Podešavanje spF-a da biste sprečili da se šalju iskažu](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
