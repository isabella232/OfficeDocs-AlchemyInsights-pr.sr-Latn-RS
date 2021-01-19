---
title: Rešavanje problema sa korisničkim odobravama
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7785"
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901631"
---
# <a name="troubleshoot-user-consent"></a><span data-ttu-id="baf40-102">Rešavanje problema sa korisničkim odobravama</span><span class="sxs-lookup"><span data-stu-id="baf40-102">Troubleshoot user consent</span></span>

1. <span data-ttu-id="baf40-103">Možete da konfigurišete kako krajnji korisnici odobravate aplikacije putem Azure portala ili PowerShell.</span><span class="sxs-lookup"><span data-stu-id="baf40-103">You can configure how end-users consent to applications through the Azure Portal or PowerShell.</span></span> <span data-ttu-id="baf40-104">Više informacija potražite u članku [postavke korisničkog pristanka](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) .</span><span class="sxs-lookup"><span data-stu-id="baf40-104">See [User consent settings](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) for more information.</span></span>
1. <span data-ttu-id="baf40-105">Administrator može da koristi i [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) za odobravanje saglasnosti za delegirane dozvole u ime jednog korisnika.</span><span class="sxs-lookup"><span data-stu-id="baf40-105">An administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="baf40-106">Više informacija potražite u članku [pristup pristupu u ime korisnika](https://docs.microsoft.com/graph/auth-v2-user).</span><span class="sxs-lookup"><span data-stu-id="baf40-106">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>
1. <span data-ttu-id="baf40-107">[Greške korisnika](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): ovaj članak govori o greškama koje se mogu pojaviti tokom procesa saglasnosti sa primenom aplikacije.</span><span class="sxs-lookup"><span data-stu-id="baf40-107">[User Consent Errors](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): this article discusses errors that can occur during the process of consenting to an application.</span></span> <span data-ttu-id="baf40-108">Ako rešavate neočekivani pristanak koji ne sadrže nijednu poruku o grešci, pročitajte članak [scenariji potvrde identiteta za Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span><span class="sxs-lookup"><span data-stu-id="baf40-108">If you are troubleshooting unexpected consent prompts that do not contain any error messages, see [Authentication Scenarios for Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>