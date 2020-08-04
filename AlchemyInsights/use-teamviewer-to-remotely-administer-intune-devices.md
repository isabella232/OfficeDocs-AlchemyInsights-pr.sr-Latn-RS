---
title: Korišćenje Timprikazivača za daljinsko upravljanje Intune uređajima
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555748"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a>Korišćenje Timprikazivača za daljinsko upravljanje Intune uređajima

Uređaji kojima upravlja Intune mogu da se administriraju daljinski, koristeći [Timviewer](https://www.teamviewer.com/).

Da biste administrirate Intune pomoću Timprikazivača, slijedite ove korake: 

Počnite tako što ćete dobiti akreditive iz Timprikazivača da biste podesili konektor Timprikazivača na Intune. Ovo omogućava administratoru da unese akreditive u korisničkom interfejsu "Timviewer konektor" u okviru uređaja, jednokratna operacija za uspostavljanje veze između Intune i usluge Timviewer.

**Deo 1: pokretanje sesije sa udaljenim uređajem**

1. U okviru stavke **Svi uređaji**izaberite uređaj sa kojim želite da započnete udaljenu sesiju.
2. Od **... Više**, izaberite **novu sesiju daljinske pomoći**.
3. Izaberite **da** da biste potvrdili da želite da uspostavite udaljenu sesiju.
    Nakon što je usluga Timviewer potvrdila zahtev "pokretanje nove udaljene sesije", videćete opciju da **pokrenete daljinsku pomoć** u okviru detalja okna za pregled (ili, Essentials) za uređaj. Izaberite stavku **vidi više** da biste razvili okno i prikazali status daljinske pomoći.
4. Izaberite stavku " **Započni udaljenu sesiju** " da biste pokrenuli sesiju na strani administratora.
5. Odaberite da preuzmete binarni prikazivač "Timviewer" (Windows) i izaberite stavku " **Pokreni**".<br/>
    **Belešku** Možete da zanemarite bilo koju stranicu Web pregledača koja je otvorena na Web lokaciji Timviewer.

6. Potvrđuje zahtev za aplikaciju Timviewer da bi se promene na uređaju (samo za Windows).
7. Pokreće se aplikacija Timviewer i uključuje kôd sesije za potvrdu verodostojnosti veze sa udaljenim uređajem.

**Deo 2: uređaj koji je usmeren na udaljenu sesiju**

1. Otvorite portal "Intune Company".
2. Potražite zastavicu za obaveštenje: "vaš IT administrator zahteva kontrolu nad ovim uređajem za sesiju daljinske pomoći" i izaberite obaveštenje.
3. Odaberite da preuzmete aplikaciju Timviewer ili da potvrdite Preuzimanje aplikacije Timviewer iz skladišta aplikacija, a zatim izaberite komandu " **Pokreni**".
    **Belešku** Možete da zanemarite bilo koju stranicu Web pregledača koja je otvorena na Web lokaciji Timviewer.

4. Potvrđuje zahtev za aplikaciju Timviewer da bi se promene na uređaju (samo za Windows).
5. Pokreće se aplikacija Timviewer i uključuje kôd sesije za potvrdu verodostojnosti veze sa udaljenim uređajem.
6. Iskačući meni vas pita da li želite da dozvolite pokretanje sesije.

**Belešku** Kodovi sesije koje je generisao usluga "Timviewer" predstavljaju samo jednokratno korišćenje. Ako izgubite vezu, morate da:

1. Zatvorite instancu aplikacije Timviewer na udaljenom uređaju i na admin Workstation.
2. Zatvorite portal kompanije na udaljenom uređaju.
3. Iniciranje nove "nove sesije daljinske pomoći" sa administratorskog portala.
4. Ponovo otvorite portal kompanije na udaljenom uređaju da biste dobili novo obaveštenje.
5. Preuzmite i otvorite aplikaciju Timviewer na udaljenom uređaju i u okviru administratorske radne stanice kao što je ranije.