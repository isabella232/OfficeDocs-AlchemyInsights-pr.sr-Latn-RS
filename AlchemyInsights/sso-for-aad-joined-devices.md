---
title: Single-Sign je za Azure Active Directory pridružene uređaje
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
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405659"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a><span data-ttu-id="58f5a-102">Jedinstveno prijavljivanje za Azure Active Directory pridružene uređaje</span><span class="sxs-lookup"><span data-stu-id="58f5a-102">Single-sign on for Azure Active Directory Joined Devices</span></span>

<span data-ttu-id="58f5a-103">Ako imate okruženje iz usluge Active Directory (AD) i želite da se pridružite računarima pridruženim AD domenu u uslugu Azure AD, to možete da postignete tako što ćete izvršiti hibridno Azure AD pridruživanje.</span><span class="sxs-lookup"><span data-stu-id="58f5a-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="58f5a-104">Kako [da: Planirate hibridnu primenu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) pridruživanja pružaju vam srodne korake za primenu hibridnog Azure AD pridruživanja u okruženju.</span><span class="sxs-lookup"><span data-stu-id="58f5a-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

[<span data-ttu-id="58f5a-105">Konfigurisanje Azure AD pridruženih uređaja za Single-Sign Na korišćenje usluge Windows Hello za posao</span><span class="sxs-lookup"><span data-stu-id="58f5a-105">Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business</span></span>](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

<span data-ttu-id="58f5a-106">**Problemi sa primarnim tokenim osvežavanja (PRT)** Primarni token osvežavanja (PRT) je ključni artikt Azure AD potvrde identiteta na Windows 10, Windows Server 2016 i novijim verzijama, iOS i Android uređajima.</span><span class="sxs-lookup"><span data-stu-id="58f5a-106">**Primary Refresh Token (PRT) issues** A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="58f5a-107">To je JSON veb token (JWT) posebno izdat Microsoft raskidačima tokena za prve strane kako bi se omogućilo jedinstveno prijavljivanje (SSO) u svim aplikacijama koje se koriste na tim uređajima.</span><span class="sxs-lookup"><span data-stu-id="58f5a-107">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="58f5a-108">[U 1.](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)izdanju Šta je to primarni token za osvežavanje? pružićemo detalje o tome kako se PRT izdaje, koristi i štiti na Windows 10 uređajima.</span><span class="sxs-lookup"><span data-stu-id="58f5a-108">[In What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), we will provide details on how a PRT is issued, used, and protected on Windows 10 devices.</span></span>

<span data-ttu-id="58f5a-109">**WamDefaultSet: YES i AzureADPrt: YES** Ova polja ukazuju na to da li je korisnik uspešno potvrdio identitet za Azure AD prilikom prijave na uređaj.</span><span class="sxs-lookup"><span data-stu-id="58f5a-109">**WamDefaultSet: YES and AzureADPrt: YES** These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="58f5a-110">Ako su vrednosti **NE**, može biti krajnji rok:</span><span class="sxs-lookup"><span data-stu-id="58f5a-110">If the values are **NO**, it could be due:</span></span>

- <span data-ttu-id="58f5a-111">Loš ključ za skladištenje u TPM-u povezanom sa uređajem nakon registracije (proverite KeySignTest dok ste pokrenuti sa punim punim brojem).</span><span class="sxs-lookup"><span data-stu-id="58f5a-111">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).</span></span>
- <span data-ttu-id="58f5a-112">Alternativni ID za prijavljivanje</span><span class="sxs-lookup"><span data-stu-id="58f5a-112">Alternate Login ID</span></span>
- <span data-ttu-id="58f5a-113">HTTP proxy nije pronađen</span><span class="sxs-lookup"><span data-stu-id="58f5a-113">HTTP Proxy not found</span></span>

<span data-ttu-id="58f5a-114">Rešavanje problema sa uređajima pomoću dsregcmd komande – [SSO stanje](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="58f5a-114">Troubleshoot devices using the dsregcmd command - [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span></span>
