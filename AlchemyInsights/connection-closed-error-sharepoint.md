---
title: Greška pri zatvaranju veze je zatvorena u programu SharePoint
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10802"
- "9006390"
ms.openlocfilehash: f0f82eaaa00d71992af445bb89346fb85bad3ade5d120b25ad3a6ea4f9674893
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/11/2021
ms.locfileid: "57883333"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>Greška "Osnova veza je zatvorena" u programu SharePoint

Ako dobijate grešku "Srodna veza je zatvorena" u programu SharePoint možda je povezana sa ukidanjem TLS 1.0/1.1. Više informacija potražite u sledećim člancima:

- [Priprema za TLS 1.2 u Office 365 i Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Greške u potvrdi identiteta se javljaju ako klijent nema podršku za TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Ispravka koja omogućava TLS 1.1 i TLS 1.2 kao podrazumevane bezbedne protokole u winHTTP protokolima u programu Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Ako su korisnici na Windows 7, proverite da li su proverili [TLS cipher pakete u programu Windows 7.](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)