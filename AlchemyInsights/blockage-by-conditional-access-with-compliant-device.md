---
title: Uslovni pristup me blokira pomoću usagašenog uređaja
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
ms.openlocfilehash: 709749b1a62f2d9cdabfb3fe4b7538c22101d7109204d9163f6059336b817bf8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019162"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>Uslovni pristup me blokira pomoću usagašenog uređaja

**Izuzetno preporučene alatke**

- [Alatka za rešavanje problema sa registracijom uređaja](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – Sveobuhvatna alatka koja pomaže u rešavanju najčešćih problema sa registracijom uređaja.
- [Testiranje skripte registracije](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) uređaja – Alatka koja se koristi za obezbeđivanje da uređaj može da pristupi krajnjim tačkama registracije uređaja u okviru naloga sistema.
- [Skripta za čišćenje Azure AD](https://github.com/mzmaili/AzureADDeviceCleanup) uređaja – Alatka koja se koristi za traženje zauštenih uređaja i upravljanje zastojima u okruženju.

Ovo su neki uobičajeni razlozi zašto uslovni pristup možda ne radi na  usagašenom uređaju ili zašto vaši korisnici možda dobijaju Ovde ne možete da odete poruku tokom zahteva za prijavljivanje u organizacioni resurs.

1. **Uređaj nije u stanju potrebnog uređaja sa MDM uređajem:**

Proverite da li je uređaj upisan kod odobrenog MDM dobavljača kao što je Intune i označen *kao usaglasan*. Dodatne informacije o sajtu Intune potražite u ovom [dokumentu.](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) Da biste bolje razumeli usaglašenost uređaja i intune, pogledajte tj. korišćenje smernica za usaglašenost da biste podesili pravila za uređaje na koje [upravljate pomoću usluge Intune.](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started) Ako imate problema sa upisivanju uređaja pomoću usluge Intune, detalje o rešavanju problema pronađite u članku Rešavanje problema sa upisivanju [uređaja u Microsoft](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune). Za dalju Intune podršku kreirajte zahtev za podršku. Da biste to uradio, posetite [stranicu "Pomoć i podrška za Intune"](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport).

2. **Uređaj nije pridružen mreži organizacija:**

Da biste pristupili resursima organizacije, uređaj mora da bude povezan sa mrežom organizacije, putem direktne veze ili virtuelne privatne mreže (VPN), kao i pridruženojoj lokaciji ili Azure Active Directory. Da biste se pridružili poslovnim uređajima na mreži organizacije, pogledajte [pridruživanje poslovnim uređaju mreži organizacije.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network) Da biste registrovali lični/BYOD uređaj, pogledajte [registrovanje ličnog uređaja na mreži organizacije.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network)

- Da biste proverili da li se uređaj pridružio mreži, ovde možete da pratite korake za registrovane uređaje [ili](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) radne [uređaje.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined) Da biste suzili problem na mrežno povezivanje za mrežu Org, pratite dolenaveđena uputstva:

    1. Prijavite se u Windows koristeći poslovni ili školski nalog, na primer alain@contoso.com.
    2. Povezivanje na mrežu vaše organizacije putem VPN-a ili DirectAccess.
    3. Kada se povežete, pritisnite taster sa **Windows logotipom + L** da biste zaključali uređaj.
    4. Otključajte uređaj pomoću poslovnih ili školskih naloga, a zatim ponovo pokušajte da pristupite problematičnoj aplikaciji ili usluzi.

Ako vidite poruku o **grešci Ovde ne možete ponovo** da je dobijete, problem je verovatno na drugom mestu.

3. **Operativni sistem nije podržan:**

Uverite se da imate podržanu verziju operativnog sistema, uključujući:

- **Windows – klijent**: Windows 7 ili kasnije

- **Windows server:** Windows Server 2008 R2 ili kasnije

- **macOS**: macOS X ili kasnije

- **Android i iOS**: Najnovija verzija operativnih sistema Android i iOS mobilnih sistema

4. **Veb pregledač nije podržan:**

Pronađite podržane pregledače u nastavku. Za podršku za Chrome sa Windows 1703 ili novijim verzijama, potrebno je proširenje Windows 10 Nalozi. Za Edge 85+, korisnik mora biti prijavljen da bi ispravno prošao informacije o usaglašenosti uređaja. Više detalja možete da vidite [ovde.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)

- **Windows 10:** Microsoft Edge, Internet Explorer, Chrome
- **Windows 8 / 8.1**: Internet Explorer, Chrome
- **Windows 7**: Internet Explorer, Chrome
- **iOS**: Microsoft Edge, Intune Kontrolisani pregledač, Safari
- **Android**: **Microsoft Edge**: Intune kontrolisani pregledač, Chrome
- **Windows Phone:** Microsoft Edge, Internet Explorer
- **Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016**: Internet Explorer
- **Windows Server 2012 R2**: Internet Explorer
- **Windows Server 2008 R2**: Internet Explorer
- **macOS**: Chrome, Safari

Dodatne informacije o **poruci Ne možete da pronađete ovde i** o koracima za rešavanje [problema ovde.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation)
