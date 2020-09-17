---
title: Treba da označite domen ili pošiljalac e-pošte bezbedan?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803259"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="823b9-102">Treba da označite domen ili pošiljalac e-pošte bezbedan?</span><span class="sxs-lookup"><span data-stu-id="823b9-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="823b9-103">Korišćenje **Lista bezbednih pošiljalaca se ne preporučuje** jer otvara vašu organizaciju u spam, Fish i lažne napade.</span><span class="sxs-lookup"><span data-stu-id="823b9-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="823b9-104">Međutim, ako postoji uslov za posao, **preporučujemo** da koristite **[pravila toka pošte](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** za ovo.</span><span class="sxs-lookup"><span data-stu-id="823b9-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="823b9-105">Naše vođstvo osigurava potvrdu identiteta pošiljaoca (Verifikacija slanja domena nije lažnjava).</span><span class="sxs-lookup"><span data-stu-id="823b9-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="823b9-106">**Napomena**: ne preporučujemo da upravljate lažnim sigurnošću pomoću lista pouzdanih pošiljalaca, jer izuzeci od filtriranja bezvredne pošte mogu da otvore vašu organizaciju bezbednosnim napadima.</span><span class="sxs-lookup"><span data-stu-id="823b9-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="823b9-107">Ako korisnici primaju poruke koje su pogrešno označene kao bezvredne ili neželjene e-pošte, **[Prijavite poruke i datoteke korporaciji Microsoft](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="823b9-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="823b9-108">Pouzdani pošiljaoci u programu Outlook, dozvoljeni spisak poљiljaocu ili dozvoljenu listu domena u smernicama za borbu protiv bezvredne pošte **treba izbegavati** zato što pošiljaoci zaobilaze sve bezvredne, podve i Phish potvrdu identiteta pošiljaoca (SPF, dkim, dmarc).</span><span class="sxs-lookup"><span data-stu-id="823b9-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="823b9-109">Ovaj metod se najbolje koristi samo za privremeno testiranje.</span><span class="sxs-lookup"><span data-stu-id="823b9-109">This method is best used for temporary testing only.</span></span>
