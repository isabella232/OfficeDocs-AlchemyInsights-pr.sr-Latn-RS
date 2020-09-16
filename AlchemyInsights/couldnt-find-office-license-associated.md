---
title: Popravka Microsoft 365 aplikacija nije mogla da pronađe pridruženu poruku za Office licence
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: bd127d6287b4438f6105a6158abdbd5b964b7e70
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747709"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Ispravljanje Microsoft 365 aplikacija "nije bilo povezano sa porukom Office licenci"

Ako primite ovu poruku, Isprobajte sledeće:

1. Proverite zaštitni zid, antivirusni softver i postavke proxy servera da biste potvrdili da ne blokiraju Internet pristup aplikacijama Microsoft 365. Pogledajte [Microsoft 365 URL adrese i OPSEGE IP adresa](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Uklonite i [ponovo dodelite Office licencu](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) za pogođene korisnike. 
3. Otvorite Office aplikaciju i [odjavite](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) se sa bilo kog postojećeg korisničkog naloga.
4. Idite na Windows Settings > **nalozima**  >  **&** nalozima i uklonite sve naloge za posao osim naloga koji je uticao.
5. Idite na postavke operativnog sistema Windows > **nalozima**u operativnom sistemu  >  **Access**i isključite sve naloge za posao osim naloga koji je uticao.
6. Poništite stanje sistema Office. [Saznajte kako](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Prijavite](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) se koristeći korisnik koji utiče na njega.

Dodatne rešenja za rešavanje problema potražite [u članku nelicencirane greške proizvoda i aktivacije u sistemu Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).