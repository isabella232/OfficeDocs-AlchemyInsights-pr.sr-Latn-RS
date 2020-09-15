---
title: Prvi koraci uz SharePoint online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: bba89489cb75555e1f508224de223bee04e1d665
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700721"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="94720-102">Tokovi posla u sistemu SharePoint</span><span class="sxs-lookup"><span data-stu-id="94720-102">Workflows in SharePoint</span></span>

<span data-ttu-id="94720-103">Ako SharePoint tokovi posla ne šalju e-poruke, možda je organizacija naišla na ograničenja za Exchange online.</span><span class="sxs-lookup"><span data-stu-id="94720-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="94720-104">Poruka "tok posla je obustavljena" može da se pojavi ako imate jednu od sledećih stavki:</span><span class="sxs-lookup"><span data-stu-id="94720-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="94720-105">Imate tok posla u sistemu SharePoint online koji koristi SharePoint 2010 ili SharePoint 2013 tip platforme toka posla.</span><span class="sxs-lookup"><span data-stu-id="94720-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="94720-106">Tok posla je konfigurisan da šalje prilagođenu e-poruku za više od 200 korisnika po danu, više od 10.000 primalaca dnevno ili više od 30 poruka u minuti.</span><span class="sxs-lookup"><span data-stu-id="94720-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="94720-107">Kada pokrećete tok posla, e-poruka se ne šalje i primetićete da je poruka o grešci, interno postavljen na obustavljeno ili ne može da pošalje primaoca.</span><span class="sxs-lookup"><span data-stu-id="94720-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="94720-108">Više informacija potražite u sledećem [članku](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span><span class="sxs-lookup"><span data-stu-id="94720-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

