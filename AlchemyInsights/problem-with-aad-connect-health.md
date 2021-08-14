---
title: Problem sa AAD Povezivanje Health
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
ms.openlocfilehash: 82cfcc6132549b52278b174fce3173f5566268864a207882a4dd639cb8024ee3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923766"
---
# <a name="problem-with-aad-connect-health"></a>Problem sa AAD Povezivanje Health

- Uverite se da ste ovlašćeni za izvršavanje operacije. Globalni dobavljači podrazumevano imaju pristup. Pored toga, možete da koristite kontrolu pristupa [na osnovu uloga](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) da biste delegirao dozvolu za registraciju saradniku.
- Uverite se da su potrebne krajnje tačke omogućene, a ne blokirane zbog zaštitnog zida. Za više detalja pogledajte [zahteve](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Registracija može da ne uspe jer odlazna komunikacija podleže SSL pregledu od strane mrežnog sloja.
- Proverite da li ste potvrdili postavke obaveštenja za Azure AD Povezivanje Health. Pregledajte postavku. Ovaj [vodič](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) može da vam pomogne da razumete kako da konfigurišete postavke obaveštenja za Azure AD Povezivanje obaveštenja o ispravnosti.
- Da biste saznali više o AAD Povezivanje Health izveštaju sinhronizacije i o tome kako da ga preuzmete, pogledajte izveštaj sinhronizacije na nivou [objekta.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

Da biste rešili probleme sa AAD Povezivanje Health upozorenjima, pratite vodič za rešavanje problema za [AAD Povezivanje Obaveštenja](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) o svežini podataka o zdravlju i za najčešća pitanja pogledajte Uobičajena pitanja o [AAD Povezivanje Health](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)instalaciji.
