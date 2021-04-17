---
title: Teams centar administracije
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: 4a3a0796cedd81919066d870c5ca99fe2e978cf8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826393"
---
# <a name="teams-admin-center"></a><span data-ttu-id="7a7ad-102">Teams centar administracije</span><span class="sxs-lookup"><span data-stu-id="7a7ad-102">Teams Admin Center</span></span>

<span data-ttu-id="7a7ad-103">Saznajte više o upravljanju uslugom Teams uz[Teams centar administracije](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span><span class="sxs-lookup"><span data-stu-id="7a7ad-103">Learn about managing Teams with the [Teams Admin Center](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span></span>

<span data-ttu-id="7a7ad-104">Ako ne možete da pristupite Teams centru administracije, proverite sledeće stavke:</span><span class="sxs-lookup"><span data-stu-id="7a7ad-104">If you are unable to access the Teams Admin Center, please check the following items:</span></span>

- <span data-ttu-id="7a7ad-105">Uverite se da ste omogućili odgovarajuće [Office 365 IP adrese i URL adrese ](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service)na bilo kom uređaju (zaštitnom zidu itd.) ili u okviru pravila zaštitnog zida na lokalnom računaru.</span><span class="sxs-lookup"><span data-stu-id="7a7ad-105">Verify that you have allowed the appropriate [Office 365 IP addresses and URL's](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) on any perimeter devices (firewall, etc.) or in the firewall rules on your local machine.</span></span>
- <span data-ttu-id="7a7ad-106">Proverite da li se prijavljivanje koje koristite za pristup Teams portalu za administraciju podudara sa vašim korisničkim imenom navedeno na [Microsoft 365 portalu za administraciju](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="7a7ad-106">Verify that the login you are using to access the Teams Admin Portal matches your username listed in the [Microsoft 365 Admin portal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>

<span data-ttu-id="7a7ad-107">Ako se korisnici ne pojavljuju u Teams centru administracije, proverite sledeće:</span><span class="sxs-lookup"><span data-stu-id="7a7ad-107">If users are not appearing in the Teams Admin Center, please check the following:</span></span>

- <span data-ttu-id="7a7ad-108">Da li ste kreirali korisnike ili dodeljivali licence u protekla 24 časa?</span><span class="sxs-lookup"><span data-stu-id="7a7ad-108">Have you created users or assigned licenses in the last 24 hours?</span></span> <span data-ttu-id="7a7ad-109">Uverite se da ste sačekali najmanje 24 časa pre otvaranja tiketa za podršku.</span><span class="sxs-lookup"><span data-stu-id="7a7ad-109">Please make sure you wait at least 24 hours before opening a support ticket.</span></span>
- <span data-ttu-id="7a7ad-110">Proverite da li ste dodelili odgovarajuće licence?</span><span class="sxs-lookup"><span data-stu-id="7a7ad-110">Verify you have assigned appropriate licenses?</span></span>
- <span data-ttu-id="7a7ad-111">Ako imate lokalnu uslugu Active Directory, proverite da li je vrednost [msRTCSIP-PrimaryUserAddress](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) ili SIP adrese u polju ProxyAddresses u lokalnoj sistemu Active Directory jedinstvena, a format se podudara sa sip: Korisničko ime korisnika iz [Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)centra za adminitre.</span><span class="sxs-lookup"><span data-stu-id="7a7ad-111">If you have an on-premise Active Directory, verify that [the value of msRTCSIP-PrimaryUserAddress or the SIP address in the ProxyAddresses field in your local Active Directory is unique and the format matches](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Username** of the user from the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>
- <span data-ttu-id="7a7ad-112">Ako nameravate da zadržite primenu sistema Skype za posao Server i imate korisnike koji koriste kućnu primenu i na mreži: pratite **"Podešavanje hibridne** primene sa uslugama Teams i Skype za posao Online" na kontrolnoj tabli sistema Skype za posao Server i premestite korisnike na mrežu.</span><span class="sxs-lookup"><span data-stu-id="7a7ad-112">If you intend to keep a Skype for Business Server deployment and have users homed on-premises and Online: follow the **"Set up hybrid with Teams and Skype for Business Online"** in your Skype for Business Server Control Panel and move users Online.</span></span>
