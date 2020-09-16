---
title: Zaštita podataka – BitLocker
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
- "1802"
- "9000220"
ms.openlocfilehash: ab28162fcdf0a37060be3bdf15a78aceca7a48b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731253"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Omogućavanje BitLocker šifrovanja pomoću Intune

 Smernice zaštite krajnjih tačaka mogu se koristiti za konfigurisanje BitLocker postavki šifrovanja za Windows uređaje. Više informacija potražite u članku [Postavke operativnog sistema Windows 10 (i novije) kako biste zaštitili uređaje pomoću funkcije Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).
 
Trebalo bi da budete svesni da mnogi noviji uređaji koji koriste Windows 10 podržavaju BitLocker šifrovanje, koji se pokreće bez aplikacije MDM smernica. Ovo može da utiče na primenu smernica ako su postavke koje nisu podrazumevane. Detaljnije pogledajte sledeće najčešća pitanja.
 
Informacije o rešavanju problema sa BitLocker problemom potražite [u članku rešavanje problema sa BitLocker smernicama u programu Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**NAJČEŠĆA PITANJA**

 Q: koje izdanje sistema Windows podržava šifrovanje uređaja pomoću smernica za zaštitu krajnje tačke?<br>
 A: postavke u smernicama za zaštitu krajnje tačke se sprovode pomoću [BitLocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). Ne svi izdanci ili verzije operativnog sistema Windows podržavaju BitLocker CSP. <br><br>
      U ovom trenutku, podržavaju se sledeća izdanja operativnog sistema Windows: Enterprise, edukacija, mobilni, mobilni Enterprise i Professional (izdanje 1809 i novije verzije).
 
P: ako je uređaj već šifrovan pomoću usluge OS BitLocker pomoću podrazumevanih postavki OS za šifrovanje i jačine šifrovanja (XTS-AES-128), primena smernica sa drugim postavkama automatski izaziva ponovno šifrovanje disk jedinice sa novim postavkama?<br>
O: Ne. Da biste primenili nove postavke šifrovanja, disk jedinica mora prvo da se dešifruje.<br><br>
**Napomena:** Za uređaje koje se upisuju na Autoautopilot, automatsko šifrovanje koje bi se desilo tokom OOBE ne pokreće se dok se ne proceni politika Intune, što omogućava postavkama zasnovane na smernicama da se koriste umesto podrazumevanih vrednosti OS.
 
Q: ako je uređaj šifrovan kao rezultat primene smernica Intune, da li će se dešifruti kada se ta smernica ukloni?<br>
A: uklanjanje smernica vezanim za šifrovanje ne prouzrokuje dešifrovanje diskova koje su podešene.
 
P: Zašto smernice za usaglašenost sa Intune prikazuju da moj uređaj nema omogućen BitLocker, čak i ako jeste?<br>
A: postavka "omogućeno je da BitLocker omogućena" u smernicama za usaglašenost u Intune koristi Windows uređaj za zdravstvenu proveru (DHA) klijentu. Ovaj klijent Meri samo stanje uređaja u vreme pokretanja. Ako uređaj nije ponovo rešen od završetka usluge BitLocker šifrovanja, usluga DHA klijenta neće prijaviti da je BitLocker aktivan.
 
 