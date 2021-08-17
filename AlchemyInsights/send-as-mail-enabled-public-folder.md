---
title: Send As Mail Enabled Public Folder in EXO
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: 22aa3e8f46c2ff4f62cb520b9498041dffb9d3a3eb607d788cc97b10bf32dbb5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052580"
---
# <a name="sendas-mail-enabled-public-folder"></a>SendAs Mail Enabled Public Folder

Sledeći primer dodeljuje dozvole "Pošalji kao" za poštanske javne fascikle NewPF1 korisniku Jason.

Add-RecipientPermission -Identity 'NewPF1' -Trustee "Jason" -AccessRights 'SendAs'

Detaljnu sintaksu i informacije o parametrima potražite u temi Dodela [dozvola "Pošalji kao"](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs)ili "Pošalji u ime" za javne fascikle omogućene za poštu.

