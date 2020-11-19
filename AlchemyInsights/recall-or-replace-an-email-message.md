---
title: Opoziv ili zamena e-poruke
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353520"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a><span data-ttu-id="ecd25-102">Opoziv ili zamena e-poruke u usluzi Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="ecd25-102">Recall or replace an email message in Microsoft 365</span></span>

- <span data-ttu-id="ecd25-103">Možete da **opozovete poruke koje se šalju osobama u vašoj organizaciji**.</span><span class="sxs-lookup"><span data-stu-id="ecd25-103">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="ecd25-104">Na primer, ako je poruka poslata na gmail adresu, ne možete da je opozovete.</span><span class="sxs-lookup"><span data-stu-id="ecd25-104">For example, if the message was sent to a Gmail address, you can't recall it.</span></span>
- <span data-ttu-id="ecd25-105">Možete **samo da opozovete poruke poslate iz programa Outlook za PC**.</span><span class="sxs-lookup"><span data-stu-id="ecd25-105">You can **only recall messages sent from Outlook for the PC**.</span></span> <span data-ttu-id="ecd25-106">Ako korisnik pošalje poruku pomoću programa Outlook za Mac ili Outlook na vebu, ne možete da ga opozovete.</span><span class="sxs-lookup"><span data-stu-id="ecd25-106">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>
- <span data-ttu-id="ecd25-107">Kao administrator zakupca, možete da **opozovete poruke u ime korisnika pomoću programa PowerShell** (više informacija potražite u članku: [pretraživanje i brisanje e-poruka](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span><span class="sxs-lookup"><span data-stu-id="ecd25-107">As a tenant administrator, you can **recall messages on behalf of users by using PowerShell** (For more information, see: [Search for and delete email messages](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span></span>
- <span data-ttu-id="ecd25-108">Ne možete da opozovete poruke iz centra administracije.</span><span class="sxs-lookup"><span data-stu-id="ecd25-108">You can't recall messages from the admin center.</span></span> <span data-ttu-id="ecd25-109">Pomerajte se nadole do stavke "Pretraga i brisanje e-poruka u organizaciji" za više informacija.</span><span class="sxs-lookup"><span data-stu-id="ecd25-109">Scroll down to "Search for and delete email messages in your organization" for more information.</span></span>

<span data-ttu-id="ecd25-110">**Opoziv ili zamena e-poruke koju ste poslali**</span><span class="sxs-lookup"><span data-stu-id="ecd25-110">**Recall or replace an email message that you sent**</span></span>

1. <span data-ttu-id="ecd25-111">U oknu sa fasciklama na levoj strani prozora programa Outlook Odaberite fasciklu poslate stavke.</span><span class="sxs-lookup"><span data-stu-id="ecd25-111">In the folder pane on the left of the Outlook window, choose the Sent Items folder.</span></span>
2. <span data-ttu-id="ecd25-112">Otvorite poruku koju želite da opozovete.</span><span class="sxs-lookup"><span data-stu-id="ecd25-112">Open the message that you want to recall.</span></span> <span data-ttu-id="ecd25-113">Morate da kliknete dvaput da biste otvorili poruku.</span><span class="sxs-lookup"><span data-stu-id="ecd25-113">You must double-click to open the message.</span></span> <span data-ttu-id="ecd25-114">Izbor poruke tako da se pojavljuje u oknu za čitanje neće vam omogućiti da opozovete poruku.</span><span class="sxs-lookup"><span data-stu-id="ecd25-114">Selecting the message so it appears in the reading pane won't allow you to recall the message.</span></span>
3. <span data-ttu-id="ecd25-115">Na kartici poruka izaberite **stavke Radnje**  >  **Opozovi ovu poruku**.</span><span class="sxs-lookup"><span data-stu-id="ecd25-115">From the Message tab, select **Actions** > **Recall This Message**.</span></span>
4. <span data-ttu-id="ecd25-116">Odaberite stavku **Izbriši nepročitane kopije ove poruke** ili **Izbriši nepročitane kopije i zameni je novom porukom**, a zatim kliknite na **dugme u redu**.</span><span class="sxs-lookup"><span data-stu-id="ecd25-116">Choose **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, then select **OK**.</span></span>
5. <span data-ttu-id="ecd25-117">Ako šaljete poruku za zamenu, sastavite poruku, a zatim izaberite **Pošalji**.</span><span class="sxs-lookup"><span data-stu-id="ecd25-117">If you're sending a replacement message, compose the message, then select **Send**.</span></span>
6. <span data-ttu-id="ecd25-118">Uspeh ili otkazivanje opoziva poruke zavisi od postavki primalaca u programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="ecd25-118">The success or failure of a message recall depends on the recipients' settings in Outlook.</span></span>

<span data-ttu-id="ecd25-119">Više informacija o tome kako da potvrdite opoziv potražite u članku [opoziv ili zamena e-poruke koju ste poslali](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="ecd25-119">For more information, including how to check on the recall, see [Recall or replace an email message that you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="ecd25-120">**_Da biste pretražili i izbrisali e-poruke u organizaciji_**, to je najlakše ako ste globalni administrator. Ako niste globalni administrator, nalog mora da se doda u grupu uloga menadžera eDiscovery ili na ulogu upravljanja usaglašenosti.</span><span class="sxs-lookup"><span data-stu-id="ecd25-120">**_To search for and delete email messages in your organization_**, it's easiest if you're a global admin. If you're not a global admin, your account must be added to the eDiscovery Manager role group, or to the Compliance Search management role.</span></span> <span data-ttu-id="ecd25-121">Da biste izbrisali poruke, moraćete da se pridružite grupi uloga za upravljanje organizacijom ili svojoj ulozi za pretraživanje i čišćenje.</span><span class="sxs-lookup"><span data-stu-id="ecd25-121">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="ecd25-122">Dozvole za ove uloge se dodeljuju u [centru za bezbednost & bezbednosti](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="ecd25-122">Permissions to these roles are assigned in the [Security & compliance center](https://protection.office.com/).</span></span>

1. <span data-ttu-id="ecd25-123">[Kreirajte pretragu sadržaja](https://docs.microsoft.com/microsoft-365/compliance/content-search) da biste pronašli poruku za brisanje.</span><span class="sxs-lookup"><span data-stu-id="ecd25-123">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
2. <span data-ttu-id="ecd25-124">[Povezivanje sa bezbednosnim & PowerShell Center usaglašenosti](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="ecd25-124">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span>

<span data-ttu-id="ecd25-125">Ako koristite MFA (multifaktor verifikacije identiteta), pogledajte članak [Povezivanje sa uslugom Microsoft 365 Security & centar za usaglašenost sa PowerShell pomoću multifaktor potvrde identiteta](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="ecd25-125">If you're using MFA (multi-factor authentication), see [Connect to Microsoft 365 Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span></span>
