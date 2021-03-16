---
title: Uklanjanje usluge pozadine za Microsoft Search u usluzi Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816336"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a>Uklanjanje usluge pozadine za Microsoft Search u usluzi Bing

Da biste uklonili uslugu pozadine za Microsoft Search u usluzi Bing, možete da probate sledeće lekove:

1. Da biste se vratili na originalne postavke mašine za pretraživanje, uradite sledeće:

    Neko. Prebacite na **opciju koristi Bing kao podrazumevani [prekidač](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) za pretraživanje**.

    -. [Idite u Microsoft 365 centar administracije](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) i opozovite izbor u okviru podešavanja koja utiče na sve korisnike u organizaciji.

2. Da biste uklonili trenutnu uslugu sa pojedinačnih uređaja, uradite sledeće:

    Neko. Odaberite **kontrolnu tablu > programe > programima i funkcijama**.

    -. Kliknite desnim tasterom miša na **Microsoft Search u usluzi Bing** ispod liste instaliranih programa, a zatim kliknite na dugme **Deinstaliraj**.

3. Da biste uklonili trenutnu uslugu sa više uređaja u organizaciji, prijavite se kao administrator i uradite sledeću komandu u skriptama: 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
