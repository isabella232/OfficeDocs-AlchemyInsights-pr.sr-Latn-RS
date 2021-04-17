---
title: Rešavanje problema sa savetom za bezbednost za provere otkrivanja prevara
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
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834745"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Rešavanje problema sa savetom za bezbednost za provere otkrivanja prevara

Ako dobijate bezbednosni savet u kome piše "Pošiljalac nije uspeo da proveri otkrivanje prevare i možda nije onaj ko izgleda kao da jeste", pošiljalac nije uspeo da prosledi DKIM ili SPF provere identiteta. Najbolji metod da to rešite jeste da pošiljalac ovlasti sebe. Ako pošiljalac šalje u vaše ime, morate da ga ovlastite tako što ćete dodati IP adresu pošiljaoca u SPF zapis.
  
Više [informacija potražite u članku Rešavanje problema sa crvenom (sumnjivom)](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) bezbednosnom savetom za provere otkrivanja prevare.
  
Evo još nekih veza koje vam mogu pomoći:
  
- [Kako Microsoft koristi spominjanje smernica za pošiljaoca (SPF) za sprečavanje predstavljanja](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Podešavanje spF-a da biste sprečili da se šalju iskažu](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
