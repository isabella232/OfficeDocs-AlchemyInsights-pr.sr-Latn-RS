---
title: Agregejgrupsanduče full NDR Primljeno za e-poštu koja se šalje u Microsoft 365 Group
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004286"
- "7656"
ms.openlocfilehash: 9de09ab4cbd2f09648305b11da6273ed990907cf
ms.sourcegitcommit: 2ffdf6096de5608b117c6677d3cd7dd4c23ea024
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 12/18/2020
ms.locfileid: "49722081"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>Agregejgrupsanduče full NDR Primljeno za e-poštu koja se šalje u Microsoft 365 Group

Koristite sledeće komandno polje za EXO Shell da biste kreirali Exchange pravilo za transport za nepristupačnog otpuštanje e-poruka poslatih u agregat Group

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> Zamenite SMTP adresu u **-sentto** sa SMTP adresom grupe agregat Group u zakupcu. SMTP adresu agregatne grupe poštanskog sandučeta možete da nabavite od primljene NDR.



