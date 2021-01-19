---
title: Rešavanje problema sa korisničkim odobravama
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
- "9004353"
- "7785"
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901631"
---
# <a name="troubleshoot-user-consent"></a>Rešavanje problema sa korisničkim odobravama

1. Možete da konfigurišete kako krajnji korisnici odobravate aplikacije putem Azure portala ili PowerShell. Više informacija potražite u članku [postavke korisničkog pristanka](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) .
1. Administrator može da koristi i [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) za odobravanje saglasnosti za delegirane dozvole u ime jednog korisnika. Više informacija potražite u članku [pristup pristupu u ime korisnika](https://docs.microsoft.com/graph/auth-v2-user).
1. [Greške korisnika](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): ovaj članak govori o greškama koje se mogu pojaviti tokom procesa saglasnosti sa primenom aplikacije. Ako rešavate neočekivani pristanak koji ne sadrže nijednu poruku o grešci, pročitajte članak [scenariji potvrde identiteta za Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).