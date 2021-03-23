---
title: Obaveštenje o povezivanju
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
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037238"
---
# <a name="notification-aad-connect"></a><span data-ttu-id="190bb-102">Obaveštenje o povezivanju</span><span class="sxs-lookup"><span data-stu-id="190bb-102">Notification AAD Connect</span></span>

- <span data-ttu-id="190bb-103">Uverite se da ste ovlašćeni da uradite operaciju.</span><span class="sxs-lookup"><span data-stu-id="190bb-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="190bb-104">Globalni Administratori imaju Access po podrazumevanoj vrednosti.</span><span class="sxs-lookup"><span data-stu-id="190bb-104">Global Admins have access by default.</span></span> <span data-ttu-id="190bb-105">Pored toga, možete da koristite [kontrolu pristupa na osnovu uloge](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) za delegiranje dozvole za registraciju saradnikom.</span><span class="sxs-lookup"><span data-stu-id="190bb-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="190bb-106">Uverite se da su neophodne krajnje tačke omogućene i da nisu blokirane zbog zaštitnog zida.</span><span class="sxs-lookup"><span data-stu-id="190bb-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="190bb-107">Detalje potražite u članku [zahtevi](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span><span class="sxs-lookup"><span data-stu-id="190bb-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="190bb-108">Registracija može da ne uspe zbog toga što je odlazna komunikacija podvrgnuta SSL ispravci pomoću sloja mreže.</span><span class="sxs-lookup"><span data-stu-id="190bb-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="190bb-109">Uverite se da ste potvrdili postavke obaveštenja za Azure AD Connect zdravstvo i Redigujte postavku.</span><span class="sxs-lookup"><span data-stu-id="190bb-109">Make sure you have verified the notification settings for Azure AD Connect Health and review your setting.</span></span> <span data-ttu-id="190bb-110">Da biste razumeli kako da konfigurišete postavke obaveštenja za Azure AD povežite zdravstvena obaveštenja, pogledajte ovaj [Vodič](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span><span class="sxs-lookup"><span data-stu-id="190bb-110">To understand how to configure the notification settings for Azure AD Connect Health notifications, see this [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span></span>
- <span data-ttu-id="190bb-111">Da biste saznali više o ispravnosti izveštaja AAD Connect za zdravlje i kako da ga preuzmete, pogledajte [izveštaj sinhronizacija nivoa objekata](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span><span class="sxs-lookup"><span data-stu-id="190bb-111">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="190bb-112">Da biste rešili probleme sa AAD Connect zdravstvenim obaveštenjima, pogledajte [Vodič za rešavanje problema za AAD Connect obaveštenja o zdravstvenoj ispravnosti](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) i za najčešća pitanja pogledajte [najčešća pitanja za AAD Connect za zdravstvenu instalaciju](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span><span class="sxs-lookup"><span data-stu-id="190bb-112">To troubleshoot AAD Connect Health Alerts follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
