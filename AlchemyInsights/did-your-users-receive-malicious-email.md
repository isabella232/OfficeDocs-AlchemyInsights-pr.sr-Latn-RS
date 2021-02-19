---
title: Da li su korisnici dobili zlonamernu e-poštu
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
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 2197e7f195d789193798b80cb092d8046eb6e0be
ms.sourcegitcommit: 3c708a4a349b60b59bc623c44fb78674c685f3c2
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 02/18/2021
ms.locfileid: "50291806"
---
# <a name="did-your-users-receive-malicious-email"></a><span data-ttu-id="9a064-102">Da li su korisnici dobili zlonamernu e-poštu?</span><span class="sxs-lookup"><span data-stu-id="9a064-102">Did your users receive malicious email?</span></span>

- <span data-ttu-id="9a064-103">Sada možete da prijavite zlonamernu e-poštu korporaciji Microsoft putem opcije [Prosleđivanja administratora u Centru za bezbednost i usaglašenost](https://sip.protection.office.com/reportsubmission).</span><span class="sxs-lookup"><span data-stu-id="9a064-103">You can now report the malicious email to Microsoft using the [Admin Submissions in Security & Compliance Center](https://sip.protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="9a064-104">Poruke koje su prosleđene u [prosleđivanja administratora](https://sip.protection.office.com/reportsubmission) se skeniraju a sledeći rezultati se prikazuju u iskačućem prozoru **detalja**:</span><span class="sxs-lookup"><span data-stu-id="9a064-104">Messages that are submitted in [admin submissions](https://sip.protection.office.com/reportsubmission) are scanned, and the following results shown in the **details** flyout:</span></span>

- <span data-ttu-id="9a064-105">Ako je došlo do greške prilikom potvrde identiteta e-poruke pošiljaoca u vreme isporuke.</span><span class="sxs-lookup"><span data-stu-id="9a064-105">If there was a failure in the sender's email authentication at the time of delivery.</span></span>
- <span data-ttu-id="9a064-106">Informacije o broju pogodaka smernica koji su možda uticali na odluku o poruci ili su je zamenili.</span><span class="sxs-lookup"><span data-stu-id="9a064-106">Information about any policy hits that could have affected or overridden the verdict of a message.</span></span>
- <span data-ttu-id="9a064-107">Trenutni rezultati neutralizacije koje treba videti ako su URL adrese ili datoteke sadržane u poruci bile zlonamerne ili ne.</span><span class="sxs-lookup"><span data-stu-id="9a064-107">Current detonation results to see if the URLs or files contained in the message were malicious or not.</span></span>
- <span data-ttu-id="9a064-108">Povratne informacije od ocenjivača</span><span class="sxs-lookup"><span data-stu-id="9a064-108">Feedback from graders</span></span>

<span data-ttu-id="9a064-109">Ako je pronađena zamena, ponovno skeniranje treba da se dovrši za nekoliko minuta.</span><span class="sxs-lookup"><span data-stu-id="9a064-109">If an override was found, the rescan should complete in several minutes.</span></span> <span data-ttu-id="9a064-110">Ako nije bilo problema u potvrdi identiteta e-pošte ili ako zamena nije uticala na isporuku, onda povratne informacije od ocenjivača mogu potrajati i do jedan dan.</span><span class="sxs-lookup"><span data-stu-id="9a064-110">If there wasn't a problem in email authentication or if the delivery wasn't affected by an override, then the feedback from graders could take up to a day.</span></span>

<span data-ttu-id="9a064-111">Ako se ne složite sa konačnom odlukom o poruci, URL adresi ili datoteci (blokirano ili neblokirano), prosledite poruku za ponovno skeniranje nakon jednog dana.</span><span class="sxs-lookup"><span data-stu-id="9a064-111">If you disagree with the final verdict on a message, URL or file (blocked vs. not blocked), submit the message again after a day for rescan.</span></span> <span data-ttu-id="9a064-112">Velike su šanse da odluka neće biti promenjena nakon ponovnog prosleđivanja poruke.</span><span class="sxs-lookup"><span data-stu-id="9a064-112">The chances are high that the verdict would change after submitting the message again.</span></span>

<span data-ttu-id="9a064-113">U međuvremenu zlonamernu e-poruku možete da uklonite iz prijemnog sandučeta korisnika tako što ćete pratiti uputstvo iz [ovog članka](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).</span><span class="sxs-lookup"><span data-stu-id="9a064-113">Meanwhile, you can remove malicious email from user inboxes by following the instructions in [this article](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).</span></span>

- <span data-ttu-id="9a064-114">Klijenti sa uslugom Microsoft zaštitnik za Office 365 mogu da:</span><span class="sxs-lookup"><span data-stu-id="9a064-114">Customers with Microsoft Defender for Office 365 can:</span></span>
    - <span data-ttu-id="9a064-115">koriste [Istraživač pretnji za pronalaženje i brisanje sumnjivih e-poruka](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span><span class="sxs-lookup"><span data-stu-id="9a064-115">use [Threat Explorer to Find and Delete Suspicious email](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span></span>
    - <span data-ttu-id="9a064-116">[koriste bezbedne veze za blokiranje pristupa](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) zlonamernim URL adresama</span><span class="sxs-lookup"><span data-stu-id="9a064-116">[use Safe Links to block access](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) to a malicious URL</span></span>
    - <span data-ttu-id="9a064-117">prate korisnike koji su kliknuli na zlonamernu URL adresu i pristupili joj: [Prikažite URL koji sadrži phishing i kliknite na podatke o odluci](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Preuzmi-praćenjeURL-a](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span><span class="sxs-lookup"><span data-stu-id="9a064-117">track users who clicked and accessed malicious URLs: [View phishing URL and click verdict data](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span></span>
    - <span data-ttu-id="9a064-118">ručno [pokrenu automatizovano ispitivanje](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span><span class="sxs-lookup"><span data-stu-id="9a064-118">manually [start an Automated Investigation](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span></span>

<span data-ttu-id="9a064-119">Takođe možete da se zaštitite od zlonamernih datoteka i URL adresa tako što ćete pratiti uputstvo u članku [Zaštita od zlonamernih URL adresa i datoteka](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).</span><span class="sxs-lookup"><span data-stu-id="9a064-119">You can also protect against malicious files and URLs by following the instructions in [Protection from malicious URLs and files](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).</span></span>