---
title: Nije podešen nijedan od jabuka MDM Push certifikata
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440012"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a><span data-ttu-id="decc1-102">Nije podešen nijedan od jabuka MDM Push certifikata</span><span class="sxs-lookup"><span data-stu-id="decc1-102">Apple MDM Push Certificate has not been set up</span></span>

<span data-ttu-id="decc1-103">Certifikat "Apple MDM" (poznat i kao Apple) nije konfigurisan za vašu pretplatu.</span><span class="sxs-lookup"><span data-stu-id="decc1-103">An Apple MDM Push Certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured for your subscription.</span></span> <span data-ttu-id="decc1-104">Bez konfigurisanog, Apple MDM Push certifikata, ne možete da se prijavite i upravljate uređajima za iOS i Mac OS.</span><span class="sxs-lookup"><span data-stu-id="decc1-104">Without an Apple MDM Push Certificate configured, you are unable to enroll and manage iOS and Mac OS devices.</span></span> <span data-ttu-id="decc1-105">Kada dodate certifikat u Intune, korisnici mogu da instaliraju aplikaciju "portal Company" kako bi ih upišu.</span><span class="sxs-lookup"><span data-stu-id="decc1-105">After you add the certificate to Intune, users can install the Company Portal app to enroll their iOS devices.</span></span>

1. <span data-ttu-id="decc1-106">Izaberite **"slažem se".**</span><span class="sxs-lookup"><span data-stu-id="decc1-106">Select **"I agree."**</span></span> <span data-ttu-id="decc1-107">da biste dali korporaciji Microsoft dozvolu da šalje podatke u Apple.</span><span class="sxs-lookup"><span data-stu-id="decc1-107">to give Microsoft permission to send data to Apple.</span></span>

2. <span data-ttu-id="decc1-108">Izaberite **Preuzmi svoj CSR** zahtev za potpisivanje potvrda o potpisivanju zahteva za kreiranje certifikata "Apple MDM".</span><span class="sxs-lookup"><span data-stu-id="decc1-108">Select **Download your CSR** the Intune certificate signing request required to create an Apple MDM push certificate.</span></span> <span data-ttu-id="decc1-109">Datoteka se koristi da bi se zahtijevale odnos poverenja sa portala za Push certifikata na Apple.</span><span class="sxs-lookup"><span data-stu-id="decc1-109">The file is used to request a trust relationship certificate from the Apple Push Certificates Portal.</span></span>

3. <span data-ttu-id="decc1-110">Izaberite opciju **Kreiraj vaš MDM Push certifikat** da biste otišli do portala "Push certifikata".</span><span class="sxs-lookup"><span data-stu-id="decc1-110">Select **Create your MDM push Certificate** to go to the Apple Push Certificates Portal.</span></span> <span data-ttu-id="decc1-111">Prijavite se koristeći ID jabuke kompanije, a zatim izaberite stavku **Kreiraj certifikat**.</span><span class="sxs-lookup"><span data-stu-id="decc1-111">Sign in with your company Apple ID, and then select **Create a Certificate**.</span></span> <span data-ttu-id="decc1-112">Izaberite **stavku Odaberi datoteku**, potražite datoteku zahteva za potpisivanje certifikata, a zatim odaberite stavku **Otpremi**.</span><span class="sxs-lookup"><span data-stu-id="decc1-112">Select **Choose File**, browse to the certificate signing request file, and then choose **Upload**.</span></span> <span data-ttu-id="decc1-113">Na stranici za potvrdu izaberite stavku **Preuzmi** da biste preuzeli datoteku certifikata (. Pem) i sačuvajte datoteku lokalno.</span><span class="sxs-lookup"><span data-stu-id="decc1-113">On the Confirmation page, choose **Download** to download the certificate (.pem) file, and save the file locally.</span></span>
 
<span data-ttu-id="decc1-114">**Napomena**: certifikat je pridružen ID-u jabuke koji je korišćen za njegovo kreiranje.</span><span class="sxs-lookup"><span data-stu-id="decc1-114">**Note**: The certificate is associated with the Apple ID used to create it.</span></span> <span data-ttu-id="decc1-115">Kao najbolja praksa, koristite ID kompanije jabuka za zadatke upravljanja i uverite se da poštansko sanduče nadgleda više od jedne osobe ili korišćenjem liste distribucije.</span><span class="sxs-lookup"><span data-stu-id="decc1-115">As a best practice, use a company Apple ID for management tasks, and make sure the mailbox is monitored by more than one person or by using a distribution list.</span></span> <span data-ttu-id="decc1-116">Nikada nemojte koristiti lični ID jabuke.</span><span class="sxs-lookup"><span data-stu-id="decc1-116">Never use a personal Apple ID.</span></span> <span data-ttu-id="decc1-117">Koristite isti ID jabuke da biste obnovili Jabukovo uverenje na svakih 12 meseci.</span><span class="sxs-lookup"><span data-stu-id="decc1-117">Use the same Apple ID to renew the Apple Push Certificate every 12 months.</span></span>
 
4. <span data-ttu-id="decc1-118">Unesite ID jabuke koji se koristi za kreiranje vašeg Apple MDM Push certifikata.</span><span class="sxs-lookup"><span data-stu-id="decc1-118">Enter the Apple ID used to create your Apple MDM push certificate.</span></span> <span data-ttu-id="decc1-119">Zapišite ovaj ID kao podsetnik kada je potrebno da obnovite certifikat.</span><span class="sxs-lookup"><span data-stu-id="decc1-119">Record this ID as a reminder for when you need to renew the certificate.</span></span>

5. <span data-ttu-id="decc1-120">Idite na datoteku certifikata (. Pem), izaberite stavku **Otvori**, a zatim odaberite stavku " **Otpremi**".</span><span class="sxs-lookup"><span data-stu-id="decc1-120">Go to the certificate (.pem) file, choose **Open**, and then choose **Upload**.</span></span> <span data-ttu-id="decc1-121">Pomoću Push certifikata Intune može da se prijavi i upravlja Apple uređajima.</span><span class="sxs-lookup"><span data-stu-id="decc1-121">With the push certificate, Intune can enroll and manage Apple devices.</span></span>