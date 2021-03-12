---
title: Rešavanje uobičajenih problema sa oblikovanjem DKIM zapisa
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750758"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a><span data-ttu-id="1a5f3-102">Rešavanje uobičajenih problema sa oblikovanjem DKIM zapisa</span><span class="sxs-lookup"><span data-stu-id="1a5f3-102">Fix common problems with DKIM record formatting</span></span>

<span data-ttu-id="1a5f3-103">Većina DKIM podešavanje problema je povezana sa netačnim DNS zapisima.</span><span class="sxs-lookup"><span data-stu-id="1a5f3-103">Most DKIM set-up issues are related to incorrect DNS records.</span></span>

<span data-ttu-id="1a5f3-104">Da biste rešili probleme sa podešenjem za DKIM, uverite se da je DKIM CNAME zapis (**nije** txt zapis) ispravno oblikovan.</span><span class="sxs-lookup"><span data-stu-id="1a5f3-104">To fix the DKIM set-up issues, verify that the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="1a5f3-105">Više informacija potražite u članku [Šta treba da uradite da biste ručno podesili DKIM u sistemu Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).</span><span class="sxs-lookup"><span data-stu-id="1a5f3-105">For more information, see [What you need to do to manually set up DKIM in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).</span></span>

<span data-ttu-id="1a5f3-106">Ako vam je potrebna pomoć sa DNS zapisima, pogledajte članak [Kreiranje DNS zapisa kod bilo kog dobavljača usluga DNS hostinga za Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span><span class="sxs-lookup"><span data-stu-id="1a5f3-106">If you need help with DNS records in general, see [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span></span>

> [!NOTE]
> <span data-ttu-id="1a5f3-107">Kada kreirate ili ažurirate DKIM DNS zapise u usluzi DNS hostinga za domen, moraćete da sačekate da se DNS zapisi umnože.</span><span class="sxs-lookup"><span data-stu-id="1a5f3-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain, you'll need to wait for the DNS records to propagate.</span></span>
