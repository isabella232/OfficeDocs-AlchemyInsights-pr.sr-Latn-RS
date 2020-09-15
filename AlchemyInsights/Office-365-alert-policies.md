---
title: 1385-Office-365-upozorenje-smernice
ms.author: markjjo
author: markjjo
manager: lauraw
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1385"
- "3200002"
ms.assetid: ''
ms.openlocfilehash: 8821a2ee1ae2207de5d1604762badf43808373c8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664040"
---
# <a name="alert-policies"></a><span data-ttu-id="29b97-102">Smernice za obaveštenja</span><span class="sxs-lookup"><span data-stu-id="29b97-102">Alert policies</span></span>

<span data-ttu-id="29b97-103">Microsoft 365 Security & centar za usaglašenost pruža [podrazumevane smernice za obaveštenje](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies) koje aktiviraju obaveštenja za organizacije sa Office 365 Enterprise ili Office 365 američka vlada E1/G1, E3/G3 ili E5/G5 pretplatu.</span><span class="sxs-lookup"><span data-stu-id="29b97-103">The Microsoft 365 security & Compliance Center offers [default alert policies](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies) that trigger alerts for organizations with an Office 365 Enterprise or Office 365 US Government E1/G1, E3/G3, or E5/G5 subscription.</span></span> <span data-ttu-id="29b97-104">Stoga, administratori mogu da prime obaveštenje o obaveštenju e-pošte koje šalje Office365Alerts@microsoft.com pomoću reda za temu kao što je "obaveštenje o niskom iznosu: *ime smernica upozorenja*".</span><span class="sxs-lookup"><span data-stu-id="29b97-104">Therefore, admins may receive an alert email notification sent by Office365Alerts@microsoft.com with a subject line such as "A low-severity alert: *name of alert policy*".</span></span> <span data-ttu-id="29b97-105">Obaveštenja se šalju prilikom aktiviranja obaveštenja za uobičajene aktivnosti, na primer kada korisnici:</span><span class="sxs-lookup"><span data-stu-id="29b97-105">Alert notifications are sent when alerts are triggered for common activities, such as when users:</span></span>

- <span data-ttu-id="29b97-106">Kreirajte pravila za prijemno poštansko sanduče koja prosleđuje e-poštu.</span><span class="sxs-lookup"><span data-stu-id="29b97-106">Create inbox rules that forward email.</span></span>
- <span data-ttu-id="29b97-107">Dodeljivanje dozvola svom poštanskom sandučetu.</span><span class="sxs-lookup"><span data-stu-id="29b97-107">Assign permissions their mailbox.</span></span>
- <span data-ttu-id="29b97-108">Delite ili izbrišite veliki broj datoteka u deljenju SharePoint datoteka.</span><span class="sxs-lookup"><span data-stu-id="29b97-108">Share or delete a large number of files in SharePoint file sharing.</span></span>
- <span data-ttu-id="29b97-109">Kreirajte eDiscovery pretrage i izvezite rezultate pretrage.</span><span class="sxs-lookup"><span data-stu-id="29b97-109">Create eDiscovery searches and export search results.</span></span>

<span data-ttu-id="29b97-110">Da biste pregledali i radili po obaveštenju:</span><span class="sxs-lookup"><span data-stu-id="29b97-110">To review and act on an alert:</span></span>

1. <span data-ttu-id="29b97-111">Idite na [bezbednosni & centar za usaglašenost](https://protection.office.com) i prijavite se.</span><span class="sxs-lookup"><span data-stu-id="29b97-111">Go to the [Security & Compliance center](https://protection.office.com) and sign in.</span></span>
2. <span data-ttu-id="29b97-112">Kliknite **na dugme upozori**  >  **Prikaz**upozorenja.</span><span class="sxs-lookup"><span data-stu-id="29b97-112">Click **Alerts** > **View alerts**.</span></span>
3. <span data-ttu-id="29b97-113">Kliknite na upozorenje da biste otvorili stranicu sa informacijama o obaveštenju.</span><span class="sxs-lookup"><span data-stu-id="29b97-113">Click an alert to display a flyout page with information about the alert.</span></span>

<span data-ttu-id="29b97-114">Možete da uradite nešto u vezi sa obaveštenjem, kao što [je uklanjanje sumnjivog prijemnog poštanskog sandučeta](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account).</span><span class="sxs-lookup"><span data-stu-id="29b97-114">You can take action on an alert, such as [removing a suspicious inbox rule](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account).</span></span> <span data-ttu-id="29b97-115">Možete jednostavno da zatvorite obaveštenje tako što ćete kliknuti na dugme **rešenje** na stranici obaveštenje.</span><span class="sxs-lookup"><span data-stu-id="29b97-115">Or you can simply close the alert by clicking **Resolve** on the alert flyout page.</span></span>

<span data-ttu-id="29b97-116">Više informacija o konfigurisanju i upravljanju smernicama obaveštenja potražite u  [članku ovaj članak](https://docs.microsoft.com/microsoft-365/compliance/alert-policies).</span><span class="sxs-lookup"><span data-stu-id="29b97-116">For more information about configuring and managing alert policies, see  [this article](https://docs.microsoft.com/microsoft-365/compliance/alert-policies).</span></span>

<span data-ttu-id="29b97-117">**Važno**: obaveštavanje obaveštenja e-poštom od korporacije Microsoft nikada vam neće zatražiti da uradite sledeće:</span><span class="sxs-lookup"><span data-stu-id="29b97-117">**Important**: Alert email notifications from Microsoft will never ask you to do the following:</span></span>

- <span data-ttu-id="29b97-118">Obezbeđivanje lozinke</span><span class="sxs-lookup"><span data-stu-id="29b97-118">Provide a password</span></span>
- <span data-ttu-id="29b97-119">Verifikacija bezbednosnih detalja naloga</span><span class="sxs-lookup"><span data-stu-id="29b97-119">Verify the security details of your account</span></span>
- <span data-ttu-id="29b97-120">Ponovo potvrdite sebe</span><span class="sxs-lookup"><span data-stu-id="29b97-120">Re-authenticate yourself</span></span>

<span data-ttu-id="29b97-121">Ako primite e-poruku kao što je ova, Microsoft nije poslao Microsoft i treba da se smatra phishing prevarom.</span><span class="sxs-lookup"><span data-stu-id="29b97-121">If you receive an email message like this, it was not sent by Microsoft and should be considered a phishing scam.</span></span> <span data-ttu-id="29b97-122">Ako se to desi, [Prijavite ga korporaciji Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop).</span><span class="sxs-lookup"><span data-stu-id="29b97-122">If that happens, please [report it to Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop).</span></span>