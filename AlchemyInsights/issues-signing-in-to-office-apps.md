---
title: Problemi sa prijavljivanjem u Microsoft 365 aplikacije
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: e4f2fea5c2f368ae240614ee1f7bc729338dd75d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579951"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Popravljanje aplikacija za Microsoft 365 "Nažalost, drugi nalog iz vaše organizacije je već potpisan u poruci

Da biste ispravili ovu grešku, pokušajte sledeće:

- Uklonite sve poslovne naloge, izuzev sa pogođenim nalogom, koristeći Windows postavke > **pristup poslu ili školi**.
- [Obrišite Office akreditive](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) koristeći Windows upravljač akreditivima.<br/>
    **Napomena:** Putanje registratora za Office 2016 su promenjene u 16,0. (Ex: \Software\microsoft\office\16.0\zajed\identitet\)
- Otvorite Office aplikaciju, odaberite stavku **File**"  >  **nalog**za datoteku"  >  **Sign Out**. Zatim se prijavite koristeći korisnički nalog sa važećom licencom. Detaljne informacije potražite u članku [Nalozi u sistemu Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Za Mac računar pročitajte članak [Nije moguće prijaviti se u Office 2016 za Mac aplikaciju](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Za više informacija pogledajte odeljak ["Nažalost, drugi nalog iz vaše organizacije je već prijavljen na ovom računaru" u sistemu Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).