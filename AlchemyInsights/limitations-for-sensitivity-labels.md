---
title: Ograničenja oznaka osetljivosti za Kancelarija datoteka u programima SharePoint i OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12451"
- "9000181"
ms.openlocfilehash: e197c43712c0ead9508a1cfdf48b51d01d2ae957649f73703f9c33733e332bf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813165"
---
# <a name="limitations-for-sensitivity-labels-for-office-files-in-sharepoint-and-onedrive"></a>Ograničenja oznaka osetljivosti za Kancelarija datoteka u programima SharePoint i OneDrive

Kada omogućavate oznake osetljivosti za Kancelarija datoteke u SharePoint i OneDrive, imajte na umu zahteve i ograničenja, u koja spadaju:

- SharePoint i OneDrive neke datoteke označene i šifrovane iz Kancelarija aplikacija za računare kada datoteke sadrže PowerQuery podatke, podatke koje skladište prilagođeni programski dodaci ili prilagođene XML delove.
- SharePoint i OneDrive oznake osetljivosti ne primenjuju automatski na postojeće datoteke koje ste već šifrovali pomoću Azure Information Protection (AIP) oznaka. Da biste primenili oznake osetljivosti na šifrovane datoteke: 
    - Uverite se da su AIP oznake migracije i objavljene u Microsoft 365 za usaglašenost.
    - Preuzmite označene datoteke, a zatim ih otpremite na originalnu SharePoint ili OneDrive lokaciji.
- Štampanje šifrovanih dokumenata nije podržano.

Dodatne detalje o ograničenjima možete da vidite u Kancelarija oznake osetljivosti za [datoteke u SharePoint i OneDrive.](/microsoft-365/compliance/sensitivity-labels-sharepoint-onedrive-files#limitations)
