---
title: Dozvole za API i pristanak
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
- "9004343"
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974992"
---
# <a name="api-permissions-and-consent"></a><span data-ttu-id="1af5a-102">Dozvole za API i pristanak</span><span class="sxs-lookup"><span data-stu-id="1af5a-102">API permissions and consent</span></span>

<span data-ttu-id="1af5a-103">Aplikacije koje se integrišu sa Microsoft platformom za identifikaciju slede model identiteta koji korisnicima i administratori pružaju kontrolu nad načinom na koji se podaci mogu pristupiti.</span><span class="sxs-lookup"><span data-stu-id="1af5a-103">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="1af5a-104">Primena modela autorizacije ažurirana je na krajnjoj tački Microsoft platforme identiteta.</span><span class="sxs-lookup"><span data-stu-id="1af5a-104">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint.</span></span> <span data-ttu-id="1af5a-105">Menja kako aplikacija mora da komunicira sa Microsoft platformom identiteta.</span><span class="sxs-lookup"><span data-stu-id="1af5a-105">It changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="1af5a-106">[Dozvole i pristanak u krajnjoj tački Microsoft platforme identiteta](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) pokrivaju osnovne koncepte ovog modela autorizacije, uključujući opsege, dozvole i saglasnost.</span><span class="sxs-lookup"><span data-stu-id="1af5a-106">[Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) covers the basic concepts of this authorization model, including scopes, permissions, and consent.</span></span>

<span data-ttu-id="1af5a-107">Okvir za pristup [Azure Active Directory (AZURE AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) olakšava razvijanje Veb lokacija multi-zakupaca i izvornih klijentskih aplikacija.</span><span class="sxs-lookup"><span data-stu-id="1af5a-107">The [Azure Active Directory (Azure AD) consent framework](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) makes it easy to develop multi-tenant web and native client applications.</span></span> <span data-ttu-id="1af5a-108">Ove aplikacije mogu da se prijave po korisničkim nalozima od Azure AD zakupca koji se razlikuje od onog u kom se registruje aplikacija.</span><span class="sxs-lookup"><span data-stu-id="1af5a-108">These applications allow sign-in by user accounts from an Azure AD tenant that's different from the one where the application is registered.</span></span> <span data-ttu-id="1af5a-109">Možda će biti potrebno da pristupe i vebu Veb Appsu, kao što je Microsoft Graph API (za pristup Azure AD, Intune i uslugama u programu Microsoft 365) i drugim AFIS uslugama Microsoft Services, pored sopstvenog Veb APIs.</span><span class="sxs-lookup"><span data-stu-id="1af5a-109">They may also need to access web APIs such as the Microsoft Graph API (to access Azure AD, Intune, and services in Microsoft 365) and other Microsoft services' APIs, in addition to your own web APIs.</span></span>

