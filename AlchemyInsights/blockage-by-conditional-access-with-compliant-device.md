---
title: Blokira me uslovno pristup sa usaglašenim uređajem
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 240bd25f4d62505202c8cd7ceabe4c1cd3d5c0b5
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037075"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>Blokira me uslovno pristup sa usaglašenim uređajem

**Visoko preporučene alatke**

- [Alatka za rešavanje problema sa registracijom uređaja](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – sveobuhvatna alatka koja pomaže u rešavanju uobičajenih problema sa registracijom uređaja.
- [Probna greška registrovanja za registraciju uređaja](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – alatka koja se koristi za obezbeđivanje krajnjih tačaka registracije uređaja ispod sistemskog naloga.
- [Azure alatka za čišćenje čišćenja uređaja](https://github.com/mzmaili/AzureADDeviceCleanup) – alatka koja se koristi za traženje zastareli uređaja u okruženju.

Evo nekih uobičajenih razloga zašto uslovno pristup može da bude neispravni za usaglašeni uređaj ili zašto vaši korisnici mogu da primaju ne možete da **dobijete poruku od ove** poruke tokom zahteva za prijavljivanje u program za organizovanje.

1. **Uređaj se ne nalazi u obavezno stanje uređaja sa MDM**:

Proverite da li je uređaj upisan sa odobrenim MDM uređajem kao što je Intune i *označen kao usaglašeni*. Više informacija o init videćete ovaj [dokument](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment). Da biste bolje razumeli usaglašenost i Intune, pogledajte članak [Korišćenje smernica za usaglašenost za podešavanje pravila za uređaje sa kojima upravljate pomoću Intune](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started). Ako imate problema sa ugrađenim uređajem pomoću Intune, pronađite detalje o rešavanju problema u [članku rešavanje problema sa uređajem u programu Microsoft](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune). Za dodatnu podršku za Intune Kreirajte zahtev za podršku. Da biste to uradili, posetite [stranicu pomoć i podrška za Intune](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport).

2. **Uređaj nije pridružen organizacijama organizacije**:

Za pristup organizacionim resursima, uređaj mora da se poveže sa mrežom organizacije, putem direktne veze ili virtuelne privatne mreže (VPN) i takođe se pridružuje na lokalno ili Azure aktivnom direktorijumu. Da biste se na računaru organizacije pridružili poslu, pogledajte članak [pridruživanje svom poslu uređaja na mreži organizacije](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network). Da biste registrovali lični/BYOD uređaj, pogledajte članak [Registrovanje ličnog uređaja na mreži organizacije](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network).

- Da biste proverili valjanost da li se uređaj pridružio mreži, možete da izvršite korake za registraciju [ovde](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) ili za poslovne uređaje [.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined) Da biste opsežali problem za organizaciju mrežne veze, slede uputstva ispod:

    1. Prijavite se u Windows pomoću poslovnog ili školskog naloga, na primer, alain@contoso.com.
    2. Povežite se sa mrežom organizacije kroz VPN ili DirectAccess.
    3. Kada se povežete, pritisnite taster sa **Windows logotipom + L** da biste zaključali uređaj.
    4. Otključajte uređaj pomoću poslovnog ili školskog naloga, a zatim ponovo isprobajte problematičnu aplikaciju ili uslugu.

Ako vidite da ne možete ponovo da dobijete poruku o grešci, problem je verovatno **na** drugom mestu.

3. **Operativni sistem nije podržan**:

Uverite se da koristite podržanu verziju operativnog sistema, uključujući:

- **Windows klijent**: Windows 7 ili noviji

- **Windows Server**: windows Server 2008 R2 ili noviji

- **MacOS** X ili noviji

- **Android i iOS**: najnovija verzija Android i iOS mobilnog operativnog sistema

4. **Veb pregledač nije podržan**:

Pronađite podržani pregledači ispod. Za podršku na hromu sa operativnim sistemom Windows 1703 ili novijim verzijama obavezno je proširenje Windows 10 naloga. Za Edge 85 +, korisnik mora da bude prijavljen da bi ispravno prosleđen informacije o usaglašenosti uređaja. Više detalja potražite u članku [ovde](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

- **Windows 10**: Microsoft Edge, Internet Explorer, Chrome
- **Windows 8/8,1**: Internet Explorer, Chrome
- **Windows 7**: Internet Explorer, Chrome
- **iOS**: Microsoft Edge, Intune kontrolisani pregledač, safari
- **Android**: **Microsoft Edge**: Intune kontrolisani pregledač, Chrome
- **Windows Phone**: Microsoft Edge, Internet Explorer
- **Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016**: Internet Explorer
- **Windows Server 2012 R2**: Internet Explorer
- **Windows Server 2008 R2**: Internet Explorer
- **MacOS**: Chrome, safari

Pronađite više informacija o tome ne možete da **dobijete tu** poruku [i korake za](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation)rešavanje problema.
