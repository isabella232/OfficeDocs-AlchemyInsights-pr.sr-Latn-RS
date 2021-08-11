---
title: Testiranje IRM konfiguracije za nove OME mogućnosti
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12428"
- "9000078"
ms.openlocfilehash: 62697d6379ea6ab3c6af86d3bab752af560da7c1250e5ef6dd2a3eae8023a05e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812445"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>Testiranje IRM konfiguracije za nove OME mogućnosti

Da biste potvrdili Microsoft 365 da je Microsoft 365 konfigurisan da koristi nove OME mogućnosti, pokrenite sledeće cmdlet Exchange Online [u programu PowerShell:](/powershell/exchange/exchange-online-powershell)


1. Proverite IRM konfiguraciju zakuljca tako što biste pokrenuti `Get-IRMConfiguration` . Uverite se da su ove vrednosti postavljene na **Tačno:**
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. Pokrenite domen, adresu pošiljaoca i `Test-IRMConfiguration` primaoca. Ako test ne prođe, ispitajte IRM konfiguraciju.

Više informacija o verifikaciji IRM konfiguracije potražite u članku Verifikacija nove [OME konfiguracije u programu Exchange Online PowerShell.](/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell)