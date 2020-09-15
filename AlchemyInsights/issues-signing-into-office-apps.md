---
title: Problemi sa prijavljivanjem u Microsoft 365 aplikacije
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
- "9000571"
- "2559"
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695193"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="beda6-102">Popravka Microsoft 365 aplikacija "modul pouzdane platforme računara ne radi ispravno" poruka</span><span class="sxs-lookup"><span data-stu-id="beda6-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="beda6-103">Da biste ispravili ovu grešku, pokušajte sledeće:</span><span class="sxs-lookup"><span data-stu-id="beda6-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="beda6-104">Instalirajte najnovije ispravke za [Windows](https://support.microsoft.com/help/4027667/windows-10-update) i [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="beda6-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="beda6-105">[Brisanje Office akreditiva](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomoću upravljača Windows akreditivima.</span><span class="sxs-lookup"><span data-stu-id="beda6-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="beda6-106">**Napomena:** Putanje registratora za Office 2016 su promenjene u 16,0.</span><span class="sxs-lookup"><span data-stu-id="beda6-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="beda6-107">(Ex: \Software\microsoft\office\16.0\local \ identitet\)</span><span class="sxs-lookup"><span data-stu-id="beda6-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="beda6-108">Isprobajte [proces oporavka korisnika](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) za popravljanje otkazivanja modula pouzdane platforme (TPM).</span><span class="sxs-lookup"><span data-stu-id="beda6-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="beda6-109">Postavljanje programskog programskog + = 0 pomoću sledećih koraka:</span><span class="sxs-lookup"><span data-stu-id="beda6-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="beda6-110">Kliknite desnim tasterom miša na dugme Start operativnog sistema Windows, odaberite stavku **Pokreni**, otkucajte **ponovno gedit**, a zatim odaberite stavku **u redu**.</span><span class="sxs-lookup"><span data-stu-id="beda6-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="beda6-111">Kliknite na dugme **da** da biste omogućili uređivaču registratora da napravi promene na uređaju.</span><span class="sxs-lookup"><span data-stu-id="beda6-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="beda6-112">U uređivaču registratora dodajte DWORD vrednost programskog **dodatka sa** podešavanjem **0** u okviru HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity.</span><span class="sxs-lookup"><span data-stu-id="beda6-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="beda6-113">Više informacija potražite u članku [problemi sa vezom u prijavljivanju nakon ažuriranja na Office 2016 16.0.7967 u operativnom sistemu Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="beda6-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>