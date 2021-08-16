---
title: Popravljanje smernica korisnika/postavki poštanskog sandučeta
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
ms.openlocfilehash: fecc52bea66e0aed709a8995d2509f4432c09482459aa575d29e4c7551375211
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034732"
---
# <a name="fix-user-policymailbox-settings"></a>Popravljanje smernica korisnika/postavki poštanskog sandučeta

Postavke neželjene pošte u poštanskom sandučetu uticale su na ovu poruku. Da biste pregledali postavke, uradite sledeće:

1. Pokrenite Exchange Management Shell. Dodatne informacije potražite u [Exchange Upravljanje programom .](https://go.microsoft.com/fwlink/?linkid=2101432)
2. Pokrenite ovu komandu (pomoću adrese e-pošte korisnika):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. Proverite da li je e-adresa pošiljaoca deo **TrustedSendersAndDomains** ili **BlockedSendersAndDomains**. Ako je e-adresa na jednoj od lista, možda ćete morati da je uklonite. Da biste saznali više, [pogledajte temu Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).
