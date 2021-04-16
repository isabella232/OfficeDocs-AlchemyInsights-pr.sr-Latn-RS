---
title: Treba da označite domen ili pošiljaoca e-pošte kao bezbedne?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792146"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="c2992-102">Treba da označite domen ili pošiljaoca e-pošte kao bezbedne?</span><span class="sxs-lookup"><span data-stu-id="c2992-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="c2992-103">Ne preporučuje se **korišćenje lista** bezbednih pošiljalaca jer otvara vašu organizaciju za napade kao što su upućivanje od phish i phishova.</span><span class="sxs-lookup"><span data-stu-id="c2992-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="c2992-104">Međutim, ako postoji poslovni zahtev, preporučujemo **da** za to **[koristite pravila](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** za protok pošte.</span><span class="sxs-lookup"><span data-stu-id="c2992-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="c2992-105">Naša uputstva obezbeđuju da pošiljalac potvrde identiteta (potvrđuje da domen koji šaljete nije potvrđen) nije potvrđen.</span><span class="sxs-lookup"><span data-stu-id="c2992-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="c2992-106">Napomena: Ne preporučujemo da upravljate pozitivnim informacijama o netačnim pošiljaocima pomoću lista bezbednih pošiljalaca jer izuzeci za filtriranje bez-pošte mogu da otvore organizaciju za bezbednosne **napade.**</span><span class="sxs-lookup"><span data-stu-id="c2992-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="c2992-107">Ako korisnici neispravno primaju poruke koje su pogrešno označene kao bezvredna ili neželjena e-pošta, prijavite poruke **[i datoteke korporaciji Microsoft](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="c2992-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="c2992-108">Bezbedni pošiljaoci u programu Outlook, listi dozvoljenih  pošiljalaca ili listi dozvoljenih domena u smernicama za borbu protiv bezverne e-poruke trebalo bi izbegavati zato što pošiljaoci zaobiđu svu bezvernu, phish zaštitu i phish zaštitu i potvrdu identiteta pošiljaoca (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="c2992-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="c2992-109">Ovaj metod je najbolje koristiti samo za privremeno testiranje.</span><span class="sxs-lookup"><span data-stu-id="c2992-109">This method is best used for temporary testing only.</span></span>
