---
title: Rešavanje problema sa umanjeno zasnovanim na OIDC-u na osnovu jedinstvenog prijavljivanja (SSO)
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9375"
ms.openlocfilehash: e4ddde6176d9ab021b93e23b3cb363e10b1c1048
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747129"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>Rešavanje problema sa umanjeno zasnovanim na OIDC-u na osnovu jedinstvenog prijavljivanja (SSO)

- Da biste saznali kako da dodate OIDC aplikaciju na osnovu Azure zakupca, pogledajte program [Quickstart: podešavanje OIDC-a za jedinstveno prijavljivanje (SSO) za aplikaciju u Azure Active Directory programu (AZURE AD) zakupcu](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso).
- Više detalja o aplikacijama koje koriste standard OpenID Connect za primenu jedinstvenog prijavljivanja potražite u članku [razumevanje jedinstvenog prijavljivanja na zasnovan na OIDC-u](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on).
- Za informacije u slučaju da odaberete da napišete kôd putem direktnog slanja i rukovanja HTTP zahtevima ili korišćenja nezavisne biblioteke iz otvorenog izvora, umesto da koristite neku od naših otvorenih biblioteka, pogledajte članak [OAuth 2,0 i OpenID Poveži protokole na Microsoft platformi za identifikaciju](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols).

**Protokoli**

1. [Microsoft Platform identiteta i implicitni protok](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) – odredjena karakteristika implicitne pomoći je da su simboli (ID-ovi ili Access tokena) vraćeni direktno sa krajnjih krajnjih tačaka umesto krajnje tačke/Token. To se često koristi kao deo toka autorski kôd, u onom što se zove **"hibridni protok" – preuzimanje SIMBOLA ID-a na/autorizaciji zajedno sa kodom za autorizaciju**. Ovaj članak opisuje kako da se direktno programira u odnosu na protokol u aplikaciji da bi zahtevali Tokene iz usluge Azure AD.
2. [Microsoft Access platforma za identifikaciju i oauth 2,0 tok autorskih kodova](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) – kôd oauto 2,0 Grant može da se koristi u aplikacijama koje su instalirane na uređaju da bi dobili pristup zaštićenim resursima, kao što je Veb Apis. Korišćenje Microsoft platforme za primenu identiteta u usluzi 2,0, možete da **dodate pristup prijavljivanju i API-ju mobilnim i aplikacijama za stone računare**. Ovaj članak opisuje kako se direktno programira protokol u aplikaciji pomoću bilo kog jezika.
3. [Microsoft protokol za primenu identiteta i openid](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) – kada koristite primenu Openid povezivanja Microsoft identiteta, možete da dodate pristup prijavljivanju i API-ju u aplikacije. Ovaj članak pokazuje kako se to radi nezavisno od jezika i opisuje kako se **šalju i primaju HTTP poruke bez upotrebe bilo koje Microsoft Open-izvorne biblioteke**.
4. [Microsoft Platform identiteta i oauth 2,0 akreditivi za klijentske akreditive](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) – možete da koristite nalog "oauth 2,0 Client akreditivi koji je naveden u programu rfc 6749, koji se ponekad naziva **dva-noћna** potvrda o pristupu Veb hostovanih veb sadržaja pomoću identiteta aplikacije. Ovaj tip pomoći najčešće se koristi za interakcije servera-to-servera koje moraju da se pokreću u pozadini, bez trenutne interakcije sa korisnikom. Ovi tipovi aplikacija se često nazivaju " **demonskom** ili **nalozima usluga**". Ovaj članak opisuje kako se direktno programira protokol u aplikaciji.
