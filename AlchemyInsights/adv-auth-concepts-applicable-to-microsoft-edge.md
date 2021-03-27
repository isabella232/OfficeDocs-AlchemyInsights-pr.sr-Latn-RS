---
title: Napredni koncepti potvrde identiteta koji se primenjuju na Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398599"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="c3eee-102">Napredni koncepti potvrde identiteta koji se primenjuju na Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="c3eee-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="c3eee-103">Slede napredni koncepti potvrde identiteta koji se primenjuju na Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="c3eee-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="c3eee-104">**Proaktivna potvrda identiteta**</span><span class="sxs-lookup"><span data-stu-id="c3eee-104">**Proactive Authentication**</span></span>

<span data-ttu-id="c3eee-105">Kada omogućite [smernice ProactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) Microsoft Edge će pokušati da proaktivno potvrdi identitet prijavljenih korisnika putem Microsoft usluga.</span><span class="sxs-lookup"><span data-stu-id="c3eee-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="c3eee-106">U redovnim intervalima koristiće uslugu na mreži da bi proverila ažuriranu manifest koja sadrži konfiguraciju koja upravlja Proaktivnom potvrdom identiteta.</span><span class="sxs-lookup"><span data-stu-id="c3eee-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="c3eee-107">Pogodnosti: Proaktivna potvrda identiteta omogućava potvrdu identiteta ključnim uslugama, kao što je stranica "Nova kartica sistema Office".</span><span class="sxs-lookup"><span data-stu-id="c3eee-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="c3eee-108">Takođe, ako se Bing koristi kao pretraživač, Proaktivna potvrda identiteta poboljšava performanse trake adresa i pomaže u generisanju rezultata pretrage personalizovanih prema potrebama vašeg preduzeća.</span><span class="sxs-lookup"><span data-stu-id="c3eee-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="c3eee-109">**Windows Hello CredUI za NTLM potvrdu identiteta**</span><span class="sxs-lookup"><span data-stu-id="c3eee-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="c3eee-110">Ako jedinstveno prijavljivanje (SSO) nije dostupno kada veb lokacija pokuša da se prijavi na korisnika putem NTLM ili Negotiate mehanizma, ova funkcija će omogućiti korisniku da deli OS akredicije sa veb lokacijom i da zadovolji izazov potvrde identiteta korišćenjem Windows Hello cred korisničkog interfejsa.</span><span class="sxs-lookup"><span data-stu-id="c3eee-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="c3eee-111">Ovaj tok prijavljivanje će se pojaviti samo u operativnom sistemu Windows 10 i samo za korisnike koji ne dobijaju SSO tokom NTLM-a ili sporazumnog izazova.</span><span class="sxs-lookup"><span data-stu-id="c3eee-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="c3eee-112">**Korišćenje sačuvanih lozinki za automatsko prijavljivanje**</span><span class="sxs-lookup"><span data-stu-id="c3eee-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="c3eee-113">Korisnici koji čuvaju lozinke u programu Microsoft Edge mogu da omoguće automatsko prijavljivanje na veb lokacije na kojima imaju sačuvane akredicije.</span><span class="sxs-lookup"><span data-stu-id="c3eee-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="c3eee-114">Korisnici mogu da uključe ili isključe ovu funkciju edge://settings/passwords, a vi možete da je konfigurišete u [smernicama menadžera lozinki.](https://go.microsoft.com/fwlink/?linkid=2134622)</span><span class="sxs-lookup"><span data-stu-id="c3eee-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
