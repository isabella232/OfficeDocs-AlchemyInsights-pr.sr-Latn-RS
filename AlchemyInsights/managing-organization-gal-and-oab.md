---
title: Upravljanje globalnim spiskom adresa organizacije i vanmrežnim adresarom
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002895"
- "5550"
ms.openlocfilehash: c6ad2fcb85ef68c42cea11ebe0d1564e957b4720
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51794846"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a><span data-ttu-id="d009b-102">Upravljanje globalnim spiskom adresa (GAL) organizacije i vanmrežnim adresarom (OAB)</span><span class="sxs-lookup"><span data-stu-id="d009b-102">Managing organization global address list (GAL) and offline address book (OAB)</span></span>

<span data-ttu-id="d009b-103">Globalni spisak adresa (GAL) jeste lista objekata omogućenih za poštu (bilo koji tip primaoca koji može da prima e-poštu) u organizaciji.</span><span class="sxs-lookup"><span data-stu-id="d009b-103">A global address list (GAL) is a list of mail-enabled objects (any type of recipient that can receive an email) in the organization.</span></span> <span data-ttu-id="d009b-104">Jedan GAL se automatski kreira u svakoj organizaciji.</span><span class="sxs-lookup"><span data-stu-id="d009b-104">One GAL is automatically created in every organization.</span></span> <span data-ttu-id="d009b-105">Dodatni GAL možete da kreirate da biste razdvojili korisnike po organizaciji ili lokaciji, ali jedan korisnik može da vidi i koristi samo jedan GAL odjednom.</span><span class="sxs-lookup"><span data-stu-id="d009b-105">You can create additional GALs to separate users by organization or location, but a single user can only see and use one GAL at a time.</span></span>

<span data-ttu-id="d009b-106">Neki klijenti e-pošte, kao što je Outlook za Windows, preuzimaju GAL za vanmrežno korišćenje.</span><span class="sxs-lookup"><span data-stu-id="d009b-106">Some email clients, such as Outlook for Windows, download the GAL for offline use.</span></span> <span data-ttu-id="d009b-107">Ovo je poznato kao vanmrežni adresar (OAB).</span><span class="sxs-lookup"><span data-stu-id="d009b-107">This is known as an offline address book (OAB).</span></span> <span data-ttu-id="d009b-108">U sistemu Exchange online, OAB se ažurira samo jednom na svakih 8 časova i onda klijent mora da ga preuzme da bi ažurirao lokalnu OAB kopiju.</span><span class="sxs-lookup"><span data-stu-id="d009b-108">In Exchange online, an OAB is updated only once every 8 hours, and then clients must download it to update their local OAB copy.</span></span> <span data-ttu-id="d009b-109">Svaka promena primaoca prvo mora biti vidljiva u GAL-u, da bi se kasnije mogla pronaći u OAB-u.</span><span class="sxs-lookup"><span data-stu-id="d009b-109">Any recipient change has to first be visible in the GAL to later make it to the OAB.</span></span>

<span data-ttu-id="d009b-110">Evo nekih najčešće korišćenih GAL i OAB procedura:</span><span class="sxs-lookup"><span data-stu-id="d009b-110">Here are some commonly used GAL and OAB procedures:</span></span>

- <span data-ttu-id="d009b-111">Iz različitih razloga, možda ćete želeti da neki objekti budu sakriveni od GAL-a.</span><span class="sxs-lookup"><span data-stu-id="d009b-111">For a variety of reasons, you might want some objects to be hidden from the GAL.</span></span> <span data-ttu-id="d009b-112">Pogledajte odeljak [Sakrivanje primaoca sa spiska adresa](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span><span class="sxs-lookup"><span data-stu-id="d009b-112">Please see [Hide recipients from address lists](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span></span>
- <span data-ttu-id="d009b-113">Ako je potrebno da određenim grupama korisnika date prilagođene prikaze na GAL organizacije, pročitajte članak [Smernice za adresare u sistemu Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span><span class="sxs-lookup"><span data-stu-id="d009b-113">If you need to give specific groups of users customized views of the organization's GAL, see [Address book policies in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span></span>
- <span data-ttu-id="d009b-114">[Kreirajte globalni spisak adresa u sistemu Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) i saznajte kako da radite sa GAL, pročitajte članak [Lista adresa u sistemu Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span><span class="sxs-lookup"><span data-stu-id="d009b-114">[Create a global address list in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) and to learn how to work with GAL permissions, see [Address lists in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span></span> <span data-ttu-id="d009b-115">Imajte u vidu da ako kreirate nove GAL, možda ćete želeti da kreirate i novi OAB.</span><span class="sxs-lookup"><span data-stu-id="d009b-115">Please note that if you create new GALs, you might also want to create a new OAB.</span></span> <span data-ttu-id="d009b-116">Pogledajte [Procedure za](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures)operacije vanmrežnog adresara.</span><span class="sxs-lookup"><span data-stu-id="d009b-116">See [Offline address book procedures](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span></span>
