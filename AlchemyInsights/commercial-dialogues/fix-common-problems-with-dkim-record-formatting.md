---
title: Rešavanje uobičajenih problema sa DKIM oblikovanjem zapisa
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: e55175e7613d220eaf956d3c7fd02213dcd5803d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324004"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Rešavanje uobičajenih problema sa DKIM oblikovanjem zapisa

Većina problema sa podešavanjem DKIM-a povezana je sa neispravnim DNS zapisima.

Da biste rešili probleme sa podešavanjem DKIM-a, proverite da li je DKIM CNAME zapis ( a ne TXT zapis) ispravno oblikovan. Dodatne informacije potražite u [temi Šta treba da uradite da biste ručno podesili DKIM u programu Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)

Ako vam je uopšteno potrebna pomoć sa DNS zapisima, pogledajte kreiranje DNS zapisa kod bilo kog [dobavljača usluga DNS hostinga za Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

**Na umu:** Kada napravite ili ažurirate DKIM DNS zapise u usluzi DNS hostinga za domen, trebalo bi da sačekate da se DNS zapisi prenesu.
