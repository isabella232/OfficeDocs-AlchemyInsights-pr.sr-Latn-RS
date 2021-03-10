---
title: Prosleđivanje e-poruke tako što će obezbediti ID mrežne poruke
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: e4a0a3d9b4fede9198c8a235d05945b30a6e0807
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695383"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a><span data-ttu-id="ab64f-102">Prosleđivanje e-poruke tako što će obezbediti ID mrežne poruke</span><span class="sxs-lookup"><span data-stu-id="ab64f-102">Submit an email message by providing the network message ID</span></span>

1. <span data-ttu-id="ab64f-103">U **novom programu prosleđivanja** , izaberite stavku **e-pošta** i **ID poruke na mreži**.</span><span class="sxs-lookup"><span data-stu-id="ab64f-103">In the **New submission** flyout, select **Email** and **Network Message ID**.</span></span>
2. <span data-ttu-id="ab64f-104">Slijedite ove korake da biste pronašli ID poruke za e-poruku u programu Outlook:</span><span class="sxs-lookup"><span data-stu-id="ab64f-104">Follow these steps to find the message ID for an email message in Outlook:</span></span>
    1. <span data-ttu-id="ab64f-105">Kliknite dvaput na e-poruku da biste je otvorili.</span><span class="sxs-lookup"><span data-stu-id="ab64f-105">Double-click the email message to open it.</span></span>
    1. <span data-ttu-id="ab64f-106">Izaberite stavku  >  **Svojstva** datoteke.</span><span class="sxs-lookup"><span data-stu-id="ab64f-106">Select **File** > **Properties**.</span></span>
    1. <span data-ttu-id="ab64f-107">Otvorite Notepad ili prazan Word dokument, a zatim kopiju i nalepite sadržaj koji se nalazi u okviru " **Internet zaglavlja** " u otvorenom dokumentu radi bolje vidljivosti.</span><span class="sxs-lookup"><span data-stu-id="ab64f-107">Open Notepad or a blank Word document, and then copy and paste the content found in the **Internet headers** box into the open document for better visibility.</span></span>
    1. <span data-ttu-id="ab64f-108">Pronađite polje **X-MS-Exchange-organizacija-ID-poruka** .</span><span class="sxs-lookup"><span data-stu-id="ab64f-108">Locate the **X-MS-Exchange-Organization-Network-Message-Id** field.</span></span> <span data-ttu-id="ab64f-109">Vrednost posle **:** predstavlja ID koji vam je potreban za prosleđivanje.</span><span class="sxs-lookup"><span data-stu-id="ab64f-109">The value after the **:** is the ID you need for your submission.</span></span>
3. <span data-ttu-id="ab64f-110">Ako je e-pošta sletela u fasciklu "Neželjena pošta" za sve primaoce ove e- **poruke, odaberite** **stavku "Izaberi sve**".</span><span class="sxs-lookup"><span data-stu-id="ab64f-110">Under **Recipients**, if the email landed in the junk mail folder for all recipients of this email, choose **Select All**.</span></span> <span data-ttu-id="ab64f-111">Ako nije, izaberite samo korisnika koji je prijavio problem.</span><span class="sxs-lookup"><span data-stu-id="ab64f-111">If not, select only the user who reported the issue.</span></span>
4. <span data-ttu-id="ab64f-112">U okviru **razlog za prosleđivanje**, ako izaberete **treba da bude blokirano**, navedite da li je poruka trebalo da bude blokirana kao **bezvredna**, **phishing** ili **malver**, a zatim izaberite stavku **Prosledi**.</span><span class="sxs-lookup"><span data-stu-id="ab64f-112">Under **Reason for submission**, if you select **Should have been blocked**, specify whether the message should have been blocked as **Spam**, **Phishing**, or **Malware**, and then select **Submit**.</span></span>

<span data-ttu-id="ab64f-113">Da biste saznali više, pogledajte [Kako da prosledite osumnjičene bezvredne pošte, frish, URL adrese i datoteke korporaciji Microsoft za skeniranje](https://go.microsoft.com/fwlink/?linkid=2101479).</span><span class="sxs-lookup"><span data-stu-id="ab64f-113">To learn more, see [How to submit suspected spam, phish, URLs, and files to Microsoft for scanning](https://go.microsoft.com/fwlink/?linkid=2101479).</span></span>
