---
title: Uvoz i izvoz iz usluge Yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037260"
---
# <a name="import-and-export-from-yammer"></a>Uvoz i izvoz iz usluge Yammer

**Biste**

Opcije uvoza korisnika se razlikuju u zavisnosti od toga da li je Yammer mreža u [osnovnom režimu za Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)ili ne.

- **Režim koji nije osnovni**: korisnici mogu da se uvezu u grupe pomoću stavke [Dodaj iz adresara](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (ograničavanje na 100 korisnika) u okviru postavke grupe ili na mrežu pomoću [masovne ispravke](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) u administratoru mreže.
- **Osnovni režim**: članstvo u grupi i operacije članstva u mreži treba da se izvršavaju sa [Microsoft 365 administrator administracije](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portala](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)ili pomoću druge Azure AD AD. Mreže u osnovnom režimu više nemaju pristup masovne ispravke i drugim funkcijama nasleđa.

> [!IMPORTANT]
> Yammer nikada nije podržavao uvoz sadržaja iz administracije mreže čak i kada je funkcija izvoza podataka korišćena u drugoj mreži. Sadržaj može ponovo da se knjiži pomoću partnerskih rešenja ili Yammer OSTATAK API-ja.

**Zno**

[Izvoz mrežnih podataka u okviru administrator mreže](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) omogućava izvoz sadržaja sa Yammer mreža, uključujući poruke i datoteke. Prilozi mogu da budu izuzetno veliki i prouzrokovaće da se izvoz može značajno popuniti. Preporučujemo da se aktivne mreže izvozi pomoću API-ja za [Izvoz podataka](https://developer.yammer.com/docs/data-export-api) u delovima po danu ili sedmici. Microsoft podrška ne pruža prilagođene skripte u ovoj svrsi.

Postoji zasebni [goo goo](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) za izvoz sadržaja za pojedinačnog korisnika.