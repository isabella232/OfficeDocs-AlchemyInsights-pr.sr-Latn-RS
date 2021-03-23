---
title: Rešavanje problema sa AADSTS50000 kodom greške
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
- "9801"
- "9005744"
ms.openlocfilehash: 63689ea5afea7c6921c93f2ead2350f87c2defa8
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037832"
---
# <a name="troubleshoot-aadsts50000-error-code"></a><span data-ttu-id="feb30-102">Rešavanje problema sa AADSTS50000 kodom greške</span><span class="sxs-lookup"><span data-stu-id="feb30-102">Troubleshoot AADSTS50000 error code</span></span>

<span data-ttu-id="feb30-103">Da biste rešili AADSTS50000 grešku, uradite sledeće:</span><span class="sxs-lookup"><span data-stu-id="feb30-103">To resolve AADSTS50000 error, perform the following step:</span></span>

<span data-ttu-id="feb30-104">**AADSTS50000**: tokenizerror – postoji problem sa uslugom prijavljivanja.</span><span class="sxs-lookup"><span data-stu-id="feb30-104">**AADSTS50000**: TokenIssuanceError - There's an issue with the sign-in service.</span></span>

<span data-ttu-id="feb30-105">Ako je zahtev za oznaku pristupa važeći i ovlašćen, server za autorizaciju izdaje oznaku za pristup i opcionalni Token osvežavanja.</span><span class="sxs-lookup"><span data-stu-id="feb30-105">If the access token request is valid and authorized, the authorization server issues an access token and an optional refresh token.</span></span> <span data-ttu-id="feb30-106">Ako zahtev za neuspešnu potvrdu identiteta klijenta nije uspeo ili nije važeći, server za ovlašćenje vraća odgovor na grešku.</span><span class="sxs-lookup"><span data-stu-id="feb30-106">If the request failed client authentication or is invalid, the authorization server returns an error response.</span></span>

<span data-ttu-id="feb30-107">Server za autorizaciju se odaziva sa kodom greške i obuhvata sledeći parametar **greške** sa odgovorom:</span><span class="sxs-lookup"><span data-stu-id="feb30-107">The authorization server responds with an error code and includes the following **error** parameter with the response:</span></span>

`invalid_request: The request is missing a required parameter, includes an unsupported parameter value (other than grant type), repeats a parameter, includes multiple credentials, utilizes more than one mechanism for authenticating the client, or is otherwise malformed.`

`invalid_client: Client authentication failed (e.g., unknown client, no client authentication included, or unsupported authentication method).  The authorization server MAY return an HTTP 401 (Unauthorized) status code to indicate which HTTP authentication schemes are supported.  If the client attempted to authenticate via the "Authorization" request header field, the authorization server MUST respond with an HTTP 401 (Unauthorized) status code and include the "WWW-Authenticate" response header field matching the authentication scheme used by the client.`

`invalid_grant: The provided authorization grant (e.g., authorization code, resource owner credentials) or refresh token is invalid, expired, revoked, does not match the redirection URI used in the authorization request, or was issued to another client.`

`unauthorized_client: The authenticated client is not authorized to use this authorization grant type.`

`unsupported_grant_type: The authorization grant type is not supported by the authorization server.`

`invalid_scope: The requested scope is invalid, unknown, malformed, or exceeds the scope granted by the resource owner.`

<span data-ttu-id="feb30-108">[Otvorite ulaznicu za podršku](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-troubleshooting-support-howto) da biste rešili ovaj problem.</span><span class="sxs-lookup"><span data-stu-id="feb30-108">[Open a support ticket](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-troubleshooting-support-howto) to resolve this issue.</span></span>