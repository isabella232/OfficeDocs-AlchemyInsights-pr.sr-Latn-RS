---
title: Problemi sa prijavljivanjem u Microsoft 365 aplikacije
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579915"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="6e375-102">Prazan ekran za prijavljivanje u Microsoft 365 aplikacijama</span><span class="sxs-lookup"><span data-stu-id="6e375-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="6e375-103">Da biste rešili ovaj problem, pokušajte sledeće:</span><span class="sxs-lookup"><span data-stu-id="6e375-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="6e375-104">Instalirajte najnovije ispravke za [Windows](https://support.microsoft.com/help/4027667/windows-10-update) i [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="6e375-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="6e375-105">Poništi opcije programa Internet Explorer: idi na **Alatke**  >  **Internet opcije**  >  **Napredno**  >  **uspostavljanje početnih vrednosti postavki programa Internet Explorer** (Imajte na umu da ćete izgubiti prilagođene postavke), a zatim ponovo pokušajte da se prijavite u Office.</span><span class="sxs-lookup"><span data-stu-id="6e375-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="6e375-106">Onemogućite čuvar aplikacija Windows Defender (WDAG) ili neki sličan zaštitni zid ili program za zaštitu od virusa:</span><span class="sxs-lookup"><span data-stu-id="6e375-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="6e375-107">Na kontrolnoj tabli idite na **programe**, a zatim odaberite **Uključivanje ili isključivanje funkcija operativnog sistema Windows**.</span><span class="sxs-lookup"><span data-stu-id="6e375-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="6e375-108">Ako je čuvar aplikacije Windows Defender omogućen, pokušajte da ga onemogućite.</span><span class="sxs-lookup"><span data-stu-id="6e375-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="6e375-109">**Napomena:** Možda ćete morati ponovo da pokrenete računar.</span><span class="sxs-lookup"><span data-stu-id="6e375-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="6e375-110">Uverite se da se Microsoft. AAD. BrokerPlugin [AAD "Plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) " ne blokira ni jednom aplikacijom ili zaštitnim zidom/antivirusni program.</span><span class="sxs-lookup"><span data-stu-id="6e375-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="6e375-111">[Obrišite Office akreditive](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) koristeći Windows upravljač akreditivima.</span><span class="sxs-lookup"><span data-stu-id="6e375-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="6e375-112">**Napomena:** Putanje registratora za Office 2016 su promenjene u 16,0.</span><span class="sxs-lookup"><span data-stu-id="6e375-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="6e375-113">(Ex: \Software\microsoft\office\16.0\zajed\identitet\)</span><span class="sxs-lookup"><span data-stu-id="6e375-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="6e375-114">Više informacija potražite u članku [problemi prilikom prijavljivanja nakon ažuriranja na Office 2016 Build 16.0.7967 na Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="6e375-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>