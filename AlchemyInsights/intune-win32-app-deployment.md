---
title: Primena Win32 aplikacije za primenu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461992"
---
# <a name="intune-win32-app-deployment"></a>Primena Win32 aplikacije za primenu

Microsoft Intune omogućava Win32 aplikacijama, uključujući ali nije ograničeno na MSI i. EXE treba da bude raspoređena na Windows 10 uređaje. Korišćenje mehanizma za primenu zahteva proširenje Intune (IME) koje će biti na ciljnom uređaju. IME će se automatski instalirati kao rezultat automatskog usmeravanje ili Win32 primene aplikacije na korisnika/device.

Postoji i niz preduslova koji moraju da se ispune da bi se primenili Win32 aplikacije koje spadaju:

- Podržane platforme: Windows 10 verzija 1607 ili novije verzije (Enterprise, Pro i obrazovni verzije).
- Podržana arhitektura: x86 i x64.
- Upravljanje uređajima: AAD se pridružio i automatski upisan (uključujući hibridne domene pridruženu i grupne smernice grupe).
- Format paketa aplikacije:. IT **datoteka koju**  je pripremila [Microsoft Win32 alatka za pripremu sadržaja](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).
- Vanje
    - Maksimalna veličina: 8 GB.
    - Nepodržana arhitektura: oružje.

Pregledajte stavku "[Dodavanje, dodela i nadgledanje Win32 aplikacije u programu Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" za informacije koje se tiču tih koraka.

Detalji o rešavanju problema sa primenom aplikacije u operativnom sistemu Windows uključujući Win32 aplikacije mogu se redigovati u sledećim dokumentima

- [Rešavanje problema sa instalacijom aplikacija](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [Rešavanje problema sa Win32 aplikacijama](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)