---
title: Sporni problemi sa prijavljivanjem za SSO korisnika
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
- "9004357"
- "7811"
ms.openlocfilehash: 347ef8f8176583f2a7c15fa82435eeb118b58c39
ms.sourcegitcommit: 67c873fa6e23ec39a826d60ac830969073bf79e1
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935180"
---
# <a name="seamless-sso-user-sign-in-issues"></a>Sporni problemi sa prijavljivanjem za SSO korisnika

Kada se korisnik potvrdi, pregledač će keširati korisničke akreditive, tako da se u istom pregledaču, aplikacija automatski prijavi sa istim nalogom. To može otežati drugom korisniku ili jednom korisniku da se prijavi na više naloga na jednom uređaju. Da biste rešili ovo: 1. Pokušajte da se prijavite u drugom pregledaču. 2. Opozovite izbor keširanja pregledača i/ili kolačića i pokušajte ponovo da se prijavite.

Ako i dalje imate problema sa prijavljivanjem, preporučujemo sledeće da biste dijagnostikovali i automatizovali korake rezolucije:

1. Instalirajte [bezbednu oznaku pregledača "moje aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) " da biste pomogli Azure Active Directory (AZURE AD) da poboljšate dijagnozu i rezolucije kada koristite testiranje na Azure stranici.
2. Reprodukuju grešku koristeći testiranje iskustva na stranici "Konfigurisanje aplikacije" na Azure portalu. Da biste saznali više, pogledajte članak [otklanjanje grešaka za pojedinačne aplikacije za prijavljivanje u okviru seml](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues).
3. Ako koristite testiranje iskustva na Azure sajtu pomoću bezbednog pregledača "moje aplikacije", možete da **preskočite broj 4**.
4. Da biste otvorili stranicu za konfiguraciju jedinstvenog prijavljivanja na osnovu SAML-a:
    - Otvorite [Azure portal](https://portal.azure.com/) i prijavite se kao **globalni administrator** ili **koadministrator**.
    - Otvorite **Azure Active Directory oznaku** tako što ćete izabrati **sve usluge** na vrhu glavnog menija za navigaciju levo.
    - U polju za pretragu filtera otkucajte "Azure Active Directory" i izaberite stavku **Azure Active Directory stavka kataloga** .
    - Izaberite stavku **Enterprise aplikacije** iz levog direktorijuma "Azure Active Directory".
    - Izaberite **sve aplikacije** da biste prikazali listu svih aplikacija. Ako ne vidite aplikaciju koju želite da prikažete ovde, koristite kontrolu **filtriranja** na vrhu **liste svi aplikacije** i podesite opciju **Prikaži** na **sve aplikacije**.
    - Izaberite aplikaciju koju želite da konfigurišete za jedinstveno prijavljivanje.
    - Kada se aplikacija učita, izaberite stavku **jedinstveno prijavljivanje** iz menija aplikacije za levi navigacija.
    - Izaberite stavku **Seml-ski SSO**.
5. Na osnovu ove greške, da biste saznali više o preporučenim koracima koji treba da se slede, pogledajte članak [problemi sa prijavljivanjem na pojedinačne aplikacije podešene za jednokratnu prijavljivanje](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory).
6. Da biste rešili probleme sa drugim korisnicima korisnika, Pogledajte sledeća uputstva:
    - [Single Sign-On SEML protokola](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
    - [Kako da: rešite probleme sa prijavljivanjem pomoću Azure Active Directory izveštaja](https://docs.microsoft.com/azure/active-directory/reports-monitoring/howto-troubleshoot-sign-in-errors)
    - [Neočekivani odziv sa odobravama](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)
    - [Greška u saglasnosti korisnika](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
    - [Problemi sa prijavljivanjem iz aplikacija](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)
    - [Greška na stranici za prijavljivanje aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
    - [Problem sa prijavljivanjem u Microsoft aplikaciju](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)
