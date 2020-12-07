---
title: Šta da radite ako Azure funkcije ne funkcionišu ispravno u usluzi Microsoft Edge
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
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583784"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Šta da radite ako Azure funkcije ne funkcionišu ispravno u usluzi Microsoft Edge

Microsoft Edge ima [poznate probleme](https://go.microsoft.com/fwlink/?linkid=2140608) koji su povezani sa bezbednosnim zonama i koji možda utiču na to kako se Azure korisnici prijavljuju u Windows centar administracije. Ako imate problema prilikom korišćenja Azure funkcija sa Microsoft Edge, Isprobajte sledeće korake:

1. U meniju **Start** potražite **Internet opcije** i izaberite je.
2. U dijalogu **Svojstva Internet** izaberite karticu **bezbednost** .
3. Izaberite zonu **pouzdanih lokacija** , a zatim izaberite dugme **lokacije** .
4. U dijalogu **pouzdane lokacije** Dodajte URL adrese mrežnog prolaza [https://login.microsoftonline.com](https://login.microsoftonline.com) i [https://login.live.com](https://login.live.com) , a zatim kliknite na dugme **Zatvori**.
5. U dijalogu **Internet Svojstva** idite na karticu **Privatnost** .
6. U odeljku **blokator iskačućih prozora** izaberite stavku **Postavke**. U dijalogu koji se otvara Dodajte URL adrese mrežnog prolaza [https://login.microsoftonline.com](https://login.microsoftonline.com) i [https://login.live.com](https://login.live.com) , a zatim kliknite na dugme **Zatvori**.
