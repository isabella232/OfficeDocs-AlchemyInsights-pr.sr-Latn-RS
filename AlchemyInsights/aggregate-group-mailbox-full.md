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
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a><span data-ttu-id="b6781-102">Agregejgrupsanduče full NDR Primljeno za e-poštu koja se šalje u Microsoft 365 Group</span><span class="sxs-lookup"><span data-stu-id="b6781-102">AggregateGroupMailbox full NDR received for email sent to Microsoft 365 group</span></span>

<span data-ttu-id="b6781-103">Koristite sledeće komandno polje za EXO Shell da biste kreirali Exchange pravilo za transport za nepristupačnog otpuštanje e-poruka poslatih u agregat Group</span><span class="sxs-lookup"><span data-stu-id="b6781-103">Use the following EXO Shell command to create an Exchange transport rule to silently drop emails sent to aggregate group mailbox:</span></span>

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> <span data-ttu-id="b6781-104">Zamenite SMTP adresu u **-sentto** sa SMTP adresom grupe agregat Group u zakupcu.</span><span class="sxs-lookup"><span data-stu-id="b6781-104">Replace the SMTP address in **-SentTo** with SMTP address of aggregate group mailbox in your tenant.</span></span> <span data-ttu-id="b6781-105">SMTP adresu agregatne grupe poštanskog sandučeta možete da nabavite od primljene NDR.</span><span class="sxs-lookup"><span data-stu-id="b6781-105">You can get the SMTP address of aggregate group mailbox from the NDR received.</span></span>



