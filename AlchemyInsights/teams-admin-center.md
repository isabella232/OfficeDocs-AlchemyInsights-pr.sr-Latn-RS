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
ms.openlocfilehash: 29e54e0f8255b4ce84c433f2cc827aaedf35327626f0095788faef802763bc53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049358"
---
# <a name="teams-admin-center"></a>Teams centar administracije

Saznajte više o upravljanju uslugom Teams uz[Teams centar administracije](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Ako ne možete da pristupite Teams centru administracije, proverite sledeće stavke:

- Uverite se da ste omogućili odgovarajuće [Office 365 IP adrese i URL adrese ](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service)na bilo kom uređaju (zaštitnom zidu itd.) ili u okviru pravila zaštitnog zida na lokalnom računaru.
- Proverite da li se prijavljivanje koje koristite za pristup Teams portalu za administraciju podudara sa vašim korisničkim imenom navedeno na [Microsoft 365 portalu za administraciju](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Ako se korisnici ne pojavljuju u Teams centru administracije, proverite sledeće:

- Da li ste kreirali korisnike ili dodeljivali licence u protekla 24 časa? Uverite se da ste sačekali najmanje 24 časa pre otvaranja tiketa za podršku.
- Proverite da li ste dodelili odgovarajuće licence?
- Ako imate lokalnu uslugu Active Directory, proverite da li je vrednost [msRTCSIP-PrimaryUserAddress](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) ili SIP adrese u polju ProxyAddresses u lokalnoj uslugi Active Directory jedinstvena, a format se podudara sa sip: Korisničko ime korisnika sa lokacije [Microsoft 365 centar administracije.](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)
- Ako nameravate da zadržite primenu usluge Skype za posao Server i imate korisnike koji koriste kućnu primenu i na mreži: pratite "Podešavanje **hibrida** sa uslugama Teams i Skype za posao Na mreži" na Skype za posao Server kontrolnoj tabli i premestite korisnike na mrežu.
