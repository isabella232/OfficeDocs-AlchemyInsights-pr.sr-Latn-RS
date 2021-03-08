---
title: Automatsko premeštanje e-poruka u poštansko sanduče arhive
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
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527101"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a><span data-ttu-id="449d3-102">Automatsko premeštanje e-poruka u poštansko sanduče arhive</span><span class="sxs-lookup"><span data-stu-id="449d3-102">Automatically move email messages to the archive mailbox</span></span>

<span data-ttu-id="449d3-103">Evo kako da podesite smernice za automatsko premeštanje stare korisnikove e-poruke u poštansko sanduče arhive:</span><span class="sxs-lookup"><span data-stu-id="449d3-103">Here's how to set up a policy to automatically move a user's old email to the archive mailbox:</span></span>

1. <span data-ttu-id="449d3-104">Idite na [**Bezbednosno &**](https://go.microsoft.com/fwlink/p/?linkid=2077143)  >    >  **arhiv** za upravljanje podacima da biste potvrdili da je poštansko sanduče omogućeno za korisnika.</span><span class="sxs-lookup"><span data-stu-id="449d3-104">Go to [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143) > **Data governance** > **Archive** to verify an archive mailbox has been enabled for the user.</span></span> <span data-ttu-id="449d3-105">Ako nije, kliknite na dugme **Omogućavanje** zatim **da** u polju upozorenje.</span><span class="sxs-lookup"><span data-stu-id="449d3-105">If it hasn't, click **Enable** then **Yes** in the warning box.</span></span>
2. <span data-ttu-id="449d3-106">Idite na [**Exchange centar administracije > > oznake za zadržavanje**](https://go.microsoft.com/fwlink/?linkid=2059104).</span><span class="sxs-lookup"><span data-stu-id="449d3-106">Go to [**Exchange admin center > compliance management > retention tags**](https://go.microsoft.com/fwlink/?linkid=2059104).</span></span>
3. <span data-ttu-id="449d3-107">Kliknite na ikonu + da biste se **automatski prijavili na celokupno poštansko sanduče**.</span><span class="sxs-lookup"><span data-stu-id="449d3-107">Choose the + icon then choose **automatically apply to entire mailbox**.</span></span>
4. <span data-ttu-id="449d3-108">Dodelite ime oznake za zadržavanje i odaberite stavku **Premesti u arhivu**.</span><span class="sxs-lookup"><span data-stu-id="449d3-108">Assign a name to the retention tag, and choose **Move to Archive**.</span></span> <span data-ttu-id="449d3-109">Za period zadržavanja unesite vreme koje želite, na primer 90 dana.</span><span class="sxs-lookup"><span data-stu-id="449d3-109">For the retention period, enter the time you want, such as 90 days.</span></span> <span data-ttu-id="449d3-110">Kliknite na dugme **Sačuvaj**.</span><span class="sxs-lookup"><span data-stu-id="449d3-110">Click **Save**.</span></span>
5. <span data-ttu-id="449d3-111">Sada Kreirajte smernice za zadržavanje: odaberite **smernice za zadržavanje**, odaberite ikonu da biste dodali novu smernicu.</span><span class="sxs-lookup"><span data-stu-id="449d3-111">Now create a retention policy: choose **retention policies**, choose the icon to add a new policy.</span></span>
6. <span data-ttu-id="449d3-112">Dodelite ime smernicama za zadržavanje, a zatim kliknite i pomerajte se da biste pronašli i dodali oznaku za zadržavanje koju ste upravo kreirali.</span><span class="sxs-lookup"><span data-stu-id="449d3-112">Assign a name to the retention policy, then click and scroll to find and add the retention tag you just created.</span></span> <span data-ttu-id="449d3-113">Kliknite na dugme **Sačuvaj**.</span><span class="sxs-lookup"><span data-stu-id="449d3-113">Click **Save**.</span></span>
7. <span data-ttu-id="449d3-114">Konačno, primene smernica za zadržavanje na poštansko sanduče korisnika: još uvek se nalazi u Exchange centru administracije, idite na  >  **Poštanske sandučiće** primalaca.</span><span class="sxs-lookup"><span data-stu-id="449d3-114">Finally, apply the retention policy to the user's mailbox: still in the Exchange admin center, go to **recipients** > **mailboxes**.</span></span> <span data-ttu-id="449d3-115">Odaberite sve korisnike na koje želite da primene smernice, a zatim odaberite stavku **Uredi** (ikona olovke).</span><span class="sxs-lookup"><span data-stu-id="449d3-115">Choose all the users who you want to apply the policy to, then choose **Edit** (the pencil icon).</span></span>
8. <span data-ttu-id="449d3-116">U dijalogu izaberite stavku **funkcije poštanskog sandučeta**.</span><span class="sxs-lookup"><span data-stu-id="449d3-116">In the dialog box, click **mailbox features**.</span></span> <span data-ttu-id="449d3-117">U okviru **smernice za zadržavanje**, primenjujte smernice koje ste upravo kreirali > **Čuvanje**.</span><span class="sxs-lookup"><span data-stu-id="449d3-117">Under **Retention policy**, apply the policy you just created > **Save**.</span></span>
9. <span data-ttu-id="449d3-118">Uputstva za primenu smernica na svim korisnicima potražite u članku [Primena smernica za zadržavanje na Poštanske sandučiće](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span><span class="sxs-lookup"><span data-stu-id="449d3-118">For instructions for applying the policy to all users, see [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span></span>
