---
title: Problemi sa saglasnošću zaduženja za admini
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 08d3bfa84fd5ab31d7165090c392866d863898545ade7631e820a100eef89dea
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952587"
---
# <a name="admin-consent-issues"></a>Problemi sa saglasnošću zaduženja za admini

1. Omogućite [tok posla pristanka administratora da](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) biste omogućili korisnicima da zatraže odobrenje administratora direktno sa ekrana sa pristankom.

1. Ako vi ili korisnici aplikacije vidite neočekivane greške tokom procesa pristanka, pogledajte ovaj članak za korake za rešavanje problema: Neočekivana greška prilikom izvršavanja pristanka [na aplikaciju.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)

1. Saznajte [više](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)o saglasnosti Microsoft platforma za identitete, kako [](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) funkcioniše odziv za pristanak i kako da procenite zahtev za saglasnost širom [zakupitka.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent)

1. Aplikacije koje se integrišu sa Microsoft platforma za identitete prate model autorizacije koji korisnicima i administratorima omogućava da kontrolišu način pristupa podacima. Primena modela autorizacije ažurirana je na krajnjim tačkama programa Microsoft platforma za identitete menja način na koji aplikacija mora da vrši interakciju sa Microsoft platforma za identitete. Pogledajte [dozvole i saglasnost](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) u Microsoft platforma za identitete za pregled ovog modela autorizacije, uključujući obuhvaćenosti, dozvole i saglasnost.