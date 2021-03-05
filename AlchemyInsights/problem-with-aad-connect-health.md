---
title: Problem sa zdravim AAD Connect
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
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/04/2021
ms.locfileid: "50483118"
---
# <a name="problem-with-aad-connect-health"></a><span data-ttu-id="fde54-102">Problem sa zdravim AAD Connect</span><span class="sxs-lookup"><span data-stu-id="fde54-102">Problem with AAD Connect Health</span></span>

- <span data-ttu-id="fde54-103">Uverite se da ste ovlašćeni da uradite operaciju.</span><span class="sxs-lookup"><span data-stu-id="fde54-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="fde54-104">Globalni Administratori imaju Access po podrazumevanoj vrednosti.</span><span class="sxs-lookup"><span data-stu-id="fde54-104">Global Admins have access by default.</span></span> <span data-ttu-id="fde54-105">Pored toga, možete da koristite [kontrolu pristupa na osnovu uloge](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) za delegiranje dozvole za registraciju saradnikom.</span><span class="sxs-lookup"><span data-stu-id="fde54-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="fde54-106">Uverite se da su neophodne krajnje tačke omogućene i da nisu blokirane zbog zaštitnog zida.</span><span class="sxs-lookup"><span data-stu-id="fde54-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="fde54-107">Detalje potražite u članku [zahtevi](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span><span class="sxs-lookup"><span data-stu-id="fde54-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="fde54-108">Registracija može da ne uspe zbog toga što je odlazna komunikacija podvrgnuta SSL ispravci pomoću sloja mreže.</span><span class="sxs-lookup"><span data-stu-id="fde54-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="fde54-109">Uverite se da ste potvrdili postavke obaveštenja za Azure AD Connect zdravstvo.</span><span class="sxs-lookup"><span data-stu-id="fde54-109">Make sure you have verified the notification settings for Azure AD Connect Health.</span></span> <span data-ttu-id="fde54-110">Pregledajte postavku.</span><span class="sxs-lookup"><span data-stu-id="fde54-110">Please review your setting.</span></span> <span data-ttu-id="fde54-111">Ovaj [Vodič](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) vam može pomoći da shvatite kako da konfigurišete postavke obaveštenja za AZURE AD povežite zdravstvena obaveštenja.</span><span class="sxs-lookup"><span data-stu-id="fde54-111">This [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) can help you understand how to configure the notification settings for Azure AD Connect health notifications.</span></span>
- <span data-ttu-id="fde54-112">Da biste saznali više o ispravnosti izveštaja AAD Connect za zdravlje i kako da ga preuzmete, pogledajte [izveštaj sinhronizacija nivoa objekata](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span><span class="sxs-lookup"><span data-stu-id="fde54-112">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="fde54-113">Da biste rešili probleme sa AAD Connect zdravstvenim obaveštenjima, pogledajte [Vodič za rešavanje problema da biste imali obaveštenja o obaveštenjima o zdravstvenoj ispravnosti](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) i za najčešća pitanja pogledajte [najčešća pitanja o programu AAD Connect za zdravstvenu instalaciju](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span><span class="sxs-lookup"><span data-stu-id="fde54-113">To troubleshoot AAD Connect Health alerts, follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
