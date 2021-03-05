---
title: Konfigurisanje MIM usluge sinhronizacije
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482899"
---
# <a name="configure-mim-sync-service"></a>Konfigurisanje MIM usluge sinhronizacije

Usluga sinhronizacije Microsoft identiteta menadžera (MIM) je komponenta MIM. To je centralizovana lokalno usluga koja skladišti i integriše informacije za organizacije koje imaju više direktorijumi i baze podataka. Možda ćete moći da rešite problem sa MIM sinhronizacijom ako je problem bio adresiran na MIM ili je jedan od drugih problema pomenutih u donjem odeljku.

**Preporučeni koraci**

1. Uverite se da koristite nedavnu ispravku MIM sinhronizacije i proverite beleške sa izdanjima [Mim Sync](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) da biste utvrdili da li je problem rešen u ispravci.
2. Ako je problem sa sistemom generičkih LDAP, generičkog SQL, Lotus Domino ili Veb Services konektora, uverite se da koristite nedavnu ispravku [generičkih konektora](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).
3. Ako neki MIM Sync – pokretanje prekine sa greškom, obratite se tabeli sa [kodom greške](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) da biste utvrdili potencijalne uzroke.
4. Ako se zaustavljanje zaustavi sa **izuzetkom za proširenje DLL**-a, zatim kliknite na te reči da biste otvorili prozor **Svojstva objekta prostora spajanja** i kliknite na dugme **prati praćenje steka...** da biste videli više informacija o osnovnom cilju, kao što je opisano u programu " [produћetak](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx)podataka".
5. Ako datoteka usluge obaveštavanja lozinkom (PCNS) izveštava **o grešci 6025** u evidenciji događaja tokom sinhronizacije lozinke, potvrdite izbor u polju za rešavanje problema sa funkcijom [pcns za izveštavanje 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).
6. Ako je potpuna Sinhronizacija sa agentom za upravljanje uslugama FIM spora, potvrdite izbor u polju za proveru **automatski** , kao što je opisano u [rešavanju problema spora ili viseće cele sinhronizacije](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).
7. Ako se nalazite u grešci sa sprečenjem zaustavljanja servera sa neuspešnim kreiranjem-putem-veb-uslugama pomoću usluge Management AG za upravljanje uslugama, pogledajte članak [Podrška-Info: neuspešno kreiranje-putem-Veb-usluge](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) za pregled uzroka.

