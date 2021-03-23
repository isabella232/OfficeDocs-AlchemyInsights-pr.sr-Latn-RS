---
title: Blokirano mi je uslovno pristup uz uređaj koji se pridružio domenu
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/20/2021
ms.locfileid: "51038101"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a>Blokirano mi je uslovno pristup uz uređaj koji se pridružio domenu

**Visoko preporučene alatke**

[Alatka za rešavanje problema sa registracijom uređaja](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – alatka koja pomaže u rešavanju problema sa najčešćim problemima sa registracijom uređaja.

[Probna greška registracionog povezivanja uređaja](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – scenarij koji pomaže da se osigura da uređaj pristupi krajnjim tačkama registracije uređaja ispod sistemskog naloga.

[Azure reklama za čišćenje](https://github.com/mzmaili/AzureADDeviceCleanup) -rukopis koji vam omogućava da tražite zastarele uređaje u okruženju i da ih upravljate.

Evo nekih uobičajenih razloga zbog kojih uslovno pristup možda otkazuje uređaj koji se pridružio domenu (hibridni Azure AD).

1. **Ne postoji Azure PRT reklama na uređaju** – morate da se osigurate da uređaj ima Token Azure AD primarno osvežavanje (prt). Više informacija o PRT-u potražite u [dokumentu](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

Da biste proverili da li imate Azure AD PRT, možete da pokrećete `dsregcmd/status` komandu na uređaju i proverite da li je "Azučitprt" jednako "da".

Ako je "Azučitprt" "ne", potvrdite sledeće:

- **Bez obzira na to da li imate federirani ambijent sa uslugom AD FS i nije pristupačan na kućnim mrežama vaših korisnika**: u ovom slučaju, uverite se da su krajnje tačke "razlikovanje korisnika" pristupačne na osnovu ektraneta. Ako se oglas bavi za VPN, uverite se da se korisnici povežu sa VPN mrežom i ponovo se prijavite na uređaj. Više informacija potražite u članku ovaj [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).

- **Da li je TPM TPM neispravan i na taj način ne može da potvrdi verodostojnost uređaja**: proverite "TPM. msc" da biste videli da li je stanje TPM "spremno". Ako nije, `dsregcmd/leave` Neka se uređaj ponovo pridruži Azure AD. Zatim pokušajte ponovo. Više informacija potražite u članku ovaj [dokument](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).

- **Koristite nezavisnog dobavljača identiteta, koji ne podržava WS-Trust protokol**. Kao što je opisano u našim dokumentima, hibridni Azure spojeni uređaji ne mogu da rade u ovom slučaju. Radite sa dobavljačem identiteta za podršku.

2. **Korisnici koriste pregledač sa hromom bez Windows 10 naloga** ili **Office proširenja hroma ne koristi automatski prt u udruženim sistemima za AAD ili hibridne AAD**: to dovodi do otkazivanja bilo kakve uslovne smernice zasnovane na uređaju, a prikazuje se poruka o grešci "neregistrovani uređaj". Da biste ispravno koristili pregledač sa hromom, morate da instalirate "Windows 10 nalozi" ili "Office ekstenzije za korisnike" putem usluge SCCM ili Intune. Više informacija potražite u članku ovaj [dokument](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

Ako ne možete da pritisnete daljinski upravljač, obavestite korisnike da ručno instaliraju jednu od gorenavedenih proširenja da biste pristupili aplikacijama koje imaju uslovni pristup zasnovan na uređaju. Više informacija potražite u članku ovaj [dokument](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).

3. **Uređaj je bio ispravljen hibridni Azuri AD je pridružen, ali je nenamerno izbrisan ili invalid, bilo da su sinhronizovane promene u alatki AZOR AD Connect ili sa azulskog portala**: ako se to desi, objekat sa uređajem se više ne prepoznaje kao potpuno spojeni uređaj, čak i ako je status "Azureadconnect" i "prt" prikazan kao važeće na uređaju.

Da biste rešili ovaj problem, uradite to `dsregcmd/leave` na uređajima na koje utiče i dozvolite im da se ponovo pridruži Azure AD. Više informacija potražite u članku ovaj [dokument](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).

> [!NOTE]
> Ako su uređaji u operativnom sistemu Windows 10, 1809 Update, uz VPN/Cloud proxy i pogledajte probleme sa stanjem "Azučitprt" ili bilo koju aplikaciju sa SSO problemom (Outlook ne povezuje sa poštanskim sandučetom čak i ako ste imali PRT), uverite se da imate ovu zakrpu [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) ili aprilske kumulativne ispravke [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) da biste sprečili propusta na tim uređajima.

















