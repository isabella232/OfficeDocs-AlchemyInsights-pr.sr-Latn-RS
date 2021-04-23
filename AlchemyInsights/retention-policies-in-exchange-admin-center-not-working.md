---
title: Smernice za zadržavanje u Exchange centru aktivnosti ne rade
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
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952242"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="1b118-102">Smernice za zadržavanje u Exchange centru administrovanja</span><span class="sxs-lookup"><span data-stu-id="1b118-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="1b118-103">Ako želite da pokrenemo automatske provere postavki koje su pomenute ispod, kliknite na dugme "nazad< – na vrhu ove stranice, a zatim unesite adresu e-pošte korisnika koji ima problema sa smernicama za zadržavanje.</span><span class="sxs-lookup"><span data-stu-id="1b118-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

<span data-ttu-id="1b118-104">Ako imate problema sa smernicama za zadržavanje u Exchange centru adminimenata koje se ne primenjuju na poštanske sandučiće ili stavke koje se ne premeštaju u arhivski poštansko sanduče, proverite sledeće:</span><span class="sxs-lookup"><span data-stu-id="1b118-104">If you have problems with retention policies in the Exchange Admin Center not applying to mailboxes or items not moving to the archive mailbox, check the following:</span></span>

<span data-ttu-id="1b118-105">**Osnovni uzroci:**</span><span class="sxs-lookup"><span data-stu-id="1b118-105">**Root Causes:**</span></span>

- <span data-ttu-id="1b118-106">**Pomoćnik za kontrolisane** fascikle nije obradio poštansko sanduče korisnika.</span><span class="sxs-lookup"><span data-stu-id="1b118-106">**Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="1b118-107">Pomoćnik za kontrolisane fascikle pokušava da obradi svako poštansko sanduče u organizaciji zasnovanoj na oblaku na svakih sedam dana.</span><span class="sxs-lookup"><span data-stu-id="1b118-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span>

  <span data-ttu-id="1b118-108">**Rešenje:** Pokrenite pomoćnik za kontrolisane fascikle.</span><span class="sxs-lookup"><span data-stu-id="1b118-108">**Solution:** Run the Managed Folder Assistant.</span></span>

- <span data-ttu-id="1b118-109">**ZadržavanjeHold je** **omogućeno u** poštanskom sandučetu.</span><span class="sxs-lookup"><span data-stu-id="1b118-109">**RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="1b118-110">Ako je poštansko sanduče postavljeno na zadržavanje, smernice za zadržavanje poštanskog sandučeta neće biti obrađene tokom tog vremena.</span><span class="sxs-lookup"><span data-stu-id="1b118-110">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span>

  <span data-ttu-id="1b118-111">**Rešenje:** Proverite status postavke zadržavanja i ažurirajte po potrebi.</span><span class="sxs-lookup"><span data-stu-id="1b118-111">**Solution:** Check status of Retention Hold setting and update as needed.</span></span> <span data-ttu-id="1b118-112">Detalje možete da vidite u [temi Zadržavanje poštanskog sandučeta.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)</span><span class="sxs-lookup"><span data-stu-id="1b118-112">For details, see [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
 
<span data-ttu-id="1b118-113">**Napomogućeno:** Ako je poštansko sanduče manje od 10 MB, pomoćnik za kontrolisane fascikle neće automatski obraditi poštansko sanduče.</span><span class="sxs-lookup"><span data-stu-id="1b118-113">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="1b118-114">Više informacija o smernicama za zadržavanje u Exchange centru admin center potražite u članku:</span><span class="sxs-lookup"><span data-stu-id="1b118-114">For more info on retention policies in the Exchange Admin Center, see:</span></span>

- [<span data-ttu-id="1b118-115">Oznake za zadržavanje i smernice za zadržavanje</span><span class="sxs-lookup"><span data-stu-id="1b118-115">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- <span data-ttu-id="1b118-116">[Primena smernica za zadržavanje na poštanske](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) sandučiće ili [Dodavanje ili uklanjanje oznaka zadržavanja](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span><span class="sxs-lookup"><span data-stu-id="1b118-116">[Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) or [Add or remove retention tags](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span></span>

- [<span data-ttu-id="1b118-117">Kako da identifikujete tip zadrške postavljene u poštansko sanduče</span><span class="sxs-lookup"><span data-stu-id="1b118-117">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
