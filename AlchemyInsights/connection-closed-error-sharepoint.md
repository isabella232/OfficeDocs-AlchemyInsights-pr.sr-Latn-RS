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
ms.openlocfilehash: b64215b5b83ef1092eb58791e6dbb015b72d422d
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233440"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a><span data-ttu-id="5b046-102">Greška "Osnova veza je zatvorena" u programu SharePoint</span><span class="sxs-lookup"><span data-stu-id="5b046-102">"The underlying connection was closed" error in SharePoint</span></span>

<span data-ttu-id="5b046-103">Ako dobijate grešku "Osnova veza je zatvorena" u programu SharePoint možda je povezana sa ukidanjem TLS 1.0/1.1.</span><span class="sxs-lookup"><span data-stu-id="5b046-103">If you are receiving the error "The underlying connection was closed" in SharePoint it might be related to the deprecation of TLS 1.0/1.1.</span></span> <span data-ttu-id="5b046-104">Više informacija potražite u sledećim člancima:</span><span class="sxs-lookup"><span data-stu-id="5b046-104">For more info, see these articles:</span></span>

- [<span data-ttu-id="5b046-105">Priprema za TLS 1.2 u Office 365 i Office 365 GCC</span><span class="sxs-lookup"><span data-stu-id="5b046-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide)

- [<span data-ttu-id="5b046-106">Greške u potvrdi identiteta se javljaju ako klijent nema podršku za TLS 1.2</span><span class="sxs-lookup"><span data-stu-id="5b046-106">Authentication errors occur if client doesn't have TLS 1.2 support</span></span>](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

<span data-ttu-id="5b046-107">Ako su korisnici na Windows 7, proverite da li su proverili [TLS cipher pakete u programu Windows 7.](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)</span><span class="sxs-lookup"><span data-stu-id="5b046-107">If users are on Windows 7, make sure they check [TLS Cipher Suites in Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span></span>