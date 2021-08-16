---
title: 1065 ukidanje opsega EOP odlaznih IP adresaMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 214abc57a99c70a02a7d159441713e007f6ad980f67e373780d4ca297f69f764
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031276"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Ukidanje opsega EOP odlaznih IP adresa

Otkrili smo potencijalni problem sa vašom organizacijom koji (ako to nije ispravljeno do 26. oktobra 2018.) može da prekine protok pošte na vaše lokacije ili spoljna odredišta. Kako smo ranije komunicirali, da bismo pojednostavili upravljanje opsegom IP adresa, konsolidujemo opsege IP adresa usluge Exchange Online Protection (EOP) koji se koriste za slanje i prijem e-pošte izvan Microsoft 365. Naša analiza ukazuje na to da neki spoljni izvori e-pošte ili odredišta koje ste konfigurisali u konektorima protoka pošte ne prihvataju veze iz opsega IP adresa prikazanih [ovde.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

Predlažemo vam pre 26. oktobra da biste se uverili da će ti izvori i odredišta prihvatiti veze sa svim objavljenim [EOP IP adresama i](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)sa njih.

Dodatne informacije o ovoj promeni potražite u porukama u Centru za poruke [MC146155,](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155) [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)ili [MC149274.](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)

Naznaka: Ako ste ranije koristili objavljivanje IP ili URL adrese putem HTML, XML-a i RSS-a za ispravke krajnje **tačke,** trebalo bi da migrirate u nove veb usluge da biste automatizovali ove tipove ispravki. Dodatne informacije potražite u Microsoft 365 kategorija krajnjih tačkih tačkih podataka i Microsoft 365 IP adresa i [veb-usluga URL adrese.](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)
