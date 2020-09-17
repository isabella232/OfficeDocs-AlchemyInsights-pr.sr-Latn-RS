---
title: 1065 deprekacija EOP izlazne IP adrese rangesMC146155
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
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806809"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Razotkrivanje EOP izlaznih opsega IP adresa

Otkrili smo potencijalni problem sa organizacijom koja (ako nije ispravljena do 26 oktobra, 2018) može da prekine protok pošte na lokalno ili spoljne destinacije. Kao što je prethodno bilo vezano za pojednostavljivanje upravljanja mrežnim adresama, konsolidovamo opsege IP adresa Exchange online Protection (EOP) koji se koriste za slanje i primanje e-pošte izvan lokacije Microsoft 365. Naša analiza pokazuje da jedan ili više spoljnih izvora e-pošte ili odredišta koje ste konfigurisali u konektorima za slanje pošte ne prihvataju veze iz opsega IP adresa prikazanih [ovde](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Uradite pre 26 oktobra da biste se uverili da će ovi izvori i destinacije prihvatiti veze ka i od svih [objavljenih EOP IP adresa](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Za više informacija o ovoj promeni pogledajte članak centar za poruke [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)ili [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Napomena**: Ako ste prethodno koristili IP ili URL OBJAVLJIVANJE preko HTML, XML i RSS za ispravke krajnjih tačaka, trebalo bi da migrirate i na nove Veb usluge za automatizovanje ovih tipova ispravki. Više informacija potražite u članku [microsoft 365 krajnje tačke i microsoft 365 IP adresa i URL Veb usluge](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
