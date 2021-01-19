---
title: Greške prijavljivanja korisnika
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7790"
- "9004355"
ms.openlocfilehash: 05bd31cb4afecf1342e040eecd9e58cd38bd8d49
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901255"
---
# <a name="user-sign-in-errors"></a><span data-ttu-id="e4fec-102">Greške prijavljivanja korisnika</span><span class="sxs-lookup"><span data-stu-id="e4fec-102">User sign-in errors</span></span>

<span data-ttu-id="e4fec-103">**Rešavanje problema sa dijagnostičkim rešenjem**</span><span class="sxs-lookup"><span data-stu-id="e4fec-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="e4fec-104">Da biste otkrili uzrok ili pronašli probleme u vezi sa prijavljivanjem u korisnika, obavite sledeće korake:</span><span class="sxs-lookup"><span data-stu-id="e4fec-104">To detect the cause or diagnose problems related to user sign-in, perform the following steps:</span></span>

1. <span data-ttu-id="e4fec-105">Pokrenite [dijagnostiku prijavljivanja](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span><span class="sxs-lookup"><span data-stu-id="e4fec-105">Launch the [Sign-in Diagnostic](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
2. <span data-ttu-id="e4fec-106">Pronađite događaj za analizu tako što ćete uneti detalje koje imate o korisniku, aplikaciji, vremenu prijavljivanja, ID-u ili ID-u.</span><span class="sxs-lookup"><span data-stu-id="e4fec-106">Find the event to analyze by entering the details you have about the user, application, time of sign in, request Id, or correlation Id.</span></span>
3. <span data-ttu-id="e4fec-107">Pregledajte rezultate dijagnostike koji prikazuju detalje onoga što se dogodilo i radnje koje možete da izvršite da biste izvršili promene ako je potrebno promena.</span><span class="sxs-lookup"><span data-stu-id="e4fec-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="e4fec-108">**Tražite informacije o šifri greške AADSTS koje su vraćene iz usluge bezbednosnog koda Azure Active Directory (Azure AD)?**</span><span class="sxs-lookup"><span data-stu-id="e4fec-108">**Looking for information about the AADSTS error codes that are returned from the Azure Active Directory (Azure AD) security token service (STS)?**</span></span> <span data-ttu-id="e4fec-109">Pročitajte [Ovaj članak](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) da biste pronašli AADSTS opise grešaka, ispravke i neka predložena zaobilaženja</span><span class="sxs-lookup"><span data-stu-id="e4fec-109">Read [this article](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) to find AADSTS error descriptions, fixes, and some suggested workarounds</span></span>