---
title: BitLocker ključevi za oporavak
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: ec90e412302c74748e253f2e5430fa4205466f0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820300"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="764b7-102">Pristup BitLocker ključevima za oporavak</span><span class="sxs-lookup"><span data-stu-id="764b7-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="764b7-103">Prilikom konfigurisanja BitLocker postavki Intune smernice za zaštitu krajnje tačke, moguće je definisati da li bitlocker informacije o oporavku treba da budu uskladištene u Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="764b7-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="764b7-104">Ako je ta postavka konfigurisana, uskladišteni podaci o oporavku trebalo bi da budu vidljivi Intune adminitaru kao deo podataka zapisa o uređaju u intune uređajima na dva načina:</span><span class="sxs-lookup"><span data-stu-id="764b7-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="764b7-105">Uređaji - Azure AD uređaji - > "Uređaj" ILI uređaji -> Svi uređaji -> "Uređaj" -> za oporavak</span><span class="sxs-lookup"><span data-stu-id="764b7-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="764b7-106">Osim toga, ako postoji administrativni pristup samom uređaju, ključ za oporavak (Lozinka) može da se vidi tako što će pokrenuti sledeću komandu sa komandne linije sa punim privilegijama:</span><span class="sxs-lookup"><span data-stu-id="764b7-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
<span data-ttu-id="764b7-107">Ako je uređaj šifrovan pre upisanja u Intune, ključ za oporavak je možda povezan sa "Microsoft nalogom" (MSA) koji se koristi za prijavljivanje na uređaj tokom OOBE procesa.</span><span class="sxs-lookup"><span data-stu-id="764b7-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="764b7-108">Ako je to slučaj, pristupanje tom MSA uređaju i prijavljivanje sa njim trebalo bi da pokazuje uređaje za koje su uskladišteni  https://onedrive.live.com/recoverykey ključevi za oporavak.</span><span class="sxs-lookup"><span data-stu-id="764b7-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="764b7-109">Ako je uređaj šifrovan kao rezultat konfiguracije putem smernica grupe zasnovane na domenu, informacije o oporavku mogu da budu uskladištene u prethodnom sistemu Active Directory.</span><span class="sxs-lookup"><span data-stu-id="764b7-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>

<span data-ttu-id="764b7-110">Ako ste konfigurisali smernice za zaštitu krajnje tačke tako da skladište ključ za oporavak u Azure Active Directory, ali ključ za određeni uređaj nije otpremen, možete da pokrenete otpremanje tako što ćete rotirati ključ za oporavak za taj uređaj sa MEM konzole.</span><span class="sxs-lookup"><span data-stu-id="764b7-110">If you have configured Endpoint protection policy to store the recovery key in Azure Active Directory but the key for a specific device has not been uploaded, you can trigger the upload by rotating the recovery key for that device from the MEM console.</span></span> <span data-ttu-id="764b7-111">Za detalje pogledajte [rotiranje BitLocker ključeva za oporavak.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)</span><span class="sxs-lookup"><span data-stu-id="764b7-111">For details, see [Rotate BitLocker recovery keys](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span></span>

