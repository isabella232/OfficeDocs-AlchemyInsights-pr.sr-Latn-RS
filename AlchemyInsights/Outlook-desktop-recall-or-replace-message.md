---
title: Opoziv Outlook radne površine ili zamena e-poruke
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664004"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="62bac-102">Opoziv ili zamena Outlook e-poruke</span><span class="sxs-lookup"><span data-stu-id="62bac-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="62bac-103">Kao administrator, možete da **opozovete poruke u ime korisnika pomoću programa PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="62bac-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="62bac-104">Ne možete da opozovete poruke iz centra administracije.</span><span class="sxs-lookup"><span data-stu-id="62bac-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="62bac-105">Možete da **opozovete poruke koje se šalju osobama u vašoj organizaciji**.</span><span class="sxs-lookup"><span data-stu-id="62bac-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="62bac-106">Ako je poruka poslata na gmail adresu, na primer, ne možete da je opozovete.</span><span class="sxs-lookup"><span data-stu-id="62bac-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="62bac-107">Možete **samo da opozovete poruke poslate iz programa Outlook 2016 na računaru**.</span><span class="sxs-lookup"><span data-stu-id="62bac-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="62bac-108">Ako korisnik pošalje poruku pomoću programa Outlook za Mac ili Outlook na vebu, ne možete da ga opozovete.</span><span class="sxs-lookup"><span data-stu-id="62bac-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="62bac-109">Da biste opozvali ili zamenili e-poruku:</span><span class="sxs-lookup"><span data-stu-id="62bac-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="62bac-110">U oknu sa fasciklama na levoj strani prozora programa Outlook izaberite fasciklu poslate stavke.</span><span class="sxs-lookup"><span data-stu-id="62bac-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="62bac-111">Kliknite dvaput na poruku koju želite da opozovete da biste je otvorili.</span><span class="sxs-lookup"><span data-stu-id="62bac-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="62bac-112">Izaberite karticu **poruka** , a zatim izaberite **stavke Radnje**  >  **Opozovi ovu poruku**.</span><span class="sxs-lookup"><span data-stu-id="62bac-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="62bac-113">Izaberite stavku **Izbriši nepročitane kopije ove poruke** ili **Izbriši nepročitane kopije i zameni je novom porukom**, a zatim kliknite na **dugme u redu**.</span><span class="sxs-lookup"><span data-stu-id="62bac-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="62bac-114">Ako šaljete poruku za zamenu, sastavite poruku, a zatim izaberite stavku **Pošalji**.</span><span class="sxs-lookup"><span data-stu-id="62bac-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="62bac-115">Uspeh ili otkazivanje opoziva poruke zavisi od postavki primaoca u programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="62bac-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="62bac-116">Da biste proverili opoziv, pogledajte [Ovaj članak](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="62bac-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="62bac-117">Pretraga i brisanje e-poruka u organizaciji</span><span class="sxs-lookup"><span data-stu-id="62bac-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="62bac-118">Ako niste globalni administrator, nalog mora da se doda ulozi upravljača e-otkrivanja ili usaglašenosti u upravljanju potraživanju za pretraživanje poruka.</span><span class="sxs-lookup"><span data-stu-id="62bac-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="62bac-119">Da biste izbrisali poruke, moraćete da se pridružite grupi uloga za upravljanje organizacijom ili svojoj ulozi za pretraživanje i čišćenje.</span><span class="sxs-lookup"><span data-stu-id="62bac-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="62bac-120">Dozvole za ove uloge se dodeljuju u [centru za bezbednost i usaglašenost](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="62bac-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="62bac-121">[Kreirajte pretragu sadržaja](https://docs.microsoft.com/microsoft-365/compliance/content-search) da biste pronašli poruku za brisanje.</span><span class="sxs-lookup"><span data-stu-id="62bac-121">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="62bac-122">[Povezivanje sa PowerShell centra za bezbednost i usaglašenost](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="62bac-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="62bac-123">Ako koristite višestruku potvrdu identiteta, pogledajte članak [Povezivanje sa sistemom Microsoft 365 Security i Center za usaglašenost pomoću multifaktor potvrde identiteta](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="62bac-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>