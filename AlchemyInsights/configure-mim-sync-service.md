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
# <a name="configure-mim-sync-service"></a><span data-ttu-id="473f7-102">Konfigurisanje MIM usluge sinhronizacije</span><span class="sxs-lookup"><span data-stu-id="473f7-102">Configure MIM Sync service</span></span>

<span data-ttu-id="473f7-103">Usluga sinhronizacije Microsoft identiteta menadžera (MIM) je komponenta MIM.</span><span class="sxs-lookup"><span data-stu-id="473f7-103">Microsoft Identity Manager (MIM) Synchronization Service is a component of MIM.</span></span> <span data-ttu-id="473f7-104">To je centralizovana lokalno usluga koja skladišti i integriše informacije za organizacije koje imaju više direktorijumi i baze podataka.</span><span class="sxs-lookup"><span data-stu-id="473f7-104">It is a centralized on-premises service that stores and integrates information for organizations that have multiple on-premises directories and databases.</span></span> <span data-ttu-id="473f7-105">Možda ćete moći da rešite problem sa MIM sinhronizacijom ako je problem bio adresiran na MIM ili je jedan od drugih problema pomenutih u donjem odeljku.</span><span class="sxs-lookup"><span data-stu-id="473f7-105">You may be able to resolve your problem with MIM Sync if the issue was addressed in a recent update to MIM or is one of the other issues mentioned in the below section.</span></span>

<span data-ttu-id="473f7-106">**Preporučeni koraci**</span><span class="sxs-lookup"><span data-stu-id="473f7-106">**Recommended steps**</span></span>

1. <span data-ttu-id="473f7-107">Uverite se da koristite nedavnu ispravku MIM sinhronizacije i proverite beleške sa izdanjima [Mim Sync](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) da biste utvrdili da li je problem rešen u ispravci.</span><span class="sxs-lookup"><span data-stu-id="473f7-107">Ensure that you are using a recent update of MIM Sync and check the [MIM Sync release notes](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) to determine if the issue has been resolved in an update.</span></span>
2. <span data-ttu-id="473f7-108">Ako je problem sa sistemom generičkih LDAP, generičkog SQL, Lotus Domino ili Veb Services konektora, uverite se da koristite nedavnu ispravku [generičkih konektora](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).</span><span class="sxs-lookup"><span data-stu-id="473f7-108">If the problem is with the Generic LDAP, Generic SQL, Lotus Domino or Web Services connector, ensure that you are using a recent update of the [generic connectors](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).</span></span>
3. <span data-ttu-id="473f7-109">Ako neki MIM Sync – pokretanje prekine sa greškom, obratite se tabeli sa [kodom greške](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) da biste utvrdili potencijalne uzroke.</span><span class="sxs-lookup"><span data-stu-id="473f7-109">If an MIM Sync-run stops with an error, consult the table of [run error codes](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) to determine the potential causes.</span></span>
4. <span data-ttu-id="473f7-110">Ako se zaustavljanje zaustavi sa **izuzetkom za proširenje DLL**-a, zatim kliknite na te reči da biste otvorili prozor **Svojstva objekta prostora spajanja** i kliknite na dugme **prati praćenje steka...** da biste videli više informacija o osnovnom cilju, kao što je opisano u programu " [produћetak](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx)podataka".</span><span class="sxs-lookup"><span data-stu-id="473f7-110">If the run stops with **extension-dll-exception**, then click on those words to open the **Connector Space Object properties** window, and click on **Stack Trace...** to see more information on the underlying cause, as described in [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).</span></span>
5. <span data-ttu-id="473f7-111">Ako datoteka usluge obaveštavanja lozinkom (PCNS) izveštava **o grešci 6025** u evidenciji događaja tokom sinhronizacije lozinke, potvrdite izbor u polju za rešavanje problema sa funkcijom [pcns za izveštavanje 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).</span><span class="sxs-lookup"><span data-stu-id="473f7-111">If the Password Change Notification Service (PCNS) component reports **error 6025** in the event log during password synchronization, check the guide for troubleshooting [PCNS reporting error 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).</span></span>
6. <span data-ttu-id="473f7-112">Ako je potpuna Sinhronizacija sa agentom za upravljanje uslugama FIM spora, potvrdite izbor u polju za proveru **automatski** , kao što je opisano u [rešavanju problema spora ili viseće cele sinhronizacije](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).</span><span class="sxs-lookup"><span data-stu-id="473f7-112">If full synchronization with the FIM Service Management Agent is slow, check the **auto grow** setting for TempDB, as described in [Troubleshooting slow or hanging full synchronization](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).</span></span>
7. <span data-ttu-id="473f7-113">Ako se nalazite u grešci sa sprečenjem zaustavljanja servera sa neuspešnim kreiranjem-putem-veb-uslugama pomoću usluge Management AG za upravljanje uslugama, pogledajte članak [Podrška-Info: neuspešno kreiranje-putem-Veb-usluge](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) za pregled uzroka.</span><span class="sxs-lookup"><span data-stu-id="473f7-113">If you are encountering an error of stopped-server with failed-creation-via-web-services using the FIM Service Management Agent, see [Support-Info: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) for an overview of causes.</span></span>

