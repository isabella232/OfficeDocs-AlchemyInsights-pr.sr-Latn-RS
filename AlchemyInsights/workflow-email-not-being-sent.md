---
title: E-pošta toka posla se ne šalje
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749003"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="60c59-102">E-pošta toka posla se ne šalje za SharePoint listu ili biblioteku</span><span class="sxs-lookup"><span data-stu-id="60c59-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="60c59-103">E-pošta iz tokova posla se ne šalju svim korisnicima ili samo određenim korisnicima ili vidite grešku **koju e-poruka nije moguće poslati. Proverite da li e-pošta ima važeće primaoca**.</span><span class="sxs-lookup"><span data-stu-id="60c59-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="60c59-104">Potvrdite izbor u polju za proveru da li korisnik postoji u grupi dozvole za **sve osobe** (Lista korisničkih informacija) za tu kolekciju lokacija.</span><span class="sxs-lookup"><span data-stu-id="60c59-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="60c59-105">Uzorak direktnog URL adrese: https:// <tenant> . SharePoint.com/sites/ <sitename> /_layouts/15/ljudi Le.aspx? Članstvo "Grupito = 0</span><span class="sxs-lookup"><span data-stu-id="60c59-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="60c59-106">Ako korisnik ne postoji, uverite se da je korisnik prijavljen na stranicu.</span><span class="sxs-lookup"><span data-stu-id="60c59-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="60c59-107">Ako je to spoljni korisnik, proverite da li je poziv prihvaжen.</span><span class="sxs-lookup"><span data-stu-id="60c59-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="60c59-108">Ako korisnik postoji u grupi dozvole, uverite se da je e-adresa tačna.</span><span class="sxs-lookup"><span data-stu-id="60c59-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="60c59-109">Ako adresa e-pošte korisnika nije postavljena ovde, kreirajte uzorak obaveštenja za tog korisnika koji obavezuje sinhronizaciju tog korisničkog naloga iz korisničkih profila sistema SharePoint u ovu kolekciju lokacija.</span><span class="sxs-lookup"><span data-stu-id="60c59-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="60c59-110">E-pošta iz tokova posla se šalje administratorima kolekcije lokacija, ali ne drugim korisnicima i pogledajte grešku **http zabranjenom na <span>https:</span>2016 url/_vti_bin/Client.XVC.SP.Utilities.Utility.sendemail**.</span><span class="sxs-lookup"><span data-stu-id="60c59-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="60c59-111">[Pristup nije dozvoljen prilikom slanja e-poruke SharePoint grupi](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="60c59-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="60c59-112">Pored toga, proverite da li funkcija za ograničenje kolekcije lokacija **ograničene pristupa korisniku** nije aktivna.</span><span class="sxs-lookup"><span data-stu-id="60c59-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="60c59-113">Сродне теме</span><span class="sxs-lookup"><span data-stu-id="60c59-113">Related topics</span></span>
<span data-ttu-id="60c59-114">Želite da probate Microsoft flow u usluzi SharePoint online?</span><span class="sxs-lookup"><span data-stu-id="60c59-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="60c59-115">Kreiranje protoka</span><span class="sxs-lookup"><span data-stu-id="60c59-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="60c59-116">SharePoint i protok</span><span class="sxs-lookup"><span data-stu-id="60c59-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


