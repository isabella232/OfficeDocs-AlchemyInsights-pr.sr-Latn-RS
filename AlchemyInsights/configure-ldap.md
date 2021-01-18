---
title: Konfigurisanje LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885576"
---
# <a name="configure-ldap"></a><span data-ttu-id="d3cdb-102">Konfigurisanje LDAP</span><span class="sxs-lookup"><span data-stu-id="d3cdb-102">Configure LDAP</span></span>

<span data-ttu-id="d3cdb-103">Da biste konfigurisali LDAP, uradite sledeće:</span><span class="sxs-lookup"><span data-stu-id="d3cdb-103">To configure LDAP, do the following:</span></span>

1. <span data-ttu-id="d3cdb-104">Potvrdite zdravlje domena na lokaciji [Azure](https://aka.ms/aadds-health).</span><span class="sxs-lookup"><span data-stu-id="d3cdb-104">Check your domain’s health on the [Azure portal](https://aka.ms/aadds-health).</span></span>
1. <span data-ttu-id="d3cdb-105">Uverite se da je dostupna važeća Azure reklama za pretplatu i da su omogućene usluge Azure AD Domain.</span><span class="sxs-lookup"><span data-stu-id="d3cdb-105">Ensure a valid Azure AD subscription is available and Azure AD Domain Services has been enabled.</span></span>
1. <span data-ttu-id="d3cdb-106">Certifikat potreban za omogućavanje sigurnog LDAP-a mora biti dobijen od pouzdanog autoriteta za izdavanje certifikata ili biti samostalni certifikat.</span><span class="sxs-lookup"><span data-stu-id="d3cdb-106">The certificate required to enable secure LDAP must be obtained from a trusted public certification authority or be a self-signed certificate.</span></span>
1. <span data-ttu-id="d3cdb-107">Uverite se da certifikat prati obavezna [uputstva](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span><span class="sxs-lookup"><span data-stu-id="d3cdb-107">Ensure the certificate follows the required [guidelines](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span></span>

<span data-ttu-id="d3cdb-108">**Nevažeći certifikat**</span><span class="sxs-lookup"><span data-stu-id="d3cdb-108">**Invalid Certificate**</span></span>
1. <span data-ttu-id="d3cdb-109">Da biste obnovili certifikat, slijedite korake da biste kreirali novi certifikat i ponovo otpremili: [Konfiguriši LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="d3cdb-109">To renew a certificate, follow the steps to create a new certificate and reupload: [Configure LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
1. <span data-ttu-id="d3cdb-110">Da biste rešili poznati problem sa sigurnim LDAP obaveštenjima u usluzi Azure Active Directory Services, pogledajte članak [rešavanje LDAP upozorenja](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="d3cdb-110">To resolve known issue with Secure LDAP alerts in Azure Active directory Domain Services, see [Resolve LDAP alerts](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
