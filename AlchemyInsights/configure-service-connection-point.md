---
title: Konfigurisanje mesta povezivanja usluge (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037287"
---
# <a name="configure-service-connection-point-scp"></a>Konfigurisanje mesta povezivanja usluge (SCP)

**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**

- **Razlog**: nije moguće čitati objekat SCP i dobiti informacije o AZURE AD zakupcu
- **Rezolucija**: pogledajte odeljak [Konfigurisanje mesta povezivanja usluge](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)


**Akcioni plan**

- Provera da li je uređaj primio GPO za kontrolisanu validaciju.
- Uverite se da je GPO kreirao registarske ključeve.
- Uverite se da imate 2 ključa kreirane pomoću direktorijuma ID-a i onkosistema.

**Konfigurisanje postavke registra na strani klijenta za SCP**

Koristite sledeći primer da biste kreirali objekat smernica grupe (GPO) za primenu postavki registratora koje konfiguriše stavku SCP u registratoru uređaja.

1. Otvorite konzolu za upravljanje smernicama grupe i kreirajte novi GPO u domenu.
     - Navedite novo GPO ime (na primer, Clientsidep)

2. Uredite GPO i pronađite sledeću putanju: **Konfiguracija računara > željene postavke > Windows postavkama > registratoru**.

3. Kliknite desnim tasterom miša na **registrator** i izaberite **stavku nova > registratora**.

4. Na kartici **Opšte** podesite sledeće:
  
- **Radnja**: ispravka
    
- **Saće: HKEY_LOCAL_MACHINE**
    
- **Ključna putanja**: Software\microsoft\windows\currentversion\cdj\aad
    
- **Ime vrednosti**: tenanti
    
- **Tip vrednosti**: REG_SZ
    
- **Podaci o vrednostima**: GUID ili ID direktorijuma vaše AURE instance oglasa (Ova vrednost se može pronaći u usluzi **Azure > Azure Active Directory > svojstvima > ID direktorijuma**)
 
- Kliknite na dugme **U redu**.
 
5. Kliknite desnim tasterom miša na **registrator** i izaberite **stavku nova > registratora**.

6. Na kartici **Opšte** podesite sledeće:
  
- **Radnja**: ispravka
    
- **Saće: HKEY_LOCAL_MACHINE**
    
- **Ključna putanja**: Software\microsoft\windows\currentversion\cdj\aad
    
- **Ime vrednosti**: ime tenanga
    
- **Tip vrednosti**: REG_SZ
    
- **Podaci o vrednosti**: verifikovano ime domena ako koristite federirani ambijent kao što je AD FS. Verifikovano ime domena ili onmicrosoft.com ime domena (na primer, comtoso. onmicrosoft). com ako koristite kontrolisano okruženje

- Kliknite na dugme **U redu**.

7. Zatvorite uređivač za novi kreirani GPO.

8. Povežite novi kreirani GPO na željeni računar koji sadrži domen koji pripadaju vašem kontrolisanom broju stanovnika.

Više informacija potražite u članku [kontrolisana validacija hibridnog AZURE AD JOIN-Azure AD | Microsoft docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) i  [Rešavanje problema hibridnog Azure aktivnog direktorijuma su spojeni | Microsoft docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).









