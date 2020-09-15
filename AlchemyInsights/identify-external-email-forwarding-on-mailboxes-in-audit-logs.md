---
title: Identifikovanje spoljnog prosleđivanja e-pošte na Poštanske sandučiće u evidenciji nadzora
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
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696311"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="193c4-102">Identifikujte kada je spoljni Prosleđivanje e-pošte konfigurisan na poštanskim sandučićima</span><span class="sxs-lookup"><span data-stu-id="193c4-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="193c4-103">Kada Microsoft 365 korisnik konfiguriše spoljnu Prosleđivanje e-pošte u **poštansko sanduče,** aktivnost se nadgleda kao deo cmdlet adrese.</span><span class="sxs-lookup"><span data-stu-id="193c4-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="193c4-104">Možete da vidite aktivnost pomoću pretrage evidencije nadzora u centru za bezbednost & bezbednosti.</span><span class="sxs-lookup"><span data-stu-id="193c4-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="193c4-105">Prijavite se u [Microsoft 365 Security & centar za usaglašenost](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="193c4-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="193c4-106">Idite na stranicu **Search**  >  **Pretraga evidencije nadgledanja** za pretraživanje.</span><span class="sxs-lookup"><span data-stu-id="193c4-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="193c4-107">Izaberite opseg datuma u poljima **početni** i **Krajnji datum** .</span><span class="sxs-lookup"><span data-stu-id="193c4-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="193c4-108">Nije potrebno da navedete korisničko ime.</span><span class="sxs-lookup"><span data-stu-id="193c4-108">You don't need to specify a username.</span></span> <span data-ttu-id="193c4-109">Proverite da li je polje **aktivnosti** podešeno da **prikazuje rezultate za sve aktivnosti**.</span><span class="sxs-lookup"><span data-stu-id="193c4-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="193c4-110">Kliknite na dugme **Pretraži**.</span><span class="sxs-lookup"><span data-stu-id="193c4-110">Click **Search**.</span></span>

<span data-ttu-id="193c4-111">U rezultatima izaberite stavku **Filtriraj rezultate** i otkucajte **podešeno-poštansko sanduče** u polju Filter aktivnosti.</span><span class="sxs-lookup"><span data-stu-id="193c4-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="193c4-112">Izaberite zapis nadzora u rezultatima.</span><span class="sxs-lookup"><span data-stu-id="193c4-112">Select an audit record in the results.</span></span> <span data-ttu-id="193c4-113">U okviru **Detalji** , kliknite na dugme **više informacija**.</span><span class="sxs-lookup"><span data-stu-id="193c4-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="193c4-114">Morate da pogledate detalje o svakom zapisu nadzora da biste utvrdili da li je aktivnost povezana sa prosleđivanjem e-pošte.</span><span class="sxs-lookup"><span data-stu-id="193c4-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="193c4-115">**ObjectId**: vrednost pseudonima koja je izmenjena u poštanskom sandučetu.</span><span class="sxs-lookup"><span data-stu-id="193c4-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="193c4-116">**Parametri**: _forwardingsmtpadress_ pokazuje ciljnu e-adresu.</span><span class="sxs-lookup"><span data-stu-id="193c4-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="193c4-117">**Korisnički ID**: korisnik koji konfiguriše Prosleđivanje e-pošte na poštansko sanduče u polju **ObjectId** .</span><span class="sxs-lookup"><span data-stu-id="193c4-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="193c4-118">Više informacija potražite u članku [Utvrđivanje ko je podesio Prosleđivanje e-pošte za poštansko sanduče](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="193c4-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span></span>
