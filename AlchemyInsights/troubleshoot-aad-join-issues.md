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
ms.openlocfilehash: 0e9f7c95cf522340e9976f668c1d1a9eaff71910
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405759"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Rešavanje problema sa Azure AD pridruživanjem

1. Ako po prvi put postavljate registracije uređaja, proverite da li ste pregledali Uvod u upravljanje uređajima u [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) koji će vas voditi kroz to kako da nabavite uređaje pod kontrolom za Azure AD. 
1. Ako direktno registrujete uređaje u uslugu Azure AD i upisujete ih u [Intune,](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) morate [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) da se uverite da ste konfigurisali Intune i da prvo imate licenciranje na mestu.
1. Uverite se da ste ovlašćeni za izvršavanje operacija u Azure AD. Samo globalni administrator u Azure AD-u može da upravlja postavkama za registracije uređaja.
1. Da biste primenu Azure AD pridruživanja primenili, pogledajte [plan Azure AD Join.](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan)

Za više detalja o rešavanju uobičajenih problema sa Azure AD pridruživanjem pogledajte najčešća pitanja o [Azure Ad Join](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) i za Windows 10 Pro uređaj, pogledajte članak Nije moguće pridružiti Windows 10 Pro računarU [Azure AD –](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900) treba da izvršite nadogradnju na Microsoft zajednicu
