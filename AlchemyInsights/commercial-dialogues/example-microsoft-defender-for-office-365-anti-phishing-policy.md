---
title: Primer Microsoft Defender za Office 365 anti-phishing smernice
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
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750795"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a><span data-ttu-id="5881a-102">Primer Microsoft Defender za Office 365 anti-phishing smernice</span><span class="sxs-lookup"><span data-stu-id="5881a-102">Example Microsoft Defender for Office 365 anti-phishing policy</span></span>

<span data-ttu-id="5881a-103">Ove postavke omogućavaju smernice zvano *domen i izvršni direktor*.</span><span class="sxs-lookup"><span data-stu-id="5881a-103">These settings enable a policy called *Domain and CEO*.</span></span> <span data-ttu-id="5881a-104">Ova smernica omogućava i zaštitu korisnika i domena od imitacije, a zatim primenjuju smernice na sve e-poruke koje primaju korisnici unutar domena.</span><span class="sxs-lookup"><span data-stu-id="5881a-104">This policy provides both user and domain protection from impersonation and then applies the policy to all email received by users within the domain.</span></span> <span data-ttu-id="5881a-105">Prvo dodajte sledeće informacije da biste kreirali smernice:</span><span class="sxs-lookup"><span data-stu-id="5881a-105">First, add the following information to create the policy:</span></span>

- <span data-ttu-id="5881a-106">**Ime**: **Opis** domena i generalnog direktora: obezbeđuje da se izvršni direktor i vaš domen ne imitiraju.</span><span class="sxs-lookup"><span data-stu-id="5881a-106">**Name**: Domain and CEO **Description**: Ensures that the CEO and your domain are not being impersonated.</span></span>
  <span data-ttu-id="5881a-107">**Primeni na**: izaberite **domen primaoca**.</span><span class="sxs-lookup"><span data-stu-id="5881a-107">**Applied to**: Select **The recipient domain is**.</span></span> <span data-ttu-id="5881a-108">U okviru **bilo koje od ovih** **stavki izaberite stavku Izaberi**, a zatim izaberite domen.</span><span class="sxs-lookup"><span data-stu-id="5881a-108">Under **Any of these**, select **Choose**, and then select a domain.</span></span> <span data-ttu-id="5881a-109">Izaberite stavku **+ Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="5881a-109">Select **+ Add**.</span></span> <span data-ttu-id="5881a-110">Potvrdite izbor u polju za potvrdu pored imena domena na listi (na primer, *contoso.com*), a zatim izaberite stavku **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="5881a-110">Select the check box next to the name of the domain in the list (for example, *contoso.com*), and then select **Add**.</span></span> <span data-ttu-id="5881a-111">Izaberite stavku **gotovo**.</span><span class="sxs-lookup"><span data-stu-id="5881a-111">Select **Done**.</span></span>
- <span data-ttu-id="5881a-112">Kada se smernice kreiraju, možete precizno da kreirate smernice pomoću sledećih opcija:</span><span class="sxs-lookup"><span data-stu-id="5881a-112">After the policy is created, you can fine-tune the policy by using the following options:</span></span>
  - <span data-ttu-id="5881a-113">**Dodavanje korisnika u zaštitu:** U ovom primeru, dodajte adresu e-pošte izvršnog direktora.</span><span class="sxs-lookup"><span data-stu-id="5881a-113">**Add users to protect:** For this example, add the CEO's email address, at a minimum.</span></span>
  - <span data-ttu-id="5881a-114">**Dodajte domeni da biste zaštitili**: dodajte organizacioni domen koji uključuje Office generalnog direktora.</span><span class="sxs-lookup"><span data-stu-id="5881a-114">**Add domains to protect**: Add the organizational domain that includes the office of the CEO.</span></span>
  - <span data-ttu-id="5881a-115">**Odaberite stavke Radnje**: **Ako je imitator poslao e-poštu**, izaberite **poruku preusmeravanja na drugu e-adresu**, a zatim unesite e-adresu administratora bezbednosti (na primer, *securityadmin@contoso.com*).</span><span class="sxs-lookup"><span data-stu-id="5881a-115">**Choose actions**: For **If email is sent by an impersonated user**, select **Redirect message to another email address**, and then enter the email address of the security administrator (for example, *securityadmin@contoso.com*).</span></span> <span data-ttu-id="5881a-116">**Ako će e-pošta biti poslata pomoću imitiranog domena**, izaberite stavku **karantin**.</span><span class="sxs-lookup"><span data-stu-id="5881a-116">For **If email is sent by an impersonated domain**, select **Quarantine the message**.</span></span>
  - <span data-ttu-id="5881a-117">**Obaveštajna služba za poštansko sanduče**: Ova opcija je podrazumevano izabrana kada kreirate novu anti-phishing smernice.</span><span class="sxs-lookup"><span data-stu-id="5881a-117">**Mailbox intelligence**: By default, this option is selected when you create a new anti-phishing policy.</span></span> <span data-ttu-id="5881a-118">Ostavite **ovo podešavanje za** najbolje rezultate.</span><span class="sxs-lookup"><span data-stu-id="5881a-118">Leave this setting **On** for best results.</span></span>
  - <span data-ttu-id="5881a-119">**Dodajte Pouzdane pošiljaoce i** domeni: Za ovaj primer, nemojte definisati zamene.</span><span class="sxs-lookup"><span data-stu-id="5881a-119">**Add trusted senders and domains:** For this example, don't define any overrides.</span></span>
- <span data-ttu-id="5881a-120">Kada pregledate postavke, izaberite stavku **Kreiraj ove smernice** ili **Sačuvaj** na odgovarajući način.</span><span class="sxs-lookup"><span data-stu-id="5881a-120">Once you've reviewed your settings, select **Create this policy** or **Save**, as appropriate.</span></span>

<span data-ttu-id="5881a-121">Da biste saznali više, pogledajte članak [anti-phishing smernice u programu Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span><span class="sxs-lookup"><span data-stu-id="5881a-121">To learn more, see [Anti-phishing policies in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span></span>
