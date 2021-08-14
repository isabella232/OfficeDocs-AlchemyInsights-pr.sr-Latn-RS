---
title: Automatsko šifrovanje određenih Office 365-poruka
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 8ae1c6853f41790efc3b24a9dc696bccf8385967d8c9219a1200e287e6ce32a1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53949581"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a>Automatsko šifrovanje određenih Office 365-poruka

Poruke koje korisnici šalju određenim spoljnim osobama ili organizacijama možete automatski da šifrujete. Da biste to uradio, izvršite sledeće korake:

1. U centru [Exchange za administaciju odaberite](https://outlook.office365.com/ecp/)stavku **protok pošte > pravila.** 
2. Kliknite na **ikonu Novo (+),** a zatim izaberite stavku Office 365 šifrovanje poruka zaštitu prava **na poruke.**
3. U **2010**, unesite ime pravila, na primer *Šifruj poruke poslate DrToniRamos@gmail.com.*
4. U **e-pošti Primenite** ovo pravilo ako **odaberite stavku > je ova osoba**. 
5. U **prozoru Izbor** članova izaberite ime osobe na koju želite da se primeni pravilo za šifrovanje, a zatim kliknite na dugme **Dodaj**. 
6. Kada završite sa dodavanjem korisnika, kliknite na dugme **U redu.**
7. Pored polja **Uradite sledeće izaberite** stavku **Izaberi jedan.** 
8. U **padajućem meniju RMS predloška** izaberite stavku **Šifruj**, a zatim kliknite na dugme **U redu.** (Ako ne vidite ovu opciju, to znači da vaš plan ne uključuje automatsko šifrovanje. Ali možete da ga dodate!)
9. Odaberite bilo koji opcionalni izbor (odaberite bilo koji opcionalni izbor (od kojih mnoge možete da napravite u ovom trenutku, od kojih mnoge može da bude podrazumevana postavka radi pojednostavljivosti).
10. Kliknite na dugme **Sačuvaj**.

> [!IMPORTANT]
> Uvek možete da se vratite i uredite ovo pravilo kasnije.

Dodatne informacije o kreiranju pravila za šifrovanje potražite u temi Definisanje pravila za protok pošte radi šifrovanja [e-poruka u programu Office 365.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

