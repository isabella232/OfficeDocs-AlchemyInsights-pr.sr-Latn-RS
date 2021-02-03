---
title: Promena postavki EWS ograničavanja
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: 4f0bea884153dc1ed8699ce12e0d017d18f5e57c
ms.sourcegitcommit: 53e5caab697ebfb434ccef3ef98b8f2bee579b41
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 02/02/2021
ms.locfileid: "50075911"
---
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="a3423-102">Promena postavki EWS ograničavanja</span><span class="sxs-lookup"><span data-stu-id="a3423-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="a3423-103">Pokrenite automatizovani test koji će vam omogućiti da izmenite smernice EWS ograničavanja tokom migracije.</span><span class="sxs-lookup"><span data-stu-id="a3423-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="a3423-104">Imajte na umu da čak i nakon ovog pokretanje EWS uvoz će i dalje biti ograničen na 150 MB na 5 minuta po poštanskom sandučetu. Da biste postigli veću brzinu preuzimanja migracije, migrirajte više korisnika istovremeno.</span><span class="sxs-lookup"><span data-stu-id="a3423-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="a3423-105">Imajte na umu da promene smernica EWS ograničavanja ne utiču na sledeće tipove migracije (pomoću Microsoft alatki): hibridna, potpuna/fazna (RPC/HTTP), IMAP, G Suite, javna fascikla ili usluga PST uvoza.</span><span class="sxs-lookup"><span data-stu-id="a3423-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>