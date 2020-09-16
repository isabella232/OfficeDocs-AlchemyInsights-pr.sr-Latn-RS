---
title: Nedostaje uslovi iz prodavnice termina za usluge SharePoint online
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
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750465"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Omogućavanje BitLocker šifrovanja pomoću Intune

Smernice zaštite krajnjih tačaka mogu se koristiti za Konfigurisanje postavki usluge šifrovanje Boitlocker za Windows uređaje kao što je opisano u: Windows10 (i novije) postavkama da bi se zaštitili uređaji pomoću funkcije Intune

Trebalo bi da budete svesni da mnogi noviji uređaji koji koriste Windows 10 podržavaju BitLocker šifrovanje koji se pokreće bez aplikacije MDM smernica. Ovo može da utiče na primenu smernica ako su podrazumevane postavke podešene. Više detalja potražite u članku najčešća pitanja.


Najčešća pitanja   p: koja izdanja operativnog sistema Windows podržavaju šifrovanje uređaja pomoću smernica za zaštitu krajnje tačke?
 A: postavke u smernicama za zaštitu krajnje tačke se sprovode pomoću BitLocker CSP.Ne mogu sva izdanja ili verzije operativnog sistema Windows da podrže BitLocker CSP. 
      U ovom trenutku Windows izdanja: Enterprise; Podrška za edukaciju, mobilne uređaje i profesionalce (od 1809 ka ka njima) podržana je.




Q: ako je uređaj već šifrovan pomoću usluge OS BitLocker pomoću podrazumevanih postavki OS za šifrovanje i jačine šifrovanja (XTS-AES-128) primeniće se smernice sa drugim postavkama automatski pokrenuti šifrovanje disk jedinice sa novim postavkama?

O: Ne. Da biste primenili nove postavke šifrovanja, disk mora biti dešifruo.

Napomena za uređaje koji se upisuju sa Autoautopilot automatskim šifriranjem koji bi se dogodio tokom OOBE nije aktiviran dok se ne proceni da se smernice zasnovane na smernicama koriste umesto podrazumevanih vrednosti OS




Ako je uređaj šifrovan kao rezultat aplikacije "Intune", da li će biti dešifrovana kada se ta smernica ukloni?

A: uklanjanje povezanih smernica za šifrovanje ne prouzrokuje dešifrovanje diskova koje su konfigurisane.




P: Zašto smernice za usaglašenost sa Intune prikazuju da moj uređaj nema "omogućen je BitLocker omogućen", ali da li je?

A: postavka "omogućena za BitLocker omogućeno" u Intune smernicama za usaglašenost koristi Windows uređaj za zdravstvenu proveru (DHA). Ovaj klijent Meri samo stanje uređaja u vreme pokretanja. Ako uređaj nije ponovljen od kada je BitLocker šifrovanje dovršen, funkcija DHA klijent neće prijaviti BitLocker kao aktivni.