---
title: Nedostaje uslovi iz prodavnice termina za usluge SharePoint online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750465"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="cdc67-102">Omogućavanje BitLocker šifrovanja pomoću Intune</span><span class="sxs-lookup"><span data-stu-id="cdc67-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="cdc67-103">Smernice zaštite krajnjih tačaka mogu se koristiti za Konfigurisanje postavki usluge šifrovanje Boitlocker za Windows uređaje kao što je opisano u: Windows10 (i novije) postavkama da bi se zaštitili uređaji pomoću funkcije Intune</span><span class="sxs-lookup"><span data-stu-id="cdc67-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="cdc67-104">Trebalo bi da budete svesni da mnogi noviji uređaji koji koriste Windows 10 podržavaju BitLocker šifrovanje koji se pokreće bez aplikacije MDM smernica.</span><span class="sxs-lookup"><span data-stu-id="cdc67-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="cdc67-105">Ovo može da utiče na primenu smernica ako su podrazumevane postavke podešene.</span><span class="sxs-lookup"><span data-stu-id="cdc67-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="cdc67-106">Više detalja potražite u članku najčešća pitanja.</span><span class="sxs-lookup"><span data-stu-id="cdc67-106">See FAQ for more detail.</span></span>


<span data-ttu-id="cdc67-107">Najčešća pitanja   p: koja izdanja operativnog sistema Windows podržavaju šifrovanje uređaja pomoću smernica za zaštitu krajnje tačke?</span><span class="sxs-lookup"><span data-stu-id="cdc67-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="cdc67-108"> A: postavke u smernicama za zaštitu krajnje tačke se sprovode pomoću BitLocker CSP.</span><span class="sxs-lookup"><span data-stu-id="cdc67-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="cdc67-109">Ne mogu sva izdanja ili verzije operativnog sistema Windows da podrže BitLocker CSP. 
     </span><span class="sxs-lookup"><span data-stu-id="cdc67-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="cdc67-110">U ovom trenutku Windows izdanja: Enterprise; Podrška za edukaciju, mobilne uređaje i profesionalce (od 1809 ka ka njima) podržana je.</span><span class="sxs-lookup"><span data-stu-id="cdc67-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="cdc67-111">Q: ako je uređaj već šifrovan pomoću usluge OS BitLocker pomoću podrazumevanih postavki OS za šifrovanje i jačine šifrovanja (XTS-AES-128) primeniće se smernice sa drugim postavkama automatski pokrenuti šifrovanje disk jedinice sa novim postavkama?</span><span class="sxs-lookup"><span data-stu-id="cdc67-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="cdc67-112">O: Ne.</span><span class="sxs-lookup"><span data-stu-id="cdc67-112">A: No.</span></span> <span data-ttu-id="cdc67-113">Da biste primenili nove postavke šifrovanja, disk mora biti dešifruo.</span><span class="sxs-lookup"><span data-stu-id="cdc67-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="cdc67-114">Napomena za uređaje koji se upisuju sa Autoautopilot automatskim šifriranjem koji bi se dogodio tokom OOBE nije aktiviran dok se ne proceni da se smernice zasnovane na smernicama koriste umesto podrazumevanih vrednosti OS</span><span class="sxs-lookup"><span data-stu-id="cdc67-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="cdc67-115">Ako je uređaj šifrovan kao rezultat aplikacije "Intune", da li će biti dešifrovana kada se ta smernica ukloni?</span><span class="sxs-lookup"><span data-stu-id="cdc67-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="cdc67-116">A: uklanjanje povezanih smernica za šifrovanje ne prouzrokuje dešifrovanje diskova koje su konfigurisane.</span><span class="sxs-lookup"><span data-stu-id="cdc67-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="cdc67-117">P: Zašto smernice za usaglašenost sa Intune prikazuju da moj uređaj nema "omogućen je BitLocker omogućen", ali da li je?</span><span class="sxs-lookup"><span data-stu-id="cdc67-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="cdc67-118">A: postavka "omogućena za BitLocker omogućeno" u Intune smernicama za usaglašenost koristi Windows uređaj za zdravstvenu proveru (DHA).</span><span class="sxs-lookup"><span data-stu-id="cdc67-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="cdc67-119">Ovaj klijent Meri samo stanje uređaja u vreme pokretanja.</span><span class="sxs-lookup"><span data-stu-id="cdc67-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="cdc67-120">Ako uređaj nije ponovljen od kada je BitLocker šifrovanje dovršen, funkcija DHA klijent neće prijaviti BitLocker kao aktivni.</span><span class="sxs-lookup"><span data-stu-id="cdc67-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>