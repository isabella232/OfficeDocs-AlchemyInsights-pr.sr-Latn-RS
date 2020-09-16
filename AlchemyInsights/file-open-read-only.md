---
title: Otvori datoteku samo za čitanje
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 2fdb4f048c2bee022a49c2cca2ce9770f42a87a2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745621"
---
# <a name="file-open-read-only"></a><span data-ttu-id="9a243-102">Otvori datoteku samo za čitanje</span><span class="sxs-lookup"><span data-stu-id="9a243-102">File open read-only</span></span>

<span data-ttu-id="9a243-103">Možete otkriti da se one otvaraju samo za čitanje kada otvarate datoteke.</span><span class="sxs-lookup"><span data-stu-id="9a243-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="9a243-104">U nekom slučaju, ovo je za dodatnu bezbednost, na primer kada otvarate datoteke sa interneta, a drugi put to može da bude zbog podešavanja koja se može promeniti.</span><span class="sxs-lookup"><span data-stu-id="9a243-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="9a243-105">Evo nekih scenarija kada se datoteka otvara samo za čitanje i neke korake koje možete preduzeti da biste to promenili.</span><span class="sxs-lookup"><span data-stu-id="9a243-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="9a243-106">**Antivirus me izaziva da otvori samo za čitanje**</span><span class="sxs-lookup"><span data-stu-id="9a243-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="9a243-107">Neki antivirusni programi mogu da vas zaštite od potencijalno nebezbednih datoteka tako što ćete ih otvoriti samo za čitanje.</span><span class="sxs-lookup"><span data-stu-id="9a243-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="9a243-108">Možda ćete morati da se obratite dobavljaču virusa da biste saznali kako da prilagodite ove postavke.</span><span class="sxs-lookup"><span data-stu-id="9a243-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="9a243-109">BitDefender, na primer, ima sadržaj na dodavanju isključenja aplikacija ovde: [Kako da dodate isključivanja aplikacije ili procesa u centar za kontrolisanje BitDefender](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="9a243-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="9a243-110">**Da li su svojstva datoteke postavljena samo za čitanje?**</span><span class="sxs-lookup"><span data-stu-id="9a243-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="9a243-111">Možete da potvrdite svojstva datoteke tako što ćete kliknuti desnim tasterom miša na datoteku i izabrati svojstva.</span><span class="sxs-lookup"><span data-stu-id="9a243-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="9a243-112">Ako je potvrđen izbor u kom se atribut samo za čitanje proverava, možete da je opozovete i kliknete na dugme u redu.</span><span class="sxs-lookup"><span data-stu-id="9a243-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="9a243-113">**Sadržaj je u zaštićenom prikazu**</span><span class="sxs-lookup"><span data-stu-id="9a243-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="9a243-114">Datoteke sa interneta i iz drugih potencijalno nebezbednih lokacija mogu da sadrže viruse, crve ili druge vrste malvera koje mogu da ugroze računar.</span><span class="sxs-lookup"><span data-stu-id="9a243-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="9a243-115">Ovo je takođe najčešće slučaj sa prilozima e-pošte ili datotekama koje ste preuzeli.</span><span class="sxs-lookup"><span data-stu-id="9a243-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="9a243-116">Da biste zaštitili računar, datoteke sa ovih potencijalno nebezbednih lokacija otvaraju se u zaštićenom prikazu.</span><span class="sxs-lookup"><span data-stu-id="9a243-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="9a243-117">Pomoću zaštićenog prikaza možete da pročitate datoteku i vidite njen sadržaj dok umanjujete rizike.</span><span class="sxs-lookup"><span data-stu-id="9a243-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="9a243-118">Više informacija o zaštićenom prikazu i načinu promene postavki potražite u članku: [Šta je to zaštićeni prikaz?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="9a243-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="9a243-119">**Da li je OneDrive pun?**</span><span class="sxs-lookup"><span data-stu-id="9a243-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="9a243-120">Ako se datoteka skladišti u usluzi OneDrive i ako je OneDrive prostor za skladištenje pun, nećete moći da sačuvate dokument dok se ne nalazite u okviru dodeljenog prostora.</span><span class="sxs-lookup"><span data-stu-id="9a243-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="9a243-121">Možete da potvrdite svoj besplatan prostor u usluzi OneDrive tako što ćete kliknuti na ikonu OneDrive na traci obaveštenja i izabrati stavku Upravljanje skladištenjem ili možete otići na [https://onedrive.live.com](https://onedrive.live.com) Prijavljivanje i primetiti količinu korišćenog prostora u donjem levom delu ekrana.</span><span class="sxs-lookup"><span data-stu-id="9a243-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="9a243-122">**Da li je Office aktiviran?**</span><span class="sxs-lookup"><span data-stu-id="9a243-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="9a243-123">Ako Office nije aktiviran ili ako je pretplata istekla, možete da budete u režimu umanjenog samo za čitanje.</span><span class="sxs-lookup"><span data-stu-id="9a243-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="9a243-124">Informacije o tome kako da aktivirate Office potražite u članku: [nelicencirane greške proizvoda i aktivacije u sistemu Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="9a243-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="9a243-125">**Ako sve drugo propadne...**</span><span class="sxs-lookup"><span data-stu-id="9a243-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="9a243-126">Pokušajte da ponovo pokrenete računar</span><span class="sxs-lookup"><span data-stu-id="9a243-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="9a243-127">Instaliranje Office ispravki</span><span class="sxs-lookup"><span data-stu-id="9a243-127">Install Office updates</span></span>
    
- <span data-ttu-id="9a243-128">Obavljanje sistema Office na mreži</span><span class="sxs-lookup"><span data-stu-id="9a243-128">Perform an Online repair of Office</span></span>
    

