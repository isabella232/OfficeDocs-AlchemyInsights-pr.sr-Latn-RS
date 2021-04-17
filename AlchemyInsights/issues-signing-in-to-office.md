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
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833053"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="ddcc1-102">Prazan ekran za prijavljivanje u Microsoft 365 aplikacijama</span><span class="sxs-lookup"><span data-stu-id="ddcc1-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="ddcc1-103">Da biste rešili ovaj problem, pokušajte sledeće:</span><span class="sxs-lookup"><span data-stu-id="ddcc1-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="ddcc1-104">Instalirajte najnovije ispravke za [Windows](https://support.microsoft.com/help/4027667/windows-10-update) i [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="ddcc1-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="ddcc1-105">Uspostavite početne vrednosti opcija u programu Internet Explorer: Idite na Alatke Internet opcije Napredne postavke programa  >    >    >  **Internet Explorer** (imajte naznaku da ćete izgubiti prilagođene postavke), a zatim pokušajte ponovo da se prijavite u Office.</span><span class="sxs-lookup"><span data-stu-id="ddcc1-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="ddcc1-106">Onemogućite Application Guard Windows zaštitnik (WDAG) ili bilo koji sličan zaštitni zid ili antivirusni program:</span><span class="sxs-lookup"><span data-stu-id="ddcc1-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="ddcc1-107">Na kontrolnoj tabli idite na **stavku Programi**, a zatim odaberite stavku Uključivanje ili **isključivanje Funkcija operativnog sistema Windows.**</span><span class="sxs-lookup"><span data-stu-id="ddcc1-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="ddcc1-108">Ako je Application Guard Windows zaštitnik omogućen, pokušajte da ga onemogućite.</span><span class="sxs-lookup"><span data-stu-id="ddcc1-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="ddcc1-109">**Napomogućeno:** Možda ćete morati ponovo da pokrenete računar.</span><span class="sxs-lookup"><span data-stu-id="ddcc1-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="ddcc1-110">Uverite se da aplikacija ili programski dodatak Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) ne blokira nijednu aplikaciju ili zaštitni zid/antivirusni program.</span><span class="sxs-lookup"><span data-stu-id="ddcc1-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="ddcc1-111">[Obriši Office akredile pomoću](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows upravljača akreditima.</span><span class="sxs-lookup"><span data-stu-id="ddcc1-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="ddcc1-112">**Napomogućeno:** Putanje registratora za Office 2016 promenjene su u 16.0.</span><span class="sxs-lookup"><span data-stu-id="ddcc1-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="ddcc1-113">(Na ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="ddcc1-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="ddcc1-114">Više informacija potražite u temi Problemi sa povezivanjem pri prijavljivanjem nakon ažuriranja sistema [Office 2016 izdanje 16.0.7967](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)u operativnom sistemu Windows 10.</span><span class="sxs-lookup"><span data-stu-id="ddcc1-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>