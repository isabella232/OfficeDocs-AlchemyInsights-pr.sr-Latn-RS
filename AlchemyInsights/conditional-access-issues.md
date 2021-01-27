---
title: Problemi sa uslovnim pristupom
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015001"
---
# <a name="conditional-access-issues"></a><span data-ttu-id="8d046-102">Problemi sa uslovnim pristupom</span><span class="sxs-lookup"><span data-stu-id="8d046-102">Conditional access issues</span></span>

<span data-ttu-id="8d046-103">**Rešavanje problema sa dijagnostičkim rešenjem**</span><span class="sxs-lookup"><span data-stu-id="8d046-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="8d046-104">Možete brzo da saznate šta se dešava ili pronađu probleme u vezi sa prijavljivanjem korisnika pomoću [dijagnostike za prijavljivanje](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span><span class="sxs-lookup"><span data-stu-id="8d046-104">You can quickly find out what happened or diagnose problems related to user sign-in by using the [Sign-in Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span></span>

1. <span data-ttu-id="8d046-105">Pokrenite dijagnostiku prijavljivanja.</span><span class="sxs-lookup"><span data-stu-id="8d046-105">Launch the Sign-in Diagnostic.</span></span>
1. <span data-ttu-id="8d046-106">Pronađite događaj koji treba analizirati tako što ćete uneti detalje koje imate o korisniku, aplikaciji, vremenu prijavljivanja, ID-u zahteva ili ID korelacije.</span><span class="sxs-lookup"><span data-stu-id="8d046-106">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="8d046-107">Pregledajte rezultate dijagnoze koji prikazuju detalje šta se dogodilo i koje radnje možete preduzeti da biste izvršili promene (ako su potrebne promene).</span><span class="sxs-lookup"><span data-stu-id="8d046-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes (if any changes are needed).</span></span>

<span data-ttu-id="8d046-108">**Koraci za rešavanje problema sa prijavljivanjem**</span><span class="sxs-lookup"><span data-stu-id="8d046-108">**Steps to Troubleshoot a Sign-In**</span></span> 

1. <span data-ttu-id="8d046-109">Idite na stranicu za prijavljivanje na Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8d046-109">Navigate to the Azure AD Sign-in page.</span></span>
1. <span data-ttu-id="8d046-110">Prijavljivanje na filtriranje pomoću korisnika, vremenske vrednosti, zatvaranja, statusa, aplikacije klijenta itd.</span><span class="sxs-lookup"><span data-stu-id="8d046-110">Filter sign-ins by user, time range, application, status, client app, and so on.</span></span>
1. <span data-ttu-id="8d046-111">Izaberite događaj prijavljivanja i prikažite karticu uslovno pristup da biste videli koje smernice se procenjuju.</span><span class="sxs-lookup"><span data-stu-id="8d046-111">Select a sign-in event and view the Conditional Access tab to see which policies were evaluated.</span></span>
1. <span data-ttu-id="8d046-112">Kliknite na redu smernica da biste prikazali detalje o politici i razumeli zašto se to odnosi.</span><span class="sxs-lookup"><span data-stu-id="8d046-112">Click on the row of a policy to view the policy details and understand why it applied.</span></span>

<span data-ttu-id="8d046-113">**Alatke za rešavanje problema sa uslovnim pristupom**</span><span class="sxs-lookup"><span data-stu-id="8d046-113">**Tools to troubleshoot a Conditional Access policy**</span></span>

- <span data-ttu-id="8d046-114">Režim samo za izveštavanje omogućava vam da procenite smernice bez zaostalih korisnika.</span><span class="sxs-lookup"><span data-stu-id="8d046-114">Report-only mode lets you evaluate a policy without impacting users.</span></span>
- <span data-ttu-id="8d046-115">Alatka "Šta-ako" vam omogućava da simulirate događaje prijavljivanja i vidite koje se smernice primenjuju.</span><span class="sxs-lookup"><span data-stu-id="8d046-115">What-if tool lets you simulate sign-in events and see which policies apply.</span></span>
- <span data-ttu-id="8d046-116">Radna sveska sa shvatanju i prijavljivanju prikazuje uticaj svake smernice u realnom vremenu.</span><span class="sxs-lookup"><span data-stu-id="8d046-116">Insights and reporting workbook displays real-time impact of each policy.</span></span>

<span data-ttu-id="8d046-117">**Smernice za zaštitu osnovnih linija**</span><span class="sxs-lookup"><span data-stu-id="8d046-117">**Baseline Protection Policies**</span></span>

<span data-ttu-id="8d046-118">Smernice za zaštitu osnovnih linija su neodobrene.</span><span class="sxs-lookup"><span data-stu-id="8d046-118">Baseline Protection policies have been deprecated.</span></span> <span data-ttu-id="8d046-119">Više se ne primenjuju i uskoro će biti uklonjene iz Azure portala.</span><span class="sxs-lookup"><span data-stu-id="8d046-119">They are no longer being enforced and will soon be removed from Azure portal.</span></span> <span data-ttu-id="8d046-120">Preporučujemo omogućavanje [postavki bezbednosti](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="8d046-120">We recommend enabling [security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span>

<span data-ttu-id="8d046-121">Više informacija o uslovnom pristupu potražite u članku:</span><span class="sxs-lookup"><span data-stu-id="8d046-121">For more information on Conditional Access see:</span></span>

<span data-ttu-id="8d046-122">[Najbolje prakse za uslovno pristup u usluzi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Uslovi u uslovnom pristupu](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Kontrole u uslovnom pristupu](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Lokacije u uslovnom pristupu](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span><span class="sxs-lookup"><span data-stu-id="8d046-122">[Best practices for conditional access in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Conditions in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Controls in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/controls) 
[Locations in Conditional Access ](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span></span>
