---
title: Rešen je problem štampanja na čekanju
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 66b39434ef6f9ad2b8392f811704e67c1bcffd2b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801855"
---
# <a name="print-spooler-issue-is-resolved"></a>Rešen je problem štampanja na čekanju

Ako se uređaj ažurira pomoću operativnog sistema Windows 10  **OS Build 19041,329**, možda ste videli problem gde se određeni štampači ne štampaju. Upravljač štampanja na čekanju može da napravi grešku ili se neočekivano zatvori prilikom pokušaja štampanja, a nijedan izlaz ne potiče od štampača koji je uticao na njega. Ovaj problem je rešen u OS Build  **19041,331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).  

**Trenutna istraga**

Datoteka datoteke lokalnog bezbednosnog autoriteta za uslugu lokalne bezbednosti (LSASS) (**Isass.exe**) može da ne uspe na nekoj uređaju sa porukom o grešci "kritični sistemski proces, C:\WINDOWS\system32\Isass.exe, nije uspeo sa statusnim kodom c0000008. Mašina se sada mora ponovo pokrenuti ".  **Microsoft radi na rezoluciji i obezbediće ispravku u narednom izdanju.**

Više informacija potražite u  [verzijama poznatih problema sa operativnim sistemom Windows 10 Version 2004](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).