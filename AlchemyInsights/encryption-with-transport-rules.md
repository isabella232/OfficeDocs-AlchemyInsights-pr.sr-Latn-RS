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
ms.openlocfilehash: e1f8227047daede71d0fa3b3557db0d95a379b99b76ab0c2fe1d6ed8cc213d4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079464"
---
# <a name="encryption-with-transport-rules"></a>Šifriranje pomoću pravila za prenos

U [Exchange Centru administracije](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) možete da koristite Office Message Encryption (OME) mogućnosti u pravilima protoka pošte da biste aktivirali šifrovanje poruke. U uslovu pravila za prenos izaberite opciju **Primena Office 365 zaštita šifrovanja poruka i prava**.

- Za više informacija pogledajte članak [Definisanje pravila protoka pošte da šifruju](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- U programu PowerShell koristite [Novo pravilo za prenos](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) cmdlet i podesite parametar *Primena OME* na $true.
