---
title: Pristup je odbijen prilikom pregledanja toka posla
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 710775e8b2dee98969df7a4c8410a3e61181aaf6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688816"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="2e6ae-102">Pristup je odbijen prilikom pregledanja toka posla</span><span class="sxs-lookup"><span data-stu-id="2e6ae-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="2e6ae-103">SharePoint 2013 tokovi posla koji pokušavaju da pošalju e-poruku u SharePoint grupu mogu da ne uspeju sa porukom o grešci "pristup nije dozvoljen" Ako članstvo SharePoint grupe nije podešeno na sve.</span><span class="sxs-lookup"><span data-stu-id="2e6ae-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="2e6ae-104">**Da biste rešili ovaj problem, uradite sledeće:**</span><span class="sxs-lookup"><span data-stu-id="2e6ae-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="2e6ae-105">Omogućite svima da vide članove SharePoint grupe.</span><span class="sxs-lookup"><span data-stu-id="2e6ae-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="2e6ae-106">Uklonite SharePoint grupu iz reda "za" ili "CC" e-pošte.</span><span class="sxs-lookup"><span data-stu-id="2e6ae-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="2e6ae-107">Eksplicitno dodajte korisnike u red "za" ili "CC" Ako se vidljivost članstva ne može promeniti za SharePoint grupu.</span><span class="sxs-lookup"><span data-stu-id="2e6ae-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="2e6ae-108">Da biste videli više detalja, pogledajte [http neovlašćeno na/_vti_bin/Client.svc/SP.Utilities.Utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="2e6ae-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  