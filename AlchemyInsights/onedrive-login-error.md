---
title: Greška u OneDrive prijavljivanju AADSTS50011
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982544"
---
# <a name="onedrive-login-error-aadsts50011"></a><span data-ttu-id="d87ef-102">Greška u OneDrive prijavljivanju AADSTS50011</span><span class="sxs-lookup"><span data-stu-id="d87ef-102">OneDrive login error AADSTS50011</span></span>

<span data-ttu-id="d87ef-103">Ako primite grešku "AADSTS50011: URL adresa odgovora navedena u zahtevu se ne podudara sa odgovorom" kada se prijavite u OneDrive aplikaciji, potražite sledeće:</span><span class="sxs-lookup"><span data-stu-id="d87ef-103">If you receive an error "AADSTS50011: The reply URL specified in the request does not match the reply" when signing into the OneDrive app, check for the following:</span></span>

<span data-ttu-id="d87ef-104">Vaša OneDrive verzija treba da bude jednaka ili veća od verzije 20.052. XXXX. XXXX.</span><span class="sxs-lookup"><span data-stu-id="d87ef-104">Your OneDrive version needs to be equal to or greater than version 20.052.XXXX.XXXX.</span></span> <span data-ttu-id="d87ef-105">Da biste provjerili verziju, kliknite na ikonu Blue OneDrive na sistemskoj traci poslova, izaberite stavku **pomoć & postavkama > postavkama >**.</span><span class="sxs-lookup"><span data-stu-id="d87ef-105">To check your version, click on the blue OneDrive icon in the notification area, select **Help & Settings > Settings > About**.</span></span>

<span data-ttu-id="d87ef-106">Vaša mreža blokira saobraćaj na **g.live.com** i **oneclient.sfx.MS**.</span><span class="sxs-lookup"><span data-stu-id="d87ef-106">Your network might block traffic to **g.live.com** and **oneclient.sfx.ms**.</span></span> <span data-ttu-id="d87ef-107">Ako je taj saobraćaj blokiran, OneDrive ne može sama da se ažurira.</span><span class="sxs-lookup"><span data-stu-id="d87ef-107">If that traffic is blocked, OneDrive cannot update itself.</span></span> <span data-ttu-id="d87ef-108">Radite sa administratorom mreže da biste se uverili da imate pristup tim URL adresama.</span><span class="sxs-lookup"><span data-stu-id="d87ef-108">Work with your network administrator to ensure you have access to those URLs.</span></span> <span data-ttu-id="d87ef-109">[Ove krajnje tačke](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) treba da se pristupačnu za klijente pomoću Microsoft 365 planova.</span><span class="sxs-lookup"><span data-stu-id="d87ef-109">[These endpoints](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) should be reachable for customers using Microsoft 365 plans.</span></span>

<span data-ttu-id="d87ef-110">Ako treba da ručno nabavite trenutnu verziju usluge OneDrive, posetite [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .</span><span class="sxs-lookup"><span data-stu-id="d87ef-110">If you need to manually get a current version of OneDrive, visit [https://aka.ms/getonedrive](https://aka.ms/getonedrive).</span></span>
