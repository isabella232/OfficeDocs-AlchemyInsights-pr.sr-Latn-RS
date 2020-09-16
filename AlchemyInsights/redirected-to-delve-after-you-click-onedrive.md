---
title: OneDrive for Business Veb OneDrive preusmerava na Delve
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: faa2cf25270a3b74a12aeb63d23ce98b51e13cb6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47776394"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="3c212-102">Preusmereno na Delve kada kliknete na OneDrive</span><span class="sxs-lookup"><span data-stu-id="3c212-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="3c212-103">Pogledajte naš detaljan [Vodič za rešavanje problema](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span><span class="sxs-lookup"><span data-stu-id="3c212-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="3c212-104">Da biste rešili ovaj problem, administrator mora korisnicima da dodeli pravo da kreiraju svoje lokacije "Moji Veb lokacije".</span><span class="sxs-lookup"><span data-stu-id="3c212-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="3c212-105">To je zato što se na mojim sajtovima kreiraju OneDrive for Business stranica.</span><span class="sxs-lookup"><span data-stu-id="3c212-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="3c212-106">Da biste ovo ispravno dodelili, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="3c212-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="3c212-107">U SharePoint centru administracije izaberite stavku **korisnički profili**.</span><span class="sxs-lookup"><span data-stu-id="3c212-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="3c212-108">U odeljku **osobe** izaberite stavku **Upravljanje dozvolama korisnika**.</span><span class="sxs-lookup"><span data-stu-id="3c212-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="3c212-109">Dodajte korisnike koji zahtevaju dozvole za kreiranje lokacije mojih lokacija.</span><span class="sxs-lookup"><span data-stu-id="3c212-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="3c212-110">Ova postavka podrazumevano se podešava **svima osim spoljnim korisnicima**.</span><span class="sxs-lookup"><span data-stu-id="3c212-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="3c212-111">Kada dodate korisnika, korisnike ili grupu, uverite se da je izabran korisnik, korisnici ili grupa, idite u odeljak **dozvole** , a zatim potvrdite izbor u polju za potvrdu pored stavke **Kreiraj ličnu stranicu (obavezno za lično skladište, feed za vesti i praćene sadržaje)**.</span><span class="sxs-lookup"><span data-stu-id="3c212-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="3c212-112">Kliknite na dugme **u redu**, a zatim neka korisnik Potraži OneDrive stranicu da bi kreirao lokaciju.</span><span class="sxs-lookup"><span data-stu-id="3c212-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
