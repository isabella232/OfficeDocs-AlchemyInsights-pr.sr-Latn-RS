---
title: Rešavanje problema sa jednim znakom za Azure AD koji se pridružuje
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037331"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a><span data-ttu-id="94dcf-102">Rešavanje problema sa jednim znakom za Azure AD koji se pridružuje</span><span class="sxs-lookup"><span data-stu-id="94dcf-102">Troubleshoot Single-sign on for Azure AD Joined Devices</span></span>

<span data-ttu-id="94dcf-103">Ako imate lokalno okruženje aktivnog direktorijuma (AD) i želite da se pridružite OGLAŠAVANJU računara koji su se pridružili programu Azure AD, to možete da postignete tako što ćete postupiti na hibridnu Azure AD.</span><span class="sxs-lookup"><span data-stu-id="94dcf-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="94dcf-104">[Kako da: planirate hibridno Azure Active Directory pridruživanje](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) vam pruža srodne korake za primenu hibridnog AZURE oglašavanja u okruženju.</span><span class="sxs-lookup"><span data-stu-id="94dcf-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

<span data-ttu-id="94dcf-105">Više informacija potražite u članku [Konfigurisanje Azure AD za priključene uređaje za lokalno Single-Sign na korišćenje Windows Helo za preduzeća](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span><span class="sxs-lookup"><span data-stu-id="94dcf-105">For more information, see [Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span></span>

<span data-ttu-id="94dcf-106">**Problemi sa Token osvežavanja (PRT)**</span><span class="sxs-lookup"><span data-stu-id="94dcf-106">**Primary Refresh Token (PRT) issues**</span></span>

<span data-ttu-id="94dcf-107">Primarni Token osvežavanja (PRT) je ključni artefakt za Azure AD potvrda identiteta u operativnom sistemu Windows 10, Windows Server 2016 i novije verzije, iOS i Android uređajima.</span><span class="sxs-lookup"><span data-stu-id="94dcf-107">A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="94dcf-108">To je JSON Veb Token (JWT) naročito izdat Microsoft brokerima za potpisivanje simbola, kako bi omogućili jedinstveno prijavljivanje (SSO) u aplikacijama koje se koriste na tim uređajima.</span><span class="sxs-lookup"><span data-stu-id="94dcf-108">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="94dcf-109">Detalje o tome kako se PRT izdaje, koristi i štiti na Windows 10 uređajima potražite u članku [Šta je to simbol primarnog osvežavanja?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="94dcf-109">For details on how a PRT is issued, used, and protected on Windows 10 devices, see [What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="94dcf-110">**Vamdefaultsceno: da i AzureADPrt: da**</span><span class="sxs-lookup"><span data-stu-id="94dcf-110">**WamDefaultSet: YES and AzureADPrt: YES**</span></span>

<span data-ttu-id="94dcf-111">Ova polja ukazuju na to da li je korisnik uspešno potvrdio pristup Azure AD kada se prijavi na uređaj.</span><span class="sxs-lookup"><span data-stu-id="94dcf-111">These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="94dcf-112">Ako vrednosti **nisu, to** može da bude zbog:</span><span class="sxs-lookup"><span data-stu-id="94dcf-112">If the values are **NO**, it could be due to:</span></span>

- <span data-ttu-id="94dcf-113">Neispravan ključ skladišta u TPM-u koji je povezan sa uređajem po registraciji (Potvrdite prijavljivanje prilikom pokretanja povećanog)</span><span class="sxs-lookup"><span data-stu-id="94dcf-113">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)</span></span>
- <span data-ttu-id="94dcf-114">Alternativni ID prijavljivanja</span><span class="sxs-lookup"><span data-stu-id="94dcf-114">Alternate Login ID</span></span>
- <span data-ttu-id="94dcf-115">HTTP proxy nije pronađen</span><span class="sxs-lookup"><span data-stu-id="94dcf-115">HTTP Proxy not found</span></span>

<span data-ttu-id="94dcf-116">Da biste rešili probleme sa uređajima pomoću komande dsregcmd, pogledajte članak [SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span><span class="sxs-lookup"><span data-stu-id="94dcf-116">To troubleshoot devices using the dsregcmd command, see [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>
