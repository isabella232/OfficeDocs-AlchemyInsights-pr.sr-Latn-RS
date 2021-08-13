---
title: Rešavanje problema sa saglasnošću korisnika
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
ms.openlocfilehash: db784c133fec554604ad09f5b27941879d97ff238f926ff6338d0f3b7c3c4105
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007912"
---
# <a name="troubleshoot-user-consent"></a>Rešavanje problema sa saglasnošću korisnika

1. Možete da konfigurišete način na koji krajnji korisnici pristaju na aplikacije putem Azure portala ili programa PowerShell. Pogledajte [postavke pristanka korisnika za](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) više informacija.
1. Administrator takođe može da koristi [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) da bi dodelio saglasnost za delegirane dozvole u ime jednog korisnika. Više informacija potražite u [temi Dobijanje pristupa u ime korisnika.](https://docs.microsoft.com/graph/auth-v2-user)
1. [Greške pristanak na korisnika:](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)u ovom članku se govori o greškama do kojih može doći tokom procesa pristanka na aplikaciju. Ako rešavate probleme sa neočekivanim odzivima o pristanku koji ne sadrže nikakve poruke o grešci, pogledajte scenario potvrde identiteta [za Azure AD.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)