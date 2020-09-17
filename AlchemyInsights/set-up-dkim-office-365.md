---
title: Podešavanje DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808721"
---
# <a name="setup-dkim"></a><span data-ttu-id="31b08-102">Podešavanje DKIM</span><span class="sxs-lookup"><span data-stu-id="31b08-102">Setup DKIM</span></span>

<span data-ttu-id="31b08-103">Kompletna uputstva za konfigurisanje DKIM za prilagođene [domene](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)u programu Microsoft 365 su ovde.</span><span class="sxs-lookup"><span data-stu-id="31b08-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

1. <span data-ttu-id="31b08-104">Za **svaki** prilagođeni domen treba da kreirate **dva** dkim CNAME zapisa u usluzi DNS hostinga domena (obično je to registar domena).</span><span class="sxs-lookup"><span data-stu-id="31b08-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="31b08-105">Na primer, contoso.com i fourthcoffee.com zahtevaju četiri DKIM CNAME zapisa: dva za contoso.com i dva za fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="31b08-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="31b08-106">DKIM CNAME zapisi za **svaki** prilagođeni domen koriste sledeće formate:</span><span class="sxs-lookup"><span data-stu-id="31b08-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="31b08-107">**Ime hosta**: `selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="31b08-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="31b08-108">**Upućuje na adresu ili vrednost**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="31b08-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="31b08-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="31b08-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="31b08-110">**Ime hosta**: `selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="31b08-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="31b08-111">**Upućuje na adresu ili vrednost**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="31b08-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="31b08-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="31b08-112">**TTL**: 3600</span></span>

   <span data-ttu-id="31b08-113">\<DomainGUID\> je tekst sa leve strane `.mail.protection.outlook.com` u prilagođenom MX zapisu za prilagođeni domen (na primer, `contoso-com` za domen contoso.com).</span><span class="sxs-lookup"><span data-stu-id="31b08-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="31b08-114">\<InitialDomain\> je domen koji ste koristili kada ste se prijavili za Microsoft 365 (na primer, contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="31b08-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="31b08-115">Kada kreirate CNAME zapise za prilagođene domene, dovršite sledeća uputstva:</span><span class="sxs-lookup"><span data-stu-id="31b08-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="31b08-116">Neko.</span><span class="sxs-lookup"><span data-stu-id="31b08-116">a.</span></span> <span data-ttu-id="31b08-117">[Prijavite se u Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) pomoću poslovnog ili školskog naloga.</span><span class="sxs-lookup"><span data-stu-id="31b08-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="31b08-118">-.</span><span class="sxs-lookup"><span data-stu-id="31b08-118">b.</span></span> <span data-ttu-id="31b08-119">Izaberite ikonu za pokretanje aplikacija u gornjem levom uglu i odaberite stavku **administrator**.</span><span class="sxs-lookup"><span data-stu-id="31b08-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="31b08-120">trojku.</span><span class="sxs-lookup"><span data-stu-id="31b08-120">c.</span></span> <span data-ttu-id="31b08-121">U donjem levom oknu za navigaciju, razvijte stavku **administrator** i odaberite stavku **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="31b08-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="31b08-122">-.</span><span class="sxs-lookup"><span data-stu-id="31b08-122">d.</span></span> <span data-ttu-id="31b08-123">Idite na **bezbednost**  >  **dkim**.</span><span class="sxs-lookup"><span data-stu-id="31b08-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="31b08-124">elektron.</span><span class="sxs-lookup"><span data-stu-id="31b08-124">e.</span></span> <span data-ttu-id="31b08-125">Izaberite domen, a zatim odaberite stavku **Omogućavanje** za **potpisivanje poruka za ovaj domen pomoću dkim potpisa**.</span><span class="sxs-lookup"><span data-stu-id="31b08-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="31b08-126">Ponovite ovaj stepenik za svaki prilagođeni domen.</span><span class="sxs-lookup"><span data-stu-id="31b08-126">Repeat this step for each custom domain.</span></span>
