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
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="5883d-102">Razotkrivanje EOP izlaznih opsega IP adresa</span><span class="sxs-lookup"><span data-stu-id="5883d-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="5883d-103">Otkrili smo potencijalni problem sa organizacijom koja (ako nije ispravljena do 26 oktobra, 2018) može da prekine protok pošte na lokalno ili spoljne destinacije.</span><span class="sxs-lookup"><span data-stu-id="5883d-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="5883d-104">Kao što je prethodno bilo vezano za pojednostavljivanje upravljanja mrežnim adresama, konsolidovamo opsege IP adresa Exchange online Protection (EOP) koji se koriste za slanje i primanje e-pošte izvan lokacije Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="5883d-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="5883d-105">Naša analiza pokazuje da jedan ili više spoljnih izvora e-pošte ili odredišta koje ste konfigurisali u konektorima za slanje pošte ne prihvataju veze iz opsega IP adresa prikazanih [ovde](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="5883d-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="5883d-106">Uradite pre 26 oktobra da biste se uverili da će ovi izvori i destinacije prihvatiti veze ka i od svih [objavljenih EOP IP adresa](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="5883d-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="5883d-107">Za više informacija o ovoj promeni pogledajte članak centar za poruke [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)ili [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="5883d-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="5883d-108">**Napomena**: Ako ste prethodno koristili IP ili URL OBJAVLJIVANJE preko HTML, XML i RSS za ispravke krajnjih tačaka, trebalo bi da migrirate i na nove Veb usluge za automatizovanje ovih tipova ispravki.</span><span class="sxs-lookup"><span data-stu-id="5883d-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="5883d-109">Više informacija potražite u članku [microsoft 365 krajnje tačke i microsoft 365 IP adresa i URL Veb usluge](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="5883d-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
