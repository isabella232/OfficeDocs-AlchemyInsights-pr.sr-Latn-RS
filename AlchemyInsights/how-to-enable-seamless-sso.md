---
title: Kako da omogućite besprekoran SSO
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "628"
- "1300012"
ms.assetid: 80c88b2d-adb1-4e45-8eff-aaa80403b5b6
ms.openlocfilehash: f3581549823e1ec650a3717780bc07e9944d4c1c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780541"
---
# <a name="how-to-enable-seamless-sso"></a><span data-ttu-id="7435a-102">Kako da omogućite besprekoran SSO</span><span class="sxs-lookup"><span data-stu-id="7435a-102">How to enable Seamless SSO</span></span>

<span data-ttu-id="7435a-103">Omogućite besprekoran SSO kroz [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span><span class="sxs-lookup"><span data-stu-id="7435a-103">Enable Seamless SSO through [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span></span>
  
<span data-ttu-id="7435a-104">Ako radite na novoj instalaciji usluge Azure AD Connect, odaberite stavku [Prilagođena instalacija](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span><span class="sxs-lookup"><span data-stu-id="7435a-104">If you're doing a fresh installation of Azure AD Connect, choose the [custom installation path](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span></span> <span data-ttu-id="7435a-105">Na stranici za **Prijavljivanje korisnika** odaberite opciju **Omogućavanje jedinstvenog prijavljivanja** .</span><span class="sxs-lookup"><span data-stu-id="7435a-105">At the **User sign-in** page, choose the **Enable single sign-on** option.</span></span>
  
<span data-ttu-id="7435a-106">Da biste potvrdili da ste ispravno omogućili besprekoran SSO:</span><span class="sxs-lookup"><span data-stu-id="7435a-106">To verify that you have enabled Seamless SSO correctly:</span></span>
  
1. <span data-ttu-id="7435a-107">Prijavite se u [administrativni centar Azure Active Directory](https://aad.portal.azure.com) kao globalni administrator.</span><span class="sxs-lookup"><span data-stu-id="7435a-107">Sign in to the [Azure Active Directory administrative center](https://aad.portal.azure.com) as a global admin.</span></span>

2. <span data-ttu-id="7435a-108">U levom oknu izaberite stavku **Azure Active Directory** .</span><span class="sxs-lookup"><span data-stu-id="7435a-108">Select **Azure Active Directory** in the left pane.</span></span>

3. <span data-ttu-id="7435a-109">Potvrdite da je Nesmetna jedinstveno prijavljivanje **omogućena**.</span><span class="sxs-lookup"><span data-stu-id="7435a-109">Verify that Seamless single sign-on is **Enabled**.</span></span>

<span data-ttu-id="7435a-110">Da biste saznali više, pogledajte [Azure Active Directory Nesmetna prijavljivanje: brzi početak](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span><span class="sxs-lookup"><span data-stu-id="7435a-110">To learn more, see [Azure Active Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span></span>
  