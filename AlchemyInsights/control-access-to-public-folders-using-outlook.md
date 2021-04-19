---
title: Kontrola pristupa javnim fasciklama pomoću programa Outlook
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
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816754"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Kontrola pristupa javnim fasciklama pomoću programa Outlook

Da biste kontrolisali koji korisnici mogu da pristupe javnim fasciklama pomoću programa Outlook:

1. Koristite `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: Dozvoljavanje korisnicima da pristupe javnim fasciklama u programu Outlook  
$false: Sprečite korisnički pristup javnim fasciklama u programu Outlook. Ovo je podrazumevana vrednost.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Napom: Ova procedura može da kontroliše samo veze sa Outlook klijentima za računare za Windows. Korisnici mogu da nastave da pristupe javnim fasciklama koristeći program OWA ili Outlook za Mac.

Dodatne informacije potražite u [temi Kontrolisane veze sa javnim fasciklama u programu Outlook](https://aka.ms/controlpf) za više informacija.
