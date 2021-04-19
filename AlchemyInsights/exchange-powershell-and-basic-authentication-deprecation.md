---
title: Exchange PowerShell i osnovna zastarela potvrda identiteta
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
- "3500011"
- "4577"
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813486"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="63898-102">Exchange PowerShell i osnovna zastarela potvrda identiteta</span><span class="sxs-lookup"><span data-stu-id="63898-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="63898-103">Najnovije informacije o tome kako da se povežete sa uslugom Exchange Online PowerShell bez upotrebe osnovne potvrde identiteta [potražite ovde](https://aka.ms/exops-docs).</span><span class="sxs-lookup"><span data-stu-id="63898-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/exops-docs).</span></span> <span data-ttu-id="63898-104">Modul PowerShell V2 ne koristi osnovnu potvrdu identiteta.</span><span class="sxs-lookup"><span data-stu-id="63898-104">The PowerShell V2 module does not use basic authentication.</span></span>

<span data-ttu-id="63898-105">Imajte u vidu da Osnovna potvrda identiteta i dalje mora da bude omogućena na klijentskom računaru.</span><span class="sxs-lookup"><span data-stu-id="63898-105">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="63898-106">Novi modul programa PowerShell v2 koristi modernu potvrdu identiteta za uspostavljanje veze za omogućavanje svih V2 cmdlet zasnovanih na REST.</span><span class="sxs-lookup"><span data-stu-id="63898-106">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="63898-107">Pored V2 cmdlets, omogućava vam i da pristupate starijim daljinskim PowerShell (RPS) Cmdlets koje zahtevaju daljinsku PowerShell sesiju da bude uspostavljena.</span><span class="sxs-lookup"><span data-stu-id="63898-107">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="63898-108">Uspostavljanje RPS sesije na Windows računaru zahteva da WinRM osnovna potvrda identiteta bude omogućena na računaru klijenta iako modul koristi mehanizam moderne potvrde identiteta za potvrdu identiteta usluge.</span><span class="sxs-lookup"><span data-stu-id="63898-108">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="63898-109">WinRM kanal osnovne potvrde identiteta se koristi za prenošenje tokena moderne potvrde identiteta.</span><span class="sxs-lookup"><span data-stu-id="63898-109">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="63898-110">Ako se WinRM kanal osnovne potvrde identiteta onemogući na računaru klijenta, novi V2 cmdlet nastaviće da radi (ali stariji RPS cmdlets neće).</span><span class="sxs-lookup"><span data-stu-id="63898-110">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
