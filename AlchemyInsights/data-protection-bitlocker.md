---
title: DataProtection – Bitlocker
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 8166a055d7a967faab83484619b443cc98239c7c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815629"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Omogućavanje BitLocker šifrovanja pomoću funkcije Intune

Intune smernice za zaštitu krajnje tačke mogu da se koriste za konfigurisanje BitLocker postavki šifrovanja za Windows uređaje. Dodatne informacije potražite u [temi Postavke operativnog sistema Windows 10 (i kasnije) za zaštitu uređaja pomoću usluge Intune.](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)

Pored smernica za zaštitu krajnje tačke postoji i izveštaj o šifrovanju koji uređajima pruža detaljniji prikaz statusa šifrovanja. Ovom izveštaju može da se pristupi sa MEM portala u okviru Uređaji **> Monitor**, a zatim u okviru Izveštaj o šifrovanju **izaberite** [stavku Konfiguracija](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport).

Ako otkrijete da BitLocker nije omogućen na očekivani način ili da je profil koji se koristi za omogućavanje funkcije BitLocker u stanju greške, pregledajte izveštaj o šifrovanju da biste bolje razumeli zašto se ponašanje dešava.

Da biste pronašli detalje o tome kako da tumačite izveštaj koji uključuje različite vrednosti statusa šifrovanja, pogledajte nadgledanje šifrovanja uređaja [pomoću sajta Intune.](https://docs.microsoft.com/mem/intune/protect/encryption-monitor)

Trebalo bi da imate na umu da mnogi noviji uređaji koji rade pod operativnim sistemom Windows 10 podržavaju automatsko BitLocker šifrovanje koje se pokreće bez primene MDM smernica. Ovo može da utiče na primenu smernica ako su postavke koje nisu podrazumevane konfigurisane. Pogledajte sledeća najčešća pitanja za više detalja.

Informacije o rešavanju problema u funkciji BitLocker potražite u članku [Rešavanje problema sa BitLocker smernicama u aplikaciji Microsoft Intune.](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)
 
 
**NAJČEŠĆA PITANJA**

P: Koja izdanja operativnog sistema Windows podržavaju šifrovanje uređaja pomoću smernica za zaštitu krajnje tačke?<br>
O: Postavke u Intune smernicama za zaštitu krajnje tačke primenjuju se pomoću [Bitlocker CSP datoteke.](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp) Ne podržavaju sva izdanja ili izdanja operativnog sistema Windows Bitlocker CSP. <br><br>

P: Kako BitLocker može da se omogući na uređajima bez one ukidanja interakcije krajnjih korisnika?<br>
O: Sve dok su neophodni preduslovi ispunjeni, moguće je omogućiti Bitlocker "Silent Encryption" putem usluge Intune. Pogledajte detalje zahteva uređaja i primere postavki smernica za omogućavanje tihog šifrovanja u sledećem dokumentu: [Tiho omogući BitLocker šifrovanje](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices). <br><br>

P: Ako je uređaj već šifrovan pomoću funkcije BitLocker pomoću podrazumevanih postavki OS-a za metod šifrovanja i jačinu šifrovanja (XTS-AES-128), primena smernice sa različitim postavkama automatski će aktivirati ponovo šifrovanje disk jedinice pomoću novih postavki?<br>
O: Ne. Da biste primenili nove postavke šifrovanja, disk jedinica prvo mora biti dešifrena.<br><br>
**Napomogućeno:** Za uređaje koji su upisani pomoću funkcije Autopilot, automatsko šifrovanje koje bi se dešavalo tokom programa OOBE ne pokreće se dok se ne procene Intune smernice koje omogućavaju da se postavke zasnovane na smernicama koriste, a ne kao podrazumevane vrednosti OS.
 
P: Ako je uređaj šifrovan kao rezultat primene Intune smernica, da li će se dešifrovati kada se te smernice uklone?<br>
O: Uklanjanje smernica vezanih za šifrovanje NE rezultira dešifrovanjem disk jedinica koje su konfigurisane.
 
P: Zašto Intune smernice za usaglašenost pokazuju da na mom uređaju nije omogućen BitLocker, iako jeste?<br>
O: Postavka "BitLocker je omogućen" u Intune smernicama za usaglašenost koristi Windows Attestation Health Attestation (DHA) klijent. Ovaj klijent meri samo stanje uređaja pri pokretanju. Dakle, ako uređaj nije ponovo aktiviran nakon dovršenog BitLocker šifrovanja, DHA usluga klijenta neće prijaviti BitLocker kao aktivan.
 
 