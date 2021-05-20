---
title: 401 Neovlašćena greška u SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10935"
- "9001435"
ms.openlocfilehash: ac2fe27a8e7b277bfaf18303bf5b792410a1ea6a
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539946"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>401 Neovlašćena greška u SharePoint

Ako u programu SharePoint dobijete grešku "(401) Neovlašćeno", ona može biti povezana sa ukidanje TLS 1.0/1.1. Više informacija potražite u članku:

- [Priprema za TLS 1.2 u Office 365 i Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Greške u potvrdi identiteta se javljaju ako klijent nema podršku za TLS 1.2](/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Ažuriranje da biste omogućili TLS 1.1 i TLS 1.2 kao podrazumevane bezbedne protokole u winHTTP-u Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Ako su korisnici na Windows 7, proverite da li su proverili [TLS cipher pakete u programu Windows 7.](/windows/win32/secauthn/tls-cipher-suites-in-windows-7)