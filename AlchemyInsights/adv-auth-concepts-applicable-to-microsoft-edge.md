---
title: Napredni koncepti autentičnosti primenljiv na Microsoft Edge
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
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573529"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="4a334-102">Napredni koncepti autentičnosti primenljiv na Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="4a334-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="4a334-103">Slede Napredni koncepti autentičnosti koji se primenjuju na Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="4a334-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="4a334-104">**Proaktivna potvrda identiteta**</span><span class="sxs-lookup"><span data-stu-id="4a334-104">**Proactive Authentication**</span></span>

<span data-ttu-id="4a334-105">Kada omogućite smernice za [Proactiveda](https://go.microsoft.com/fwlink/?linkid=2134621) , Microsoft Edge će pokušati da produzi potvrdu o prijavljivanju korisnika u Microsoft usluge.</span><span class="sxs-lookup"><span data-stu-id="4a334-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="4a334-106">U redovnim intervalima, ona će koristiti uslugu na mreži za proveru ažuriranog manifesta koji sadrži trenutnu potvrdu konfiguracije.</span><span class="sxs-lookup"><span data-stu-id="4a334-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="4a334-107">Beneficije: proaktivna potvrda identiteta omogućava potvrdu identiteta na ključnim uslugama, kao što je stranica Office nova kartica.</span><span class="sxs-lookup"><span data-stu-id="4a334-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="4a334-108">Takođe, ako se Bing koristi kao pretraživač, proaktivna potvrda identiteta poboljšava performanse trake adresa i pomaže pri generisanje rezultata pretrage personalizovanih na potrebe preduzeća.</span><span class="sxs-lookup"><span data-stu-id="4a334-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="4a334-109">**Windows Hello Kredui za NTLM potvrdu identiteta**</span><span class="sxs-lookup"><span data-stu-id="4a334-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="4a334-110">Ako je pojedinačni prijavljivanje (SSO) nije dostupan kada Veb lokacija pokuša da se prijavi na korisnika kroz NTLM ili pregovaranje mehanizma, ova funkcija će korisniku omogućiti da deli akreditive OS sa Veb lokacijom i da bi ispunila izazov potvrde identiteta pomoću Windows Hello Ccrveni UI.</span><span class="sxs-lookup"><span data-stu-id="4a334-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="4a334-111">Ovaj tok prijavljivanja pojaviće se samo u operativnom sistemu Windows 10 i samo za korisnike koji ne primaju SSO tokom NTLM ili pregovaranja.</span><span class="sxs-lookup"><span data-stu-id="4a334-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="4a334-112">**Korišćenje sačuvanih lozinki za automatsko prijavljivanje**</span><span class="sxs-lookup"><span data-stu-id="4a334-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="4a334-113">Korisnici koji čuvaju lozinke u aplikaciji Microsoft Edge mogu da omoguću automatsko prijavljivanje na Veb lokacije na kojima imaju sačuvane akreditive.</span><span class="sxs-lookup"><span data-stu-id="4a334-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="4a334-114">Korisnici mogu da uključe ovu funkciju u edge://settings/passwords i da je konfigurišete u smernicama [upravljača lozinkama](https://go.microsoft.com/fwlink/?linkid=2134622) .</span><span class="sxs-lookup"><span data-stu-id="4a334-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
