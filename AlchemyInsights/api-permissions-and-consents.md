---
title: Dozvole za API i pristanak
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974992"
---
# <a name="api-permissions-and-consent"></a>Dozvole za API i pristanak

Aplikacije koje se integrišu sa Microsoft platformom za identifikaciju slede model identiteta koji korisnicima i administratori pružaju kontrolu nad načinom na koji se podaci mogu pristupiti. Primena modela autorizacije ažurirana je na krajnjoj tački Microsoft platforme identiteta. Menja kako aplikacija mora da komunicira sa Microsoft platformom identiteta. [Dozvole i pristanak u krajnjoj tački Microsoft platforme identiteta](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) pokrivaju osnovne koncepte ovog modela autorizacije, uključujući opsege, dozvole i saglasnost.

Okvir za pristup [Azure Active Directory (AZURE AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) olakšava razvijanje Veb lokacija multi-zakupaca i izvornih klijentskih aplikacija. Ove aplikacije mogu da se prijave po korisničkim nalozima od Azure AD zakupca koji se razlikuje od onog u kom se registruje aplikacija. Možda će biti potrebno da pristupe i vebu Veb Appsu, kao što je Microsoft Graph API (za pristup Azure AD, Intune i uslugama u programu Microsoft 365) i drugim AFIS uslugama Microsoft Services, pored sopstvenog Veb APIs.

