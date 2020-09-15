---
title: Rešavanje problema sa isporukom e-pošte u javne fascikle sa omogućenom poštom
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
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: da35ae4bd911fb75f23cc1c99aacbaa2392425dd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677942"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="620be-102">Rešavanje problema sa isporukom e-pošte u javne fascikle sa omogućenom poštom</span><span class="sxs-lookup"><span data-stu-id="620be-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="620be-103">Ako spoljni pošiljaoci ne mogu da šalju poruke u javne fascikle sa omogućenom poštom pošte, a pošiljaoci imaju grešku: **nije bilo moguće pronaći (550 5.4.1)**, proverite da li je domen e-pošte za javnu fasciklu konfigurisan kao unutrašnji domen relej umesto autoritativno domen:</span><span class="sxs-lookup"><span data-stu-id="620be-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="620be-104">Otvorite [Exchange centar administracije (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="620be-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="620be-105">Idite na **protok pošte** \> **prihvaćeni**domeni, izaberite prihvaćeni domen, a zatim kliknite na dugme **Uredi**.</span><span class="sxs-lookup"><span data-stu-id="620be-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="620be-106">Na stranici "Svojstva" koja se otvara, ako je tip domena podešen na **autoritativno**, promenite vrednost u **unutrašnji relej** , a zatim kliknite na dugme **Sačuvaj**.</span><span class="sxs-lookup"><span data-stu-id="620be-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="620be-107">Ako spoljni pošiljaoci dobiju grešku **nemate dozvolu (550 5.7.13)**, uradite sledeće komande u [Exchange online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) da biste videli dozvole za anonimne korisnike u javnoj fascikli:</span><span class="sxs-lookup"><span data-stu-id="620be-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="620be-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Na primer, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .</span><span class="sxs-lookup"><span data-stu-id="620be-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="620be-109">Da biste dopustili spoljnim korisnicima da šalju e-poštu u ovu javnu fasciklu, dodajte dugme Createstavke pravo na anonimni korisnik.</span><span class="sxs-lookup"><span data-stu-id="620be-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="620be-110">Na primer, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .</span><span class="sxs-lookup"><span data-stu-id="620be-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
