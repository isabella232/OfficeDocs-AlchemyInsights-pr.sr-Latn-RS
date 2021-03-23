---
title: Uvoz i izvoz iz usluge Yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037260"
---
# <a name="import-and-export-from-yammer"></a><span data-ttu-id="0e429-102">Uvoz i izvoz iz usluge Yammer</span><span class="sxs-lookup"><span data-stu-id="0e429-102">Import and export from Yammer</span></span>

<span data-ttu-id="0e429-103">**Biste**</span><span class="sxs-lookup"><span data-stu-id="0e429-103">**Import**</span></span>

<span data-ttu-id="0e429-104">Opcije uvoza korisnika se razlikuju u zavisnosti od toga da li je Yammer mreža u [osnovnom režimu za Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)ili ne.</span><span class="sxs-lookup"><span data-stu-id="0e429-104">User-import options vary depending on whether your Yammer network is in [Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), or not.</span></span>

- <span data-ttu-id="0e429-105">**Režim koji nije osnovni**: korisnici mogu da se uvezu u grupe pomoću stavke [Dodaj iz adresara](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (ograničavanje na 100 korisnika) u okviru postavke grupe ili na mrežu pomoću [masovne ispravke](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) u administratoru mreže.</span><span class="sxs-lookup"><span data-stu-id="0e429-105">**Non-Native Mode**: Users can be imported to groups using [Add from Address Book](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limit to 100 users) within group settings, or to the network using [Bulk Update](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) within Network Admin.</span></span>
- <span data-ttu-id="0e429-106">**Osnovni režim**: članstvo u grupi i operacije članstva u mreži treba da se izvršavaju sa [Microsoft 365 administrator administracije](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portala](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)ili pomoću druge Azure AD AD.</span><span class="sxs-lookup"><span data-stu-id="0e429-106">**Native Mode**: Group membership and network membership operations should be performed from the [Microsoft 365 admin portal](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory), or using another Azure AD option.</span></span> <span data-ttu-id="0e429-107">Mreže u osnovnom režimu više nemaju pristup masovne ispravke i drugim funkcijama nasleđa.</span><span class="sxs-lookup"><span data-stu-id="0e429-107">Networks in Native Mode no longer have access to Bulk Update and other legacy features.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="0e429-108">Yammer nikada nije podržavao uvoz sadržaja iz administracije mreže čak i kada je funkcija izvoza podataka korišćena u drugoj mreži.</span><span class="sxs-lookup"><span data-stu-id="0e429-108">Yammer never supported importing content from within Network Admin even when the Data Export feature was used in another network.</span></span> <span data-ttu-id="0e429-109">Sadržaj može ponovo da se knjiži pomoću partnerskih rešenja ili Yammer OSTATAK API-ja.</span><span class="sxs-lookup"><span data-stu-id="0e429-109">Content can be re-posted by partner solutions or the Yammer REST APIs.</span></span>

<span data-ttu-id="0e429-110">**Zno**</span><span class="sxs-lookup"><span data-stu-id="0e429-110">**Export**</span></span>

<span data-ttu-id="0e429-111">[Izvoz mrežnih podataka u okviru administrator mreže](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) omogućava izvoz sadržaja sa Yammer mreža, uključujući poruke i datoteke.</span><span class="sxs-lookup"><span data-stu-id="0e429-111">[Export Network Data within Network Admin](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permits the export of content from Yammer networks, including messages and files.</span></span> <span data-ttu-id="0e429-112">Prilozi mogu da budu izuzetno veliki i prouzrokovaće da se izvoz može značajno popuniti.</span><span class="sxs-lookup"><span data-stu-id="0e429-112">Attachments can be extremely large and will cause exports to take significant time to complete.</span></span> <span data-ttu-id="0e429-113">Preporučujemo da se aktivne mreže izvozi pomoću API-ja za [Izvoz podataka](https://developer.yammer.com/docs/data-export-api) u delovima po danu ili sedmici.</span><span class="sxs-lookup"><span data-stu-id="0e429-113">We recommend that active networks are exported using the [Data Export API](https://developer.yammer.com/docs/data-export-api) in chunks by day or week.</span></span> <span data-ttu-id="0e429-114">Microsoft podrška ne pruža prilagođene skripte u ovoj svrsi.</span><span class="sxs-lookup"><span data-stu-id="0e429-114">Microsoft Support does not provide custom scripts for this purpose.</span></span>

<span data-ttu-id="0e429-115">Postoji zasebni [goo goo](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) za izvoz sadržaja za pojedinačnog korisnika.</span><span class="sxs-lookup"><span data-stu-id="0e429-115">A separate [GDPR export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) exists to export content for an individual user.</span></span>