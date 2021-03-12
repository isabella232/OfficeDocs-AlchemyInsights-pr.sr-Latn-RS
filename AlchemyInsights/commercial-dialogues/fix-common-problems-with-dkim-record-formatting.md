---
title: Rešavanje uobičajenih problema sa oblikovanjem DKIM zapisa
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
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750758"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Rešavanje uobičajenih problema sa oblikovanjem DKIM zapisa

Većina DKIM podešavanje problema je povezana sa netačnim DNS zapisima.

Da biste rešili probleme sa podešenjem za DKIM, uverite se da je DKIM CNAME zapis (**nije** txt zapis) ispravno oblikovan. Više informacija potražite u članku [Šta treba da uradite da biste ručno podesili DKIM u sistemu Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).

Ako vam je potrebna pomoć sa DNS zapisima, pogledajte članak [Kreiranje DNS zapisa kod bilo kog dobavljača usluga DNS hostinga za Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).

> [!NOTE]
> Kada kreirate ili ažurirate DKIM DNS zapise u usluzi DNS hostinga za domen, moraćete da sačekate da se DNS zapisi umnože.
