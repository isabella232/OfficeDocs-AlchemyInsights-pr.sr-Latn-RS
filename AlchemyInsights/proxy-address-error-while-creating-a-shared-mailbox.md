---
title: Greška proxy adrese prilikom kreiranja deljenog poštanskog sandučeta
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568304"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a><span data-ttu-id="21653-102">Greška proxy adrese prilikom kreiranja poštanskog sandučeta ili drugog objekta omogućenog e-pošte</span><span class="sxs-lookup"><span data-stu-id="21653-102">Proxy address error while creating a mailbox or other email enabled object</span></span>

<span data-ttu-id="21653-103">Ako ste pokušali da kreirate objekat sa omogućenom e-poštom (poštansko sanduče, Deljeno poštansko sanduče itd.) i dobili grešku "Proxy adresa" SMTP:alias@domain.com "se već koristi...", e-adresa koju ste odabrali već je uzeta drugi objekat sa omogućenim e-adresom u organizaciji.</span><span class="sxs-lookup"><span data-stu-id="21653-103">If you tried to create an email-enabled object (mailbox, shared mailbox etc.) and received the error "The proxy address "SMTP:alias@domain.com" is already being used…", the email address you chose is already taken by another email-enabled object in your organization.</span></span>
  
<span data-ttu-id="21653-104">Potrebno je da pronađete korisnika, grupu, Deljeno poštansko sanduče ili javnu fasciklu koja ima ovu e-adresu i da je izbriše ili da promeni adresu e-pošte.</span><span class="sxs-lookup"><span data-stu-id="21653-104">You need to find the user, group, shared mailbox or public folder that has this email address and delete it or change its email address.</span></span> <span data-ttu-id="21653-105">Zatim možete da kreirate novi objekat sa omogućenom e-poštom sa oslobođenom adresom e-pošte.</span><span class="sxs-lookup"><span data-stu-id="21653-105">Then you can create a new email-enabled object with the freed email address.</span></span> <span data-ttu-id="21653-106">Koristite pretragu na matičnoj stranici da biste je pronašli.</span><span class="sxs-lookup"><span data-stu-id="21653-106">Use Search on the Home page to find it.</span></span> <span data-ttu-id="21653-107">Možete da koristite i sledeću Exchange online komandu PowerShell da biste je pretražili:</span><span class="sxs-lookup"><span data-stu-id="21653-107">You can also use the following Exchange Online PowerShell command to search for it:</span></span>

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
<span data-ttu-id="21653-108">Ako ne želite da izbrišete postojeću adresu e-pošte, odaberite novu e-adresu za novi objekat koji kreirate.</span><span class="sxs-lookup"><span data-stu-id="21653-108">If you don't want to delete the existing email address, choose a new email address for the new object you are creating.</span></span>
  