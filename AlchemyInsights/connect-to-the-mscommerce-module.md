---
title: Povezivanje sa MSCommerce modulom
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3528"
ms.openlocfilehash: 41dd044d99d14f25ea15699bfb74f7c37e3928c1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713252"
---
# <a name="connect-to-the-mscommerce-module"></a><span data-ttu-id="7f615-102">Povezivanje sa MSCommerce modulom</span><span class="sxs-lookup"><span data-stu-id="7f615-102">Connect to the MSCommerce module</span></span>

<span data-ttu-id="7f615-103">Morate biti povezani sa MSCommerce modulom da biste mogli da prikažete ili zapostavljate usluge Allowself.</span><span class="sxs-lookup"><span data-stu-id="7f615-103">You must be connected to the MSCommerce module before you can view or set the AllowSelfServicePurchase policy.</span></span>  

<span data-ttu-id="7f615-104">Da biste se povezali sa MSCommerce modulom, na PowerShell upitu (PS C: \) Unesite sledeću komandu:</span><span class="sxs-lookup"><span data-stu-id="7f615-104">To connect to the MSCommerce module, at the PowerShell prompt (PS C:\), enter the following command:</span></span>

`Connect-MSCommerce`

<span data-ttu-id="7f615-105">Otvoriće se dijalog za prijavljivanje.</span><span class="sxs-lookup"><span data-stu-id="7f615-105">This will open a sign-in dialog.</span></span> <span data-ttu-id="7f615-106">Unesite korisničko ime i lozinku za prijavljivanje.</span><span class="sxs-lookup"><span data-stu-id="7f615-106">Enter your username and password to sign-in.</span></span>

<span data-ttu-id="7f615-107">**Napomena:** &nbsp; &nbsp; Nalog koji se koristi za prijavljivanje mora biti administrator ili administrator naplate.</span><span class="sxs-lookup"><span data-stu-id="7f615-107">**NOTE:**&nbsp;&nbsp;The account used to sign in must be a Company or Billing Administrator.</span></span>
