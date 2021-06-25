---
title: Razmena e-pošte putem sistema Microsoft 365
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
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 3b07dd4ccc8570e77a9ce30df48f9ac987a1db71
ms.sourcegitcommit: 93292c46464ac94971d11adfb808d066ab8bc406
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/24/2021
ms.locfileid: "53117997"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="a1529-102">Kako da podesite višefunkcionalni uređaj ili aplikaciju za slanje e-pošte</span><span class="sxs-lookup"><span data-stu-id="a1529-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="a1529-103">Da biste saznali koje opcije imate i koje korake treba da izvršite, pogledajte članak [Kako da podesite višefunkcionalni uređaj ili aplikaciju za slanje e-pošte pomoću sistema Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="a1529-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="a1529-104">Ako imate uređaj ili aplikaciju koji su nedavno prestali da rade, najčešći problemi su:</span><span class="sxs-lookup"><span data-stu-id="a1529-104">If you have a device or application that recently stopped working, the most common issues are:</span></span>

- <span data-ttu-id="a1529-105">**Greške u vezi sa potvrdom identiteta prilikom korišćenja prosleđivanja SMTP Auth klijenta** Nedavno smo napravili neke promene u vezi sa načinom na koji funkcioniše SMTP potvrda identiteta.</span><span class="sxs-lookup"><span data-stu-id="a1529-105">**Authentication related errors while using SMTP Auth client submission** We recently made some changes related to how SMTP Authentication works.</span></span> <span data-ttu-id="a1529-106">Više informacija o rešavanju problema potražite u odeljku "Potvrda identiteta bezuspešno" u odeljku Rešavanje problema sa štampačima, skenerima i aplikacijama za LOB koji šalju e-poštu pomoću Microsoft 365 ili [Office 365.](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)</span><span class="sxs-lookup"><span data-stu-id="a1529-106">For more information about how to resolve issues, see the authentication unsuccessful section of [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).</span></span>
- <span data-ttu-id="a1529-107">**Prihvatamo samo TLS 1.2 verziju i obezbeđujemo bezbednu vezu sa Office 365** Ako koristite bezbednu vezu (TLS), uverite se da uređaj aplikacije podržava TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="a1529-107">**We accept only the TLS 1.2 version while making a secure connection to Office 365** If you're using Secure connection (TLS), make sure your application device supports TLS 1.2.</span></span> <span data-ttu-id="a1529-108">Više informacija potražite u [temi Priprema za TLS 1.2](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)u Office 365 i Office 365 GCC.</span><span class="sxs-lookup"><span data-stu-id="a1529-108">For more information, see [Preparing for TLS 1.2 in Office 365 and Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).</span></span>
 
<span data-ttu-id="a1529-109">Druge probleme i rešenja možete da pronađete u temi Rešavanje problema sa štampačima, skenerima i aplikacijama za LOB koji šalju e-poštu pomoću [Microsoft 365 ili Office 365.](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)</span><span class="sxs-lookup"><span data-stu-id="a1529-109">For other issues and solutions, see [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).</span></span>

<span data-ttu-id="a1529-110">Da biste videli pogođene uređaje, idite na [Izveštaj o klijentima SMTP potvrde identiteta](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="a1529-110">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span>

<span data-ttu-id="a1529-111">**Napomi:** Exchange Online ne prati scenarije masovnog slanja.</span><span class="sxs-lookup"><span data-stu-id="a1529-111">**Note**: Exchange Online doesn't accommodate bulk-mailing scenarios.</span></span> <span data-ttu-id="a1529-112">Da biste slali masovnu komercijalnu e-poštu (na primer, bištani klijenata), trebalo bi da koristite nezavisne dobavljače koji su specijalizovani za ove usluge.</span><span class="sxs-lookup"><span data-stu-id="a1529-112">To send bulk commercial email (for example, customer newsletters), you should use third-party providers that specialize in these services.</span></span>
