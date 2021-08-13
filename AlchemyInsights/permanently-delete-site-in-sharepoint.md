---
title: Trajno brisanje sajta u sistemu SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: f461963c4a5719957258349d667731231023721ab3ee4641538c94371bf3f56d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53944325"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a>Trajno brisanje sajta u sistemu SharePoint

Da biste ponovo koristili URL adresu sa izbrisanog sajta (radi ponovnog kreiranja sajta) ili da biste trajno izbrisali sajt zato što više nije u upotrebi, možete da koristite opciju **Trajno izbriši** u novom SharePoint centru administracije. 

1. Idite na [stranicu „Izbrisani sajtovi“ u novom SharePoint centru administracije](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) i prijavite se pomoću naloga koji ima administratorske dozvole za organizaciju. 

2. U levoj koloni izaberite sajt. 

3. Izaberite stavku **Trajno izbriši**. 

**Napomena**: Nije moguće trajno izbrisati sajtove povezane sa grupama u novom SharePoint centru administracije. Umesto toga ćete morati da koristite [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite).  

Više informacija potražite u članku [Trajno brisanje sajta](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site). 
