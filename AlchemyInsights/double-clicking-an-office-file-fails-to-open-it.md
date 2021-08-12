---
title: Dvostrukim klikom na Kancelarija ne uspeva da se otvori datoteka
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: 519051ac0ffc11d2b17c14959464c1123654bef38d6e10efd252b4ff3d8bbc1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53965115"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a>Dvostrukim klikom na Kancelarija ne uspeva da se otvori datoteka

Kada kliknete dvaput na Kancelarija datoteku, možda ćete videti da je program otvoren, ali se sama datoteka ne otvara. Ili ćete možda dobiti grešku: "Došlo je do problema prilikom slanja komande programu". Postoji mnogo uzroka za ovo, ali dva najčešća rešenja su:

- U okviru Excel, uverite se da je opobložena opcija DDE. Opciju možete pronaći kreiranjem nove radne sveske, a zatim odabiti stavku Datoteka **> Opcije > Napredno**. U **odeljku Opšte** poništite oznaku Zanemari druge aplikacije koje koriste **dinamičke podatke Exchange (DDE).**

- Pokrenite popravku na mreži da biste vratili podrazumevane postavke. Kliknite na dugme Windows Start i potražite stavku "Kontrolna tabla". Otvorite **kontrolnu tablu** i idite na **stavku Programi > Programi i funkcije**. Zatim kliknite desnim tasterom **miša Microsoft kancelarija [Verzija] i** odaberite stavku Promeni > **popravku na mreži.**

Ako nijedno od ovih rešenja ne funkcioniše, kompletniji spisak rešenja možete pronaći u članku podrške, dvostrukim klikom na Kancelarija ne možete da je [otvorite.](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)
