---
title: Uslovi koji nedostaju u SharePoint skladištu termina na mreži
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: d99458d6f9b65e44ad5945c909b9a8861cf0b1f23463fcdfd5b8351b1c08d670
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54106440"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Omogućavanje BitLocker šifrovanja pomoću funkcije Intune

Intune smernice za zaštitu krajnje tačke mogu da se koriste za konfigurisanje Postavki Boitlocker šifrovanja za Windows uređaje kao što je opisano u: Windows10 (i kasnijim) postavkama za zaštitu uređaja pomoću usluge Intune

Trebalo bi da imate na umu da mnogi noviji uređaji Windows 10 podržavaju automatsko bitlocker šifrovanje koje se pokreće bez primene MDM smernica. Ovo može da utiče na aplikaciju smernica ako su konfigurisane postavke koje nisu podrazumevane. Više detalja pročitajte u temi "Pitanja i o e-pošti".


Najčešća pitanja Q: Koja izdanja sistema Windows podržavaju šifrovanje uređaja pomoću smernica za zaštitu krajnje tačke?
O: Postavke u Intune smernicama za zaštitu krajnje tačke primenjuju se pomoću Bitlocker CSP datoteke.  Ne podržavaju sva izdanja i Windows Bitlocker CSP. U ovom trenutku Windows izdanja: Enterprise; Podržani su Education, Mobile, Mobile Enterprise i Professional (od revizacije 1809 pa na dalje).




P: Ako je uređaj već šifrovan pomoću funkcije BitLocker pomoću podrazumevanih postavki OS-a za metod šifrovanja i jačinu šifrovanja (XTS-AES-128) primeniće smernice sa različitim postavkama automatski će aktivirati ponovo šifrovanje disk jedinice pomoću novih postavki?

O: Ne. Da biste primenili nove postavke šifrovanja, disk jedinica prvo mora da bude dešifrena.

Natpis Za uređaje koji su upisani sa funkcijom Autopilot, automatsko šifrovanje do kojeg bi dolazilo tokom korišćenja programa OOBE ne pokreće se dok se ne procene Intune smernice koje dozvoljavaju da se postavke zasnovane na smernicama koriste na mestu podrazumevanih postavki OS-a




Q Ako je uređaj šifrovan kao rezultat primene Intune smernica, da li će se dešifrovati kada se te smernice uklone?

O: Uklanjanje smernica koje se odnose na šifrovanje NE rezultira dešifrovanjem disk jedinica koje su konfigurisane.




P: Zašto intune smernice za usaglašenost pokazuju da moj uređaj nema omogućen BitLocker, ali jeste?

O: Postavka "BitLocker je omogućen" u intune smernicama za usaglašenost koristi Windows Atestation health Device Health Attestation (DHA) klijenta. Ovaj klijent meri samo stanje uređaja pri pokretanju. Dakle, ako uređaj nije ponovo aktiviran pošto je bitLocker šifrovanje dovršeno, DHA usluga klijenta neće prijaviti bitLocker kao aktivan.