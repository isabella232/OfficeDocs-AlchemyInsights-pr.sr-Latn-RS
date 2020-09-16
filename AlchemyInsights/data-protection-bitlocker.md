---
title: Zaštita podataka – BitLocker
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
- "1802"
- "9000220"
ms.openlocfilehash: ab28162fcdf0a37060be3bdf15a78aceca7a48b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731253"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="15f03-102">Omogućavanje BitLocker šifrovanja pomoću Intune</span><span class="sxs-lookup"><span data-stu-id="15f03-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="15f03-103">Smernice zaštite krajnjih tačaka mogu se koristiti za konfigurisanje BitLocker postavki šifrovanja za Windows uređaje.</span><span class="sxs-lookup"><span data-stu-id="15f03-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="15f03-104">Više informacija potražite u članku [Postavke operativnog sistema Windows 10 (i novije) kako biste zaštitili uređaje pomoću funkcije Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="15f03-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="15f03-105">Trebalo bi da budete svesni da mnogi noviji uređaji koji koriste Windows 10 podržavaju BitLocker šifrovanje, koji se pokreće bez aplikacije MDM smernica.</span><span class="sxs-lookup"><span data-stu-id="15f03-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="15f03-106">Ovo može da utiče na primenu smernica ako su postavke koje nisu podrazumevane.</span><span class="sxs-lookup"><span data-stu-id="15f03-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="15f03-107">Detaljnije pogledajte sledeće najčešća pitanja.</span><span class="sxs-lookup"><span data-stu-id="15f03-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="15f03-108">Informacije o rešavanju problema sa BitLocker problemom potražite [u članku rešavanje problema sa BitLocker smernicama u programu Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="15f03-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="15f03-109">**NAJČEŠĆA PITANJA**</span><span class="sxs-lookup"><span data-stu-id="15f03-109">**FAQ**</span></span>

 <span data-ttu-id="15f03-110">Q: koje izdanje sistema Windows podržava šifrovanje uređaja pomoću smernica za zaštitu krajnje tačke?</span><span class="sxs-lookup"><span data-stu-id="15f03-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="15f03-111">A: postavke u smernicama za zaštitu krajnje tačke se sprovode pomoću [BitLocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="15f03-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="15f03-112">Ne svi izdanci ili verzije operativnog sistema Windows podržavaju BitLocker CSP.</span><span class="sxs-lookup"><span data-stu-id="15f03-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="15f03-113">U ovom trenutku, podržavaju se sledeća izdanja operativnog sistema Windows: Enterprise, edukacija, mobilni, mobilni Enterprise i Professional (izdanje 1809 i novije verzije).</span><span class="sxs-lookup"><span data-stu-id="15f03-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="15f03-114">P: ako je uređaj već šifrovan pomoću usluge OS BitLocker pomoću podrazumevanih postavki OS za šifrovanje i jačine šifrovanja (XTS-AES-128), primena smernica sa drugim postavkama automatski izaziva ponovno šifrovanje disk jedinice sa novim postavkama?</span><span class="sxs-lookup"><span data-stu-id="15f03-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="15f03-115">O: Ne.</span><span class="sxs-lookup"><span data-stu-id="15f03-115">A: No.</span></span> <span data-ttu-id="15f03-116">Da biste primenili nove postavke šifrovanja, disk jedinica mora prvo da se dešifruje.</span><span class="sxs-lookup"><span data-stu-id="15f03-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="15f03-117">**Napomena:** Za uređaje koje se upisuju na Autoautopilot, automatsko šifrovanje koje bi se desilo tokom OOBE ne pokreće se dok se ne proceni politika Intune, što omogućava postavkama zasnovane na smernicama da se koriste umesto podrazumevanih vrednosti OS.</span><span class="sxs-lookup"><span data-stu-id="15f03-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="15f03-118">Q: ako je uređaj šifrovan kao rezultat primene smernica Intune, da li će se dešifruti kada se ta smernica ukloni?</span><span class="sxs-lookup"><span data-stu-id="15f03-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="15f03-119">A: uklanjanje smernica vezanim za šifrovanje ne prouzrokuje dešifrovanje diskova koje su podešene.</span><span class="sxs-lookup"><span data-stu-id="15f03-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="15f03-120">P: Zašto smernice za usaglašenost sa Intune prikazuju da moj uređaj nema omogućen BitLocker, čak i ako jeste?</span><span class="sxs-lookup"><span data-stu-id="15f03-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="15f03-121">A: postavka "omogućeno je da BitLocker omogućena" u smernicama za usaglašenost u Intune koristi Windows uređaj za zdravstvenu proveru (DHA) klijentu.</span><span class="sxs-lookup"><span data-stu-id="15f03-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="15f03-122">Ovaj klijent Meri samo stanje uređaja u vreme pokretanja.</span><span class="sxs-lookup"><span data-stu-id="15f03-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="15f03-123">Ako uređaj nije ponovo rešen od završetka usluge BitLocker šifrovanja, usluga DHA klijenta neće prijaviti da je BitLocker aktivan.</span><span class="sxs-lookup"><span data-stu-id="15f03-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 