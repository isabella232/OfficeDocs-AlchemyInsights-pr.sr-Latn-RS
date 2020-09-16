---
title: Korišćenje wix Veb lokacije sa Microsoft kupljenim ili upravljanim domenima
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5855"
- "9003096"
ms.openlocfilehash: bef0943c8621043218088abf0deebddf6c19ef50
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664760"
---
# <a name="using-a-wix-website-with-microsoft-purchased-or-managed-domains"></a><span data-ttu-id="d13cf-102">Korišćenje wix Veb lokacije sa Microsoft kupljenim ili upravljanim domenima</span><span class="sxs-lookup"><span data-stu-id="d13cf-102">Using a Wix website with Microsoft purchased or managed domains</span></span>

<span data-ttu-id="d13cf-103">Informacije o tome kako da koristite wix Veb lokaciju pomoću Microsoft kupljenog ili kontrolisanog domena potražite [u članku ažuriranje DNS zapisa radi zadržavanja Veb lokacije kod trenutnog dobavljača usluga hostinga](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider).</span><span class="sxs-lookup"><span data-stu-id="d13cf-103">For information about how to use a Wix website with a Microsoft purchased or managed domain, see [Update DNS records to keep your website with your current hosting provider](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider).</span></span>

<span data-ttu-id="d13cf-104">Detalje potražite u članku:</span><span class="sxs-lookup"><span data-stu-id="d13cf-104">For details, see:</span></span> 

- <span data-ttu-id="d13cf-105">Vix članak, "povezivanje domena sa Viksom pomoću metoda pokazivača", preporučuje se Dodavanje DNS zapisa kao što je navedeno u članku iznad, a ne za menjanje servera imena kada koristite Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d13cf-105">The Wix article, "Connecting a Domain to Wix Using the Pointing Method," recommends adding DNS records as outlined in the link above rather than changing names servers when you're using Microsoft 365.</span></span>

- <span data-ttu-id="d13cf-106">Ako odaberete da promenite servere imena u Vix, morate da kreirate DNS zapise u programu wix za Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d13cf-106">If you choose to change name servers to Wix, you must create DNS records at Wix for Microsoft.</span></span> <span data-ttu-id="d13cf-107">Više informacija potražite u članku [Kreiranje DNS zapisa na lokaciji wix za Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix).</span><span class="sxs-lookup"><span data-stu-id="d13cf-107">For more info, see [Create DNS records at Wix for Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix).</span></span>

- <span data-ttu-id="d13cf-108">Ako je vaš domen kupljen od korporacije Microsoft, ne možete da promenite servere imena.</span><span class="sxs-lookup"><span data-stu-id="d13cf-108">If your domain was purchased from Microsoft the name servers can't be changed.</span></span> <span data-ttu-id="d13cf-109">Ako morate da promenite servere imena, Microsoft kupljeni domen mora biti prebačen na drugi dobavljač usluga posle 60 dana.</span><span class="sxs-lookup"><span data-stu-id="d13cf-109">If you must change names servers, the Microsoft purchased domain must be transferred to another hosting provider after 60 days.</span></span> <span data-ttu-id="d13cf-110">Više informacija potražite u članku [prenošenje domena sa korporacije Microsoft na drugi host](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host).</span><span class="sxs-lookup"><span data-stu-id="d13cf-110">For more info, see [Transfer a domain from Microsoft to another host](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host).</span></span>
