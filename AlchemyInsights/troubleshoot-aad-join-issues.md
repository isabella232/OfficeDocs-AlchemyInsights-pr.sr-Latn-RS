---
title: Rešavanje problema sa Azure AD pridruživanjem
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
- "9003246"
- "6157"
ms.openlocfilehash: 8e902aea30e6891717e08027cc009576d390c9cf2ba1649cbbc68d64883937f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939933"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Rešavanje problema sa Azure AD pridruživanjem

1. Ako po prvi put postavljate registracije uređaja, proverite da li ste pregledali Uvod u upravljanje uređajima u programu [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) koji će vas voditi kroz to kako da podvučete uređaje pod kontrolu za Azure AD. 
1. Ako direktno registrujete uređaje u uslugu Azure AD i upisujete ih u [Intune,](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) morate [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) da se uverite da ste konfigurisali Intune i da prvo imate licenciranje na mestu.
1. Uverite se da ste ovlašćeni za izvršavanje operacija u Azure AD. Postavkama za registracije uređaja može da upravlja samo globalni administrator u usluzi Azure AD.
1. Da biste primenu Azure AD pridruživanja primenili, pogledajte [plan Azure AD Join.](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan)

Više detalja o rešavanju uobičajenih problema sa Azure AD pridruživanjem možete da vidite u članku Najčešća pitanja za [Azure Ad Join](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) i za Windows 10 pro uređaj pogledajte Članak Nije moguće pridružiti [Windows 10 Pro računaru Azure AD](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900) – treba da izvršite nadogradnju na – Microsoft Community
