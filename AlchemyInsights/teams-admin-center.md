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
# <a name="teams-admin-center"></a>Teams centar administracije

Saznajte više o upravljanju uslugom Teams uz[Teams centar administracije](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Ako ne možete da pristupite Teams centru administracije, proverite sledeće stavke:

- Uverite se da ste omogućili odgovarajuće [Office 365 IP adrese i URL adrese ](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service)na bilo kom uređaju (zaštitnom zidu itd.) ili u okviru pravila zaštitnog zida na lokalnom računaru.
- Proverite da li se prijavljivanje koje koristite za pristup Teams portalu za administraciju podudara sa vašim korisničkim imenom navedeno na [Microsoft 365 portalu za administraciju](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Ako se korisnici ne pojavljuju u Teams centru administracije, proverite sledeće:

- Da li ste kreirali korisnike ili dodeljivali licence u protekla 24 časa? Uverite se da ste sačekali najmanje 24 časa pre otvaranja tiketa za podršku.
- Proverite da li ste dodelili odgovarajuće licence?
- Ako imate lokalnu uslugu Active Directory, proverite da li je vrednost [msRTCSIP-PrimaryUserAddress](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) ili SIP adrese u polju ProxyAddresses u lokalnoj sistemu Active Directory jedinstvena, a format se podudara sa sip: Korisničko ime korisnika iz [Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)centra za adminitre.
- Ako nameravate da zadržite primenu sistema Skype za posao Server i imate korisnike koji koriste kućnu primenu i na mreži: pratite **"Podešavanje hibridne** primene sa uslugama Teams i Skype za posao Online" na kontrolnoj tabli sistema Skype za posao Server i premestite korisnike na mrežu.
