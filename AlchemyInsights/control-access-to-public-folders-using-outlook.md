---
title: Kontrola pristupa javnim fasciklama pomoću Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 1386b97f804e63455094abf64b9d9e2541d57dafa36535813b0d7689e0ce2966
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54032572"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Kontrola pristupa javnim fasciklama pomoću Outlook

Da biste kontrolisali koji korisnici mogu da pristupe javnim fasciklama Outlook:

1. Koristite `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: Omogućite korisnicima da pristupe javnim fasciklama u Outlook  
$false: Sprečite korisnički pristup javnim fasciklama u Outlook. Ovo je podrazumevana vrednost.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Napom: Ova procedura može da kontroliše samo veze sa Outlook računarom Windows klijentima. Korisnici mogu da nastave da pristupe javnim fasciklama koristeći program OWA Outlook za Mac.

Dodatne informacije potražite u [temi Kontrolisane veze sa javnim fasciklama u Outlook](https://aka.ms/controlpf) za više informacija.
