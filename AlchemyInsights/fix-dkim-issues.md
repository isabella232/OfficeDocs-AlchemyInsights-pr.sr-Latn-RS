---
title: Rešavanje problema sa podešavanjem DKIM-a
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 5a613321ed79e657350ec4d19b1f07ac0a091b227a8268c793a10edd9990d41f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945945"
---
# <a name="fix-dkim-setup-issues"></a>Rešavanje problema sa podešavanjem DKIM-a

Ako naiđu na probleme sa omogućavanjem DKIM-a za prilagođeni domen, koristite sledeće korake:

- Većina problema sa podešavanjem DKIM-a povezana je sa neispravnim DNS zapisima. Potvrdite da je DKIM CNAME **zapis** ( a ne TXT zapis) ispravno oblikovan. Dodatne informacije potražite u ovoj [temi.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

- Kada napravite ili ažurirate DKIM DNS zapise u usluzi DNS hostinga za domen (obično je to registar domena), sačekajte da se DNS zapisi prenesu.

- Ako ne možete da kreirate DKIM DNS zapise u centru aktivnosti, možete da zamenite prilagođenim domenom (na primer, contoso.com) i da pokrenete ovu komandu u programu \<CustomDomain\> [Exchange Online PowerShell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
