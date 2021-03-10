---
title: Omogućavanje Microsoft zaštitnika za Office 365 za SharePoint online, OneDrive i Microsoft timove
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 1c29afdcc52e7032fea22d698371677918665fa9
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695652"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="a713b-102">Omogućavanje Microsoft zaštitnika za Office 365 za SharePoint online, OneDrive i Microsoft timove</span><span class="sxs-lookup"><span data-stu-id="a713b-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive and Microsoft Teams</span></span>

1. <span data-ttu-id="a713b-103">Korišćenje globalnih administratora ili akreditiva administracije, prijavite se u [Office 365 centar za bezbednost i usaglašenost](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="a713b-103">Using your global admin or security admin credentials, log in to the [Office 365 Security and Compliance Center](https://protection.office.com/).</span></span>
2. <span data-ttu-id="a713b-104">Izaberite stavku **Upravljanje pretnjama** u levom oknu, a **zatim izaberite stavku**  >  [sigurnosni prilozi](https://protection.office.com/safeattachment).</span><span class="sxs-lookup"><span data-stu-id="a713b-104">Select **Threat management** in the left pane, and then select **Policy** > [Safe attachments](https://protection.office.com/safeattachment).</span></span>
3. <span data-ttu-id="a713b-105">Izaberite stavku **Uključi Microsoft Defender za Office 365 za SharePoint, OneDrive i Microsoft timove**, a zatim izaberite stavku **Sačuvaj**.</span><span class="sxs-lookup"><span data-stu-id="a713b-105">Select **Turn on Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then select **Save**.</span></span>
    > [!TIP]
    >
    > - <span data-ttu-id="a713b-106">Kao globalni administrator ili SharePoint online administrator, na sledećoj PowerShell cmdlet sajtu izaberite stavku *tačno*:  [setu-spojstanar](https://go.microsoft.com/fwlink/?linkid=2092301)</span><span class="sxs-lookup"><span data-stu-id="a713b-106">As a global admin or a SharePoint Online admin, run the following PowerShell cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span></span>
    > - [<span data-ttu-id="a713b-107">Podešavanje upozorenja za otkrivene datoteke</span><span class="sxs-lookup"><span data-stu-id="a713b-107">Set up alerts for detected files</span></span>](https://go.microsoft.com/fwlink/?linkid=2092110)

<span data-ttu-id="a713b-108">Više informacija potražite u članku [Microsoft zaštitnik za Office 365 za SharePoint, OneDrive i Microsoft timove](https://go.microsoft.com/fwlink/?linkid=2092041).</span><span class="sxs-lookup"><span data-stu-id="a713b-108">For more information, see [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).</span></span>
