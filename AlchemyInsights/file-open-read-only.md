---
title: Otvaranje datoteke samo za čitanje
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: e478572ea82e5ea11bac9fd7eacafb833253235d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813198"
---
# <a name="file-open-read-only"></a><span data-ttu-id="7d697-102">Otvaranje datoteke samo za čitanje</span><span class="sxs-lookup"><span data-stu-id="7d697-102">File open read-only</span></span>

<span data-ttu-id="7d697-103">Možete da otkrijete da se datoteke otvaraju samo za čitanje kada ih otvarate.</span><span class="sxs-lookup"><span data-stu-id="7d697-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="7d697-104">U nekim slučajevima, ovo je radi dodatne bezbednosti, na primer kada otvarate datoteke sa interneta, a u drugim slučajevima to može biti zbog neke postavke koja se može promeniti.</span><span class="sxs-lookup"><span data-stu-id="7d697-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="7d697-105">Evo nekih scenarija gde se datoteka otvara kao samo za čitanje, kao i neki koraci koje možete preduzeti da biste to promenili.</span><span class="sxs-lookup"><span data-stu-id="7d697-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="7d697-106">**Moj antivirusni program uzrokuje otvaranje programa samo za čitanje**</span><span class="sxs-lookup"><span data-stu-id="7d697-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="7d697-107">Neki antivirusni programi vas možda štite od potencijalno nebezbednih datoteka tako što ih otvaraju samo za čitanje.</span><span class="sxs-lookup"><span data-stu-id="7d697-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="7d697-108">Možda ćete morati da se vašoj dobavljaču antivirusne zaštite proverite kako da prilagodite ove postavke.</span><span class="sxs-lookup"><span data-stu-id="7d697-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="7d697-109">BitDefender, na primer, ima sadržaj o dodavanju izuzetka aplikacije ovde: Kako da dodate izuzetke aplikacija ili procesa u [Bitdefender](https://aka.ms/AA6098i)kontrolni centar.</span><span class="sxs-lookup"><span data-stu-id="7d697-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="7d697-110">**Da li su svojstva datoteke podešena na samo za čitanje?**</span><span class="sxs-lookup"><span data-stu-id="7d697-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="7d697-111">Svojstva datoteke možete da proverite tako što ćete kliknuti desnim tasterom miša na datoteku i izabrati stavku Svojstva.</span><span class="sxs-lookup"><span data-stu-id="7d697-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="7d697-112">Ako je opotrebio atribut "Samo za čitanje", možete da opozivate ga i kliknete na dugme U redu.</span><span class="sxs-lookup"><span data-stu-id="7d697-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="7d697-113">**Sadržaj je u zaštićenom prikazu**</span><span class="sxs-lookup"><span data-stu-id="7d697-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="7d697-114">Datoteke sa interneta i drugih potencijalno nebezbednih lokacija mogu sadržati viruse, crve ili druge vrste malvera koji mogu oštećivati vaš računar.</span><span class="sxs-lookup"><span data-stu-id="7d697-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="7d697-115">Ovo je takođe često slučaj sa prilozima e-pošte ili preuzetim datotekama.</span><span class="sxs-lookup"><span data-stu-id="7d697-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="7d697-116">Radi zaštite računara, datoteke sa ovih potencijalno nebezbednih lokacija otvaraju se u zaštićenom prikazu.</span><span class="sxs-lookup"><span data-stu-id="7d697-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="7d697-117">Pomoću zaštićenog prikaza možete čitati datoteku i videti njen sadržaj umanjujući rizike.</span><span class="sxs-lookup"><span data-stu-id="7d697-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="7d697-118">Više informacija o zaštićenom prikazu i o tome kako da promenite postavke potražite u ovom članku: [Šta je to zaštićeni prikaz?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="7d697-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="7d697-119">**Da li je OneDrive pun?**</span><span class="sxs-lookup"><span data-stu-id="7d697-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="7d697-120">Ako je datoteka uskladištena u usluzi OneDrive i OneDrive prostor za skladištenje je pun, nećete moći da sačuvate dokument dok ne budete pod prepunjenim prostorom.</span><span class="sxs-lookup"><span data-stu-id="7d697-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="7d697-121">Možete da proverite slobodan prostor u usluzi OneDrive tako što ćete kliknuti na OneDrive ikonu u centru za obaveštenja i izabrati stavku Upravljanje skladištem, a možete i da odete na , prijavite se i zanemarite količinu iskorišćenog prostora u donjem levom delu [https://onedrive.live.com](https://onedrive.live.com) ekrana.</span><span class="sxs-lookup"><span data-stu-id="7d697-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="7d697-122">**Da li je Office aktiviran?**</span><span class="sxs-lookup"><span data-stu-id="7d697-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="7d697-123">Ako Office nije aktiviran ili ako je pretplata istekla, možda ste u režimu samo za čitanje smanjene funkcionalnosti.</span><span class="sxs-lookup"><span data-stu-id="7d697-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="7d697-124">Informacije o tome kako da aktivirate Office potražite u: Greške [sa nelicenciranim proizvodom i aktivaciju u programu Office.](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)</span><span class="sxs-lookup"><span data-stu-id="7d697-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="7d697-125">**Ako ništa ne uspe...**</span><span class="sxs-lookup"><span data-stu-id="7d697-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="7d697-126">Pokušajte da ponovo pokrenete računar</span><span class="sxs-lookup"><span data-stu-id="7d697-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="7d697-127">Instaliranje ispravki za Office</span><span class="sxs-lookup"><span data-stu-id="7d697-127">Install Office updates</span></span>
    
- <span data-ttu-id="7d697-128">Obavljanje popravke na mreži sistema Office</span><span class="sxs-lookup"><span data-stu-id="7d697-128">Perform an Online repair of Office</span></span>
    

