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
# <a name="problem-with-aad-connect-health"></a>Problem sa zdravim AAD Connect

- Uverite se da ste ovlašćeni da uradite operaciju. Globalni Administratori imaju Access po podrazumevanoj vrednosti. Pored toga, možete da koristite [kontrolu pristupa na osnovu uloge](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) za delegiranje dozvole za registraciju saradnikom.
- Uverite se da su neophodne krajnje tačke omogućene i da nisu blokirane zbog zaštitnog zida. Detalje potražite u članku [zahtevi](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Registracija može da ne uspe zbog toga što je odlazna komunikacija podvrgnuta SSL ispravci pomoću sloja mreže.
- Uverite se da ste potvrdili postavke obaveštenja za Azure AD Connect zdravstvo. Pregledajte postavku. Ovaj [Vodič](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) vam može pomoći da shvatite kako da konfigurišete postavke obaveštenja za AZURE AD povežite zdravstvena obaveštenja.
- Da biste saznali više o ispravnosti izveštaja AAD Connect za zdravlje i kako da ga preuzmete, pogledajte [izveštaj sinhronizacija nivoa objekata](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

Da biste rešili probleme sa AAD Connect zdravstvenim obaveštenjima, pogledajte [Vodič za rešavanje problema da biste imali obaveštenja o obaveštenjima o zdravstvenoj ispravnosti](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) i za najčešća pitanja pogledajte [najčešća pitanja o programu AAD Connect za zdravstvenu instalaciju](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).
