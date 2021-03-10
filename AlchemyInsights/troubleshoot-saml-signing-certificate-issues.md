---
title: Rešavanje problema sa certifikatom za SAML potpisivanje
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694448"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a>Rešavanje problema sa certifikatom za SAML potpisivanje

Da biste rešili problem sa certifikatom za SEML, obavite sledeće preporučene korake:

1. Kada dodate poslovnu aplikaciju koja podržava SSO, Azure će generisati certifikat koji se zove " [certifikat potpisa Sema](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications)". Ovaj certifikat ima datum isteka 3 godine. Da biste promenili datum isteka certifikata, pogledajte članak [Prilagođavanje datuma isteka za certifikat Federacije i vraćanje na novi certifikat](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).
2. Azure će koristiti ovaj certifikat za potpisivanje SAML Toksa koje je aplikacija zatražila i šalje ga aplikaciji za uspešan SSO. Da biste ovo dovršili, preuzmite certifikat sa Azure portala i pošaljite ga prodavcu aplikacije da biste dovršili SSO proces.

Pošto ovaj proces dovrši aplikaciju vjeruje ovaj certifikat i svi željeni simboli koje potpiše ovaj certifikat primiće aplikacija.

3. Ako ovaj certifikat istekne, kreirajte novi certifikat, ažurirajte ga na prodavca aplikacije, a zatim ga učinite aktivnim na stranici Azure. Više informacija potražite u članku obnova [certifikata koji će uskoro isteći](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).

> [!NOTE]
> Ako certifikat istekne, korisnik neće biti blokiran.

4. [Dodajte e-adresu za obaveštenja](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) koja će biti primljena pre isteka trenutnog certifikata.

> [!NOTE]
> Korak-4 je opcionalan.

5. Promenite opcije za potpisivanje certifikata za SEML certifikat i algoritam za potpisivanje certifikata. Više informacija potražite u članku [Promena opcija potpisivanja certifikata i potpisivanja algoritma](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).

