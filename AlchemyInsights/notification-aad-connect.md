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
# <a name="notification-aad-connect"></a>Obaveštenje o povezivanju

- Uverite se da ste ovlašćeni da uradite operaciju. Globalni Administratori imaju Access po podrazumevanoj vrednosti. Pored toga, možete da koristite [kontrolu pristupa na osnovu uloge](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) za delegiranje dozvole za registraciju saradnikom.
- Uverite se da su neophodne krajnje tačke omogućene i da nisu blokirane zbog zaštitnog zida. Detalje potražite u članku [zahtevi](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Registracija može da ne uspe zbog toga što je odlazna komunikacija podvrgnuta SSL ispravci pomoću sloja mreže.
- Uverite se da ste potvrdili postavke obaveštenja za Azure AD Connect zdravstvo i Redigujte postavku. Da biste razumeli kako da konfigurišete postavke obaveštenja za Azure AD povežite zdravstvena obaveštenja, pogledajte ovaj [Vodič](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).
- Da biste saznali više o ispravnosti izveštaja AAD Connect za zdravlje i kako da ga preuzmete, pogledajte [izveštaj sinhronizacija nivoa objekata](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

Da biste rešili probleme sa AAD Connect zdravstvenim obaveštenjima, pogledajte [Vodič za rešavanje problema za AAD Connect obaveštenja o zdravstvenoj ispravnosti](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) i za najčešća pitanja pogledajte [najčešća pitanja za AAD Connect za zdravstvenu instalaciju](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).
