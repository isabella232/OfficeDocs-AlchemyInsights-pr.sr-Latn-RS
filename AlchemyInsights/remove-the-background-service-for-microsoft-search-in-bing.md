---
title: Uklanjanje usluge pozadine za Microsoft Search u usluzi Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816336"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a><span data-ttu-id="a0d63-102">Uklanjanje usluge pozadine za Microsoft Search u usluzi Bing</span><span class="sxs-lookup"><span data-stu-id="a0d63-102">Remove the background service for Microsoft Search in Bing</span></span>

<span data-ttu-id="a0d63-103">Da biste uklonili uslugu pozadine za Microsoft Search u usluzi Bing, možete da probate sledeće lekove:</span><span class="sxs-lookup"><span data-stu-id="a0d63-103">To remove the background service for Microsoft Search in Bing, you can try the following remedies:</span></span>

1. <span data-ttu-id="a0d63-104">Da biste se vratili na originalne postavke mašine za pretraživanje, uradite sledeće:</span><span class="sxs-lookup"><span data-stu-id="a0d63-104">To revert to the original search engine settings, do the following things:</span></span>

    <span data-ttu-id="a0d63-105">Neko.</span><span class="sxs-lookup"><span data-stu-id="a0d63-105">a.</span></span> <span data-ttu-id="a0d63-106">Prebacite na **opciju koristi Bing kao podrazumevani [prekidač](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) za pretraživanje**.</span><span class="sxs-lookup"><span data-stu-id="a0d63-106">Switch the **Use Bing as your default search engine [toggle](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Off**.</span></span>

    <span data-ttu-id="a0d63-107">-.</span><span class="sxs-lookup"><span data-stu-id="a0d63-107">b.</span></span> <span data-ttu-id="a0d63-108">[Idite u Microsoft 365 centar administracije](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) i opozovite izbor u okviru podešavanja koja utiče na sve korisnike u organizaciji.</span><span class="sxs-lookup"><span data-stu-id="a0d63-108">[Go to the Microsoft 365 admin center](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) and clear the setting that affects all users in your organization.</span></span>

2. <span data-ttu-id="a0d63-109">Da biste uklonili trenutnu uslugu sa pojedinačnih uređaja, uradite sledeće:</span><span class="sxs-lookup"><span data-stu-id="a0d63-109">To remove the background service from an individual device, do the following tasks:</span></span>

    <span data-ttu-id="a0d63-110">Neko.</span><span class="sxs-lookup"><span data-stu-id="a0d63-110">a.</span></span> <span data-ttu-id="a0d63-111">Odaberite **kontrolnu tablu > programe > programima i funkcijama**.</span><span class="sxs-lookup"><span data-stu-id="a0d63-111">Choose **Control Panel > Programs > Programs and Features**.</span></span>

    <span data-ttu-id="a0d63-112">-.</span><span class="sxs-lookup"><span data-stu-id="a0d63-112">b.</span></span> <span data-ttu-id="a0d63-113">Kliknite desnim tasterom miša na **Microsoft Search u usluzi Bing** ispod liste instaliranih programa, a zatim kliknite na dugme **Deinstaliraj**.</span><span class="sxs-lookup"><span data-stu-id="a0d63-113">Right-click **Microsoft Search in Bing** under the list of installed programs, and then click **Uninstall**.</span></span>

3. <span data-ttu-id="a0d63-114">Da biste uklonili trenutnu uslugu sa više uređaja u organizaciji, prijavite se kao administrator i uradite sledeću komandu u skriptama:</span><span class="sxs-lookup"><span data-stu-id="a0d63-114">To remove the background service from multiple devices in your organization, log in as an administrator and run the following command in a script:</span></span> 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
