---
title: Rešavanje problema sa kodom Azure AD potvrde identiteta i autorizacije (AADSTS)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037837"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a><span data-ttu-id="12c31-102">Rešavanje problema sa kodom Azure AD potvrde identiteta i autorizacije (AADSTS)</span><span class="sxs-lookup"><span data-stu-id="12c31-102">Troubleshoot Azure AD Authentication and Authorization (AADSTS) error codes</span></span>

<span data-ttu-id="12c31-103">Da biste rešili AAD potvrde identiteta i lozinke (AADSTS), obavite sledeće preporučene korake:</span><span class="sxs-lookup"><span data-stu-id="12c31-103">To resolve AAD authentication and authorization error codes (AADSTS), perform the following recommended steps:</span></span>

1. <span data-ttu-id="12c31-104">**Rukovanje šifri grešaka u aplikaciji**</span><span class="sxs-lookup"><span data-stu-id="12c31-104">**Handling error codes in your application**</span></span>

- <span data-ttu-id="12c31-105">**OAuth 2.0 spec**, https://tools.ietf.org/html/rfc6749#section-5.2 pruža uputstva za rukovanje greškama tokom potvrde identiteta pomoću dela greške na osnovu odgovora na grešku.</span><span class="sxs-lookup"><span data-stu-id="12c31-105">The **OAuth2.0 spec**, https://tools.ietf.org/html/rfc6749#section-5.2, provides guidance on how to handle errors during authentication using the error portion of the error response.</span></span>

    - <span data-ttu-id="12c31-106">**Greška**: niska koda greške koja se može koristiti za klasifikaciju tipova grešaka koje se javljaju i treba da se koristi za reagovanje na greške.</span><span class="sxs-lookup"><span data-stu-id="12c31-106">**error**: An error code string that can be used to classify types of errors that occur, and should be used to react to errors.</span></span>
    - <span data-ttu-id="12c31-107">Polje " **Greška** " ima nekoliko mogućih vrednosti – pregledajte veze podataka protokola i OAuth 2,0 specifikacije za više informacija o određenim greškama i kako da reagujete na njih.</span><span class="sxs-lookup"><span data-stu-id="12c31-107">The **error** field has several possible values - review the protocol documentation links and OAuth 2.0 specs for more information about specific errors and how to react to them.</span></span>

- <span data-ttu-id="12c31-108">Evo uzorka odgovora o grešci:</span><span class="sxs-lookup"><span data-stu-id="12c31-108">Here is a sample error response:</span></span>
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. <span data-ttu-id="12c31-109">**Pronalaženje trenutnih informacija sa kodom greške**</span><span class="sxs-lookup"><span data-stu-id="12c31-109">**Lookup current error code information**</span></span>

- <span data-ttu-id="12c31-110">Kodovi grešaka i poruke podležu promenama.</span><span class="sxs-lookup"><span data-stu-id="12c31-110">Error codes and messages are subject to change.</span></span> <span data-ttu-id="12c31-111">Za najnovije informacije pogledajte https://login.microsoftonline.com/error stranicu da biste pronašli AADSTS opise grešaka, ispravke i neka predložena rešenja.</span><span class="sxs-lookup"><span data-stu-id="12c31-111">For the most current information, see the https://login.microsoftonline.com/error page to find AADSTS error descriptions, fixes, and some suggested workarounds.</span></span>
- <span data-ttu-id="12c31-112">Možete da tražite i rešite probleme sa [kodom greške](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) koji su navedeni u članku [Azure AD potvrda identiteta i lozinke](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span><span class="sxs-lookup"><span data-stu-id="12c31-112">You can also search for and troubleshoot [AADSTS error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) listed in the article [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span></span>

3. <span data-ttu-id="12c31-113">**Nabavite pomoć**</span><span class="sxs-lookup"><span data-stu-id="12c31-113">**Get Help**</span></span>

- <span data-ttu-id="12c31-114">[Opcije podrške i pomoći za programere](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) – ako vam je potreban odgovor na pitanje ili pomoć u rešavanju problema koji nije obuhvaćena naљom dokumentacijom, možda je vreme da se obratite ekspertima za pomoć.</span><span class="sxs-lookup"><span data-stu-id="12c31-114">[Support and help options for developers](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) - If you need an answer to a question or help in solving a problem not covered in our documentation, it might be time to reach out to experts for help.</span></span> <span data-ttu-id="12c31-115">Ovaj članak pruža nekoliko predloga za dobijanje odgovora na pitanja dok razvijate aplikacije koje se integrišu sa Microsoft platformom identiteta.</span><span class="sxs-lookup"><span data-stu-id="12c31-115">This article provides several suggestions for getting answers to your questions as you develop apps that integrate with the Microsoft identity platform.</span></span>








