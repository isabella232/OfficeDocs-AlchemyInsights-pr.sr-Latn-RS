---
title: API dozvole i saglasnost
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
ms.openlocfilehash: c45bab67d414c8f0f2ca1c5275084d4ecce538c5256154292302080ba5bd8175
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932111"
---
# <a name="api-permissions-and-consent"></a>API dozvole i saglasnost

Aplikacije koje se integrišu sa Microsoft platforma za identitete prate model autorizacije koji korisnicima i administratorima omogućava da kontrolišu način pristupa podacima. Primena modela autorizacije ažurirana je na krajnjim tačkama Microsoft platforma za identitete autorizacija. Ona menja način na koji aplikacija mora da vrši interakciju sa Microsoft platforma za identitete. [Dozvole i pristanak](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) u Microsoft platforma za identitete krajnje tačke pokrivaju osnovne koncepte ovog modela autorizacije, uključujući prorede, dozvole i saglasnost.

Novi [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) okvir za pristanak olakšava razvijanje veb aplikacija sa više zakupca i njegovih nativnih klijenta. Ove aplikacije dozvoljavaju prijavljivanje po korisničkim nalozima Azure AD zakupca koji se razlikuju od aplikacije u kojoj je aplikacija registrovana. Oni će možda morati da pristupe i veb API-ju kao što je Microsoft Graph API (da bi pristupili uslugama Azure AD, Intune i uslugama u sistemu Microsoft 365) i drugim API Microsoft usluge korporaciji Microsoft usluge, pored svojih veb API-ja.

