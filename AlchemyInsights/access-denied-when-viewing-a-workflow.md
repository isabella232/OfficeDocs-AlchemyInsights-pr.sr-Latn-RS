---
title: Access denied when viewing a Workflow
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 2b076ec5dca070555ce51b88631fb6bd619ed9269e59ccc799b23b8b95547c16
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955215"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Access denied when viewing a Workflow

SharePoint 2013 tokovi posla koji pokušaju da pošalju e-poruku u SharePoint grupu mogu da ne uspeju sa porukom o grešci "Pristup nije zabranjen" ako članstvo grupe SharePoint nije postavljeno na Svi.
  
 **Da biste rešili ovaj problem, uradite sledeće:**
  
 1. Dozvolite svima da vide članove SharePoint grupe.
  
 2. Uklonite grupu SharePoint u redu Za ili CC e-poruke.
  
 3. Eksplicitno dodajte korisnike u red "Za" ili "CC" ako u grupi nije moguće promeniti vidljivost članstva SharePoint grupi.
  
Da biste prikazali više detalja, pogledajte [HTTP neovlašćeno na /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  