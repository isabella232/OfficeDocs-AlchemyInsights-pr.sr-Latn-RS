---
title: S/MIME u programu Outlook na vebu
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772312"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="7709f-102">Šifrovanje e-poruka u programu Outlook</span><span class="sxs-lookup"><span data-stu-id="7709f-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="7709f-103">Šifrovanje usluge Microsoft 365 je ugrađeno u Microsoft Azure Rights Management (Azure RMS), koja je deo zaštite od Azure informacija.</span><span class="sxs-lookup"><span data-stu-id="7709f-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="7709f-104">Ako pretplata sadrži Azure Rights Management ili bezbednost informacija, **Ne morate da preduzimate nikakve radnje da biste ručno omogućili ili aktivirali** uslugu Rights Management.</span><span class="sxs-lookup"><span data-stu-id="7709f-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="7709f-105">Na osnovu povratnih informacija o klijentu, više nećemo koristiti pravila razmene Exchange pošte da biste automatski šifrovali izlaznu e-poštu koja sadrži određene osetljive informacije u zakupcu.</span><span class="sxs-lookup"><span data-stu-id="7709f-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="7709f-106">Umesto toga mi pružamo detaljna uputstva o tome kako to možete da uradite sami.</span><span class="sxs-lookup"><span data-stu-id="7709f-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="7709f-107">Dodatne detalje o tome kako da kreirate pravilo za transport za šifrovanje osetljivih informacija potražite u [ovom članku](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="7709f-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="7709f-108">Ako koristite Outlook na vebu (ranije **OWA**): prilikom sastavljanja e-poruke, jednostavno kliknite na dugme **zaštiti** u programu OWA.</span><span class="sxs-lookup"><span data-stu-id="7709f-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="7709f-109">To će primeniti "ne Prosledi" dozvolu.</span><span class="sxs-lookup"><span data-stu-id="7709f-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="7709f-110">Izaberite stavku **Promeni dozvolu** i odaberite stavku **šifrovanje** da biste šifruli poruku.</span><span class="sxs-lookup"><span data-stu-id="7709f-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="7709f-111">Ako koristite **Outlook klijent**: da biste poslali šifrovanu poruku iz programa Outlook 2013 ili 2016 ili Outlook 2016 za Mac, **Izaberite stavku**  >  **dozvole**za zaštitu, a zatim izaberite opciju zaštite koja vam je potrebna.</span><span class="sxs-lookup"><span data-stu-id="7709f-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="7709f-112">Da biste **automatski šifrovali sve e-poruke** poslate određenim primaocima ili spoljnim partnerskim organizacijama, potrebno je da kreirate pravilo za transport protoka pošte u Exchange centru administracije.</span><span class="sxs-lookup"><span data-stu-id="7709f-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="7709f-113">Detaljna uputstva se pružaju u [ovom članku podrške](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="7709f-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

