---
title: Popravka postavki smernica za korisnike/poštansko sanduče
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/09/2021
ms.locfileid: "50695903"
---
# <a name="fix-user-policymailbox-settings"></a>Popravka postavki smernica za korisnike/poštansko sanduče

Postavke neželjene pošte u poštanskom sandučetu utiču na ovu poruku. Da biste pregledali postavke, uradite sledeće:

1. Pokrenite Exchange Management Shell. Više informacija potražite u članku [Otvaranje programskog dodatka Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).
2. Pokrene ovu komandu (pomoću e-adrese korisnika):  **uzmi-mailboxconfiguration mail Configuration-identitet "User@domain.com"**
3. Potvrdite da li je adresa e-pošte pošiljaoca deo **poverendindersandždodomena** ili **blokiranih domena**. Ako se e-adresa nalazi na jednoj od listi, možda ćete morati da je uklonite. Da biste saznali više, pogledajte članak [Podešavanje konfiguracije-Mailboxjunkemailsanduče](https://go.microsoft.com/fwlink/?linkid=2101047).
