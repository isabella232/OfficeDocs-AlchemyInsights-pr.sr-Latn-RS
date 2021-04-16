---
title: Šifriranje pomoću pravila za prenos
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
- "9002635"
- "5154"
ms.openlocfilehash: dfd77bc83b4b278e3630858f54fdfb109ade2a14
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813882"
---
# <a name="encryption-with-transport-rules"></a>Šifriranje pomoću pravila za prenos

U [Exchange Centru administracije](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) možete da koristite Office Message Encryption (OME) mogućnosti u pravilima protoka pošte da biste aktivirali šifrovanje poruke. U uslovu pravila za prenos izaberite opciju **Primena Office 365 zaštita šifrovanja poruka i prava**.

- Za više informacija pogledajte članak [Definisanje pravila protoka pošte da šifruju](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- U programu PowerShell koristite [Novo pravilo za prenos](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) cmdlet i podesite parametar *Primena OME* na $true.
