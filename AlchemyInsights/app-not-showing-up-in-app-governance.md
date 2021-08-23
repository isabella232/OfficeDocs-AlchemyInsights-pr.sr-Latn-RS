---
title: Moja aplikacija se ne pojavljuje u upravljanju aplikacijama
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12734"
ms.openlocfilehash: a8d176fdee073e41b61de6f53c728601da955aaa
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/16/2021
ms.locfileid: "58454992"
---
# <a name="my-app-isnt-showing-up-in-app-governance"></a>Moja aplikacija se ne pojavljuje u upravljanju aplikacijama

Ako se aplikacija ne pojavljuje u upravljanju aplikacijama, proverite sledeće:

1. Idite u [Azure AD](https://aad.portal.azure.com/) i pronađite ID aplikacije za aplikaciju tako što ćete potražiti ime aplikacije na gornjoj traci na stranici Pregled.

1. Access Graph Explorer i potražite ID aplikacije u okviru principala usluge pomoću ovog upita i zamenite ga <appId> relevantnim ID-om aplikacije: < https://graph.microsoft.com/v1.0/servicePrincipals? $search= "appId: <appId> ">

1. Ako nema rezultata, potražite ID aplikacije u aplikaciji pomoću ovog upita i zamenite ga <appId> relevantnim ID-om aplikacije: < https://graph.microsoft.com/v1.0/applications? $search= "appId: <appId> ">

Ako naižete na probleme sa upitom, pogledajte [dobijanje podrške.](https://docs.microsoft.com/microsoft-365/business-video/get-help-support) 

Više informacija ili uvid u aplikacije u upravljanju aplikacijama potražite u temi Saznajte više o vidljivosti [i uvidima.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-overview)

Dodatne informacije o prikazivanja aplikacija potražite u [temi Prikaz aplikacija.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-view-apps)
