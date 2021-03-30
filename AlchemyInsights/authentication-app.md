---
title: Aplikacija za potvrdu identiteta
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405679"
---
# <a name="authentication-app"></a><span data-ttu-id="50f42-102">Aplikacija za potvrdu identiteta</span><span class="sxs-lookup"><span data-stu-id="50f42-102">Authentication app</span></span>

<span data-ttu-id="50f42-103">Ako ste globalni administ, možete brzo da saznate šta se dogodilo ili da ustanovite probleme povezane sa korisničkim prijavljivanjem pomoću funkcije "Dijagnostika [za prijavljivanje"](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span><span class="sxs-lookup"><span data-stu-id="50f42-103">If you are a Global Admin, you can quickly find out what happened or diagnose problems related to user-sign in by using the [Sign-in Diagnostics](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>

1. <span data-ttu-id="50f42-104">Pokrenite dijagnostiku tako što ćete kliknuti na dugme["Pokreni dijagnostiku".](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="50f42-104">Start the diagnostics by clicking "[Launch Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" button.</span></span> 
1. <span data-ttu-id="50f42-105">Pronađite događaj za analiziranje tako što ćete uneti detalje koje imate o korisniku, aplikaciji, vremenu prijave, ID-u zahteva ili ID-u korelacije.</span><span class="sxs-lookup"><span data-stu-id="50f42-105">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="50f42-106">Pregledajte dijagnostički rezultate koji pokazuju detalje o tome šta se dogodilo i koje radnje možete preduzeti da biste promenili po potrebi.</span><span class="sxs-lookup"><span data-stu-id="50f42-106">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="50f42-107">**Proverite da li je scenario primenljiv:**</span><span class="sxs-lookup"><span data-stu-id="50f42-107">**Check the scenario that is applicable:**</span></span>

1. <span data-ttu-id="50f42-108">Ako korisnik ne dobija push obaveštenje u aplikaciji Microsoft Authenticator, potvrdite da se korisnici ne prikazuju u okviru MFA blokiranih korisnika kao što je opisano u članku Blokiranje i [deblokiranje korisnika.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="50f42-108">If a user is not getting a push notification in the Microsoft Authenticator app, verify they are not shown under the MFA blocked users as described in [Block and unblock users](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
1. <span data-ttu-id="50f42-109">Ako korisnik nije blokiran za MFA, ali ne primi push obaveštenje, može da otvori aplikaciju Microsoft Authenticator, koja povlači zahteve za odobrenje na čekanju.</span><span class="sxs-lookup"><span data-stu-id="50f42-109">If the user is not blocked for MFA but does not receive a push notification, they can open the Microsoft Authenticator app, which will pull the pending approval requests.</span></span>
1. <span data-ttu-id="50f42-110">Kao alternativni metod prijave, korisnik može i da klikne na "Prijavite se na drugi način" i odabere da koristi kôd za verifikaciju iz moje aplikacije za mobilne uređaje.</span><span class="sxs-lookup"><span data-stu-id="50f42-110">As an alternative sign-in method, the user can also click on Sign in another way and choose use a verification code from my mobile app.</span></span>
1. <span data-ttu-id="50f42-111">Aplikacija Microsoft Authenticator je jedini dostupan metod za veliki broj korisnika.</span><span class="sxs-lookup"><span data-stu-id="50f42-111">The Microsoft Authenticator App is the only available method for many users.</span></span> <span data-ttu-id="50f42-112">[Saznajte više o podrazumevanim vrednostima bezbednosti](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), najčešća pitanja o aplikaciji [Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) za najčešća pitanja i kako da ih rešite.</span><span class="sxs-lookup"><span data-stu-id="50f42-112">[Learn more about security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), check [Authenticator App FAQ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) for commonly asked questions and how to resolve them.</span></span>
 
<span data-ttu-id="50f42-113">**Preporučeni video zapisi**</span><span class="sxs-lookup"><span data-stu-id="50f42-113">**Recommended Videos**</span></span>

<span data-ttu-id="50f42-114">[Kako da podesite aplikaciju Authenticator na novom telefonu (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="50f42-114">[How to set up Authenticator App on a new phone (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span></span>
