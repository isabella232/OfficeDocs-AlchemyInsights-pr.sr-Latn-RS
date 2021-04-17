---
title: Problemi sa prijavljivanjem u Microsoft 365 aplikacije
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
- "9000571"
- "2559"
ms.openlocfilehash: c64cf2c9dbf63caad22e54ae801adc3ed8ff0f62
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833018"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="233c9-102">Rešavanje poruke o Microsoft 365 aplikacijama "Modul pouzdane platforme na računaru ne funkcioniše ispravno"</span><span class="sxs-lookup"><span data-stu-id="233c9-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="233c9-103">Da biste ispravili ovu grešku, pokušajte sledeće:</span><span class="sxs-lookup"><span data-stu-id="233c9-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="233c9-104">Instalirajte najnovije ispravke za [Windows](https://support.microsoft.com/help/4027667/windows-10-update) i [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="233c9-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="233c9-105">[Obriši Office akredile pomoću](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) Windows upravljača akreditima.</span><span class="sxs-lookup"><span data-stu-id="233c9-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="233c9-106">**Napomogućeno:** Putanje registratora za Office 2016 promenjene su u 16.0.</span><span class="sxs-lookup"><span data-stu-id="233c9-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="233c9-107">(Na ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="233c9-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="233c9-108">Isprobajte proces [oporavka korisnika](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) da biste rešili probleme sa modulom pouzdane platforme (TPM).</span><span class="sxs-lookup"><span data-stu-id="233c9-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="233c9-109">Podesite EnableADAL = 0 na sledeći način:</span><span class="sxs-lookup"><span data-stu-id="233c9-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="233c9-110">Kliknite desnim tasterom miša na Windows Start dugme, odaberite **stavku Pokreni**, **otkucajte regedit**, a zatim kliknite na dugme **U redu.**</span><span class="sxs-lookup"><span data-stu-id="233c9-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="233c9-111">Kliknite na **dugme Da** da biste dozvolili uređivaču registratora da unosi promene na uređaju.</span><span class="sxs-lookup"><span data-stu-id="233c9-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="233c9-112">U uređivaču registratora dodajte DWORD vrednost **funkcije EnableADAL** sa postavkom 0 u **okviru** HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="233c9-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="233c9-113">Više informacija potražite u temi Problemi sa povezivanjem pri prijavljivanjem nakon ažuriranja sistema [Office 2016 izdanje 16.0.7967](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)u operativnom sistemu Windows 10.</span><span class="sxs-lookup"><span data-stu-id="233c9-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>