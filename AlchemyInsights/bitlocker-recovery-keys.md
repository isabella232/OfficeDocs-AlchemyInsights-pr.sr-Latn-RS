---
title: BitLocker ključevi za oporavak
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
- "1922"
- "9000220"
ms.openlocfilehash: 7c56e68cf303939d8e7d4ee0a7301e367ecfe9f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685900"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="f4c86-102">Pristup BitLocker tasterima za oporavak</span><span class="sxs-lookup"><span data-stu-id="f4c86-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="f4c86-103">Prilikom konfigurisanja smernica zaštite krajnjih tačaka, moguće je definisati da li se informacije o BitLocker oporavku treba uskladištiti u usluzi Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f4c86-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="f4c86-104">Ako je ta postavka konfigurisana, uskladišteni podaci o oporavku treba da budu vidljivi administratorskim administratorom kao deo podataka zapisa uređaja u okviru funkcije "Umetanje uređaja" na dva načina:</span><span class="sxs-lookup"><span data-stu-id="f4c86-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="f4c86-105">Uređaji-Azure AD uređaji-> "uređaj" ili uređaji-> svi uređaji-> "uređaj"-> ključeve za oporavak</span><span class="sxs-lookup"><span data-stu-id="f4c86-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="f4c86-106">Pored toga, ako postoji administrativni pristup samom uređaju, ključ za oporavak (lozinka) se može vidjeti tako što će pokrenuti sledeću komandu sa pune komandne linije:</span><span class="sxs-lookup"><span data-stu-id="f4c86-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="f4c86-107">Ako je uređaj šifrovan pre nego što se vrati u Intune, ključ za oporavak možda je povezan sa "Microsoft nalogom" (MSA) koji se koristi za prijavljivanje na uređaj tokom OOBE procesa.</span><span class="sxs-lookup"><span data-stu-id="f4c86-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="f4c86-108">Ako je to bio slučaj, pristupanjem  https://onedrive.live.com/recoverykey i prijavljivanju sa tom MSA trebalo bi da pokaže uređaje za koje su uskladišteni ključevi za oporavak.</span><span class="sxs-lookup"><span data-stu-id="f4c86-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="f4c86-109">Ako je uređaj šifrovan kao rezultat konfiguracije pomoću smernica grupe zasnovane na domenu, informacije o oporavku mogu se uskladištiti u aktivnom direktorijumu.</span><span class="sxs-lookup"><span data-stu-id="f4c86-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

