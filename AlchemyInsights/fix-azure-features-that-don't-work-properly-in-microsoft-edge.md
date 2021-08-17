---
title: Šta da radite ako Azure funkcije ne rade ispravno u Microsoft Edge
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: e188ecb375f3d84b45a1a7718b3c0b797c756f822ba64b3824976fe79c1e8298
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54117102"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Šta da radite ako Azure funkcije ne rade ispravno u Microsoft Edge

Microsoft Edge poznate [](https://go.microsoft.com/fwlink/?linkid=2140608) probleme koji su povezani sa bezbednosnim zonama i koji mogu da utiču na to kako se Azure korisnici prijavljivaju u Windows centru aktivnosti. Ako imate problema pri korišćenju Azure funkcija sa Microsoft Edge, isprobajte sledeće korake:

1. U **"Start" meniju** potražite stavku **Internet opcije i** izaberite je.
2. U **dijalogu Internet** svojstva idite na karticu **Bezbednost.**
3. Izaberite **zonu Pouzdani sajtovi,** a zatim kliknite **na dugme** Lokacije.
4. U **dijalogu Pouzdane lokacije** dodajte URL adresu mrežnog prolaza, kao i i [https://login.microsoftonline.com](https://login.microsoftonline.com) , a [https://login.live.com](https://login.live.com) zatim izaberite stavku **Zatvori**.
5. U **dijalogu Internet svojstva** idite na karticu **Privatnost.**
6. U **odeljku Blokator iskačućih** prozora **izaberite stavku Postavke.** U dijalogu koji se otvori dodajte URL adresu mrežnog prolaza, kao i [https://login.microsoftonline.com](https://login.microsoftonline.com) [https://login.live.com](https://login.live.com) i , a zatim izaberite stavku **Zatvori**.
