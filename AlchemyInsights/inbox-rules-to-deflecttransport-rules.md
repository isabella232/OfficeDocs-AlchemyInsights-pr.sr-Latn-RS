---
title: 929 pravila prijemnog poštanskog sandučeta u pravilima transporta
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
- "929"
- "1800021"
ms.assetid: 9733ef4e-db8d-4345-a072-c251480875a1
ms.openlocfilehash: abb729c40fb87bcca8cc03c95aa4677597d20c08
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47778705"
---
# <a name="mail-flow-rules-also-known-as-transport-rules"></a><span data-ttu-id="d0911-102">Pravila toka pošte (poznata i kao pravila transporta)</span><span class="sxs-lookup"><span data-stu-id="d0911-102">Mail flow rules (also known as transport rules)</span></span>

- <span data-ttu-id="d0911-103">Opšta pregleda pravila toka pošte: [pravila toka pošte (pravila transporta) u usluzi Exchange online](https://technet.microsoft.com/library/jj919238.aspx)</span><span class="sxs-lookup"><span data-stu-id="d0911-103">General overview of mail flow rules: [Mail flow rules (transport rules) in Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span></span>

- <span data-ttu-id="d0911-104">Podešavanje pravila toka pošte: [procedure pravila toka pošte u usluzi Exchange online](https://technet.microsoft.com/library/dn600436.aspx)</span><span class="sxs-lookup"><span data-stu-id="d0911-104">Setup mail flow rules: [Mail flow rule procedures in Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span></span>

- <span data-ttu-id="d0911-105">Kreiranje, izmena i brisanje pravila toka e-pošte: [Upravljanje pravilima toka pošte](https://technet.microsoft.com/library/jj657505.aspx)</span><span class="sxs-lookup"><span data-stu-id="d0911-105">Create, modify, and delete mail flow rules: [Manage mail flow rules](https://technet.microsoft.com/library/jj657505.aspx)</span></span>

<span data-ttu-id="d0911-106">Možete da upravljate i pravilima pošte u usluzi Exchange online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d0911-106">You can also manage mail flow rules in Exchange Online PowerShell.</span></span> <span data-ttu-id="d0911-107">Više informacija potražite u članku [Nabavite-transportrli](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (prikaz), [novo-transportrljavanje](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) [(kreiranje](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) ), [Uklanjanje-Transportrla](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (brisanje), [komplet transporta](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (izmenite postojeće), [Onemogući-transportrla](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (Onemogući postojeće)</span><span class="sxs-lookup"><span data-stu-id="d0911-107">For more information, see [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (view), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (create), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (delete), [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (modify existing), [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (disable existing), and [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (enable existing).</span></span>

<span data-ttu-id="d0911-108">Dodatni protoci protoka e-pošte (cmdlet): [Nabavite-Transportiradna radnja](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (dostupne radnje), [Nabavite-Transportpredikat](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (dostupni uslovi i izuzeci), [izvoz-transportrnacollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (izvoz pravila) i [Uvoz-transportrlecollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (uvoz pravila).</span><span class="sxs-lookup"><span data-stu-id="d0911-108">Additional mail flow rule cmdlets: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (list available actions), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (list available conditions and exceptions), [Export-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (export rules), and [Import-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (import rules).</span></span>
