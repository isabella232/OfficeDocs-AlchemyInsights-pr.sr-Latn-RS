---
title: Korišćenje PowerShell za deljenje smernica i odnosa sa organizacijom
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 717cdd6827e243ac6bf375209a911937c97088d2
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862154"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>Korišćenje PowerShell za deljenje smernica i odnosa sa organizacijom


Za relacije između organizacija Pregledajte detaljnu sintaksu i informacije o parametrima za: [Preuzimanje informacija](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [novo-organizationarelaciju](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [skup-organizationrelacija](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) i [Uklanjanje-organizationrelacija](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Da biste kreirali smernice za deljenje koristite [novu smernicu](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). Da biste [primenili smernice za deljenje na poštansko sanduče ili korisnika](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) , potrebno je da koristite kombinaciju [Set-poštansko sanduče](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) i [poštanskog sandučeta](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) sa Novokreiranim smernicama. Da biste [izmenili, onemogućili ili uklonili smernice za deljenje](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) koje su vam potrebne da biste koristili smernice za [Podešavanje](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) i [Uklanjanje](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy)smernica.

**Za potpuno razumevanje ove teme molimo vas da pročitate:**

[Deljenje u programu Exchange online](https://docs.microsoft.com/exchange/sharing/sharing)