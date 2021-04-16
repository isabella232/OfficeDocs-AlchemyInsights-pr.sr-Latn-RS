---
title: Popravljanje Microsoft 365 aplikacija Vaš nalog je u lošem stanju
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
- "2558"
- "9000571"
ms.openlocfilehash: 4654b49289a455c1e6641f47fae573d2fcebc717
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812550"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="0ccc6-102">Popravljanje greške "Vaš nalog je u lošem stanju" za Microsoft 365 aplikacije</span><span class="sxs-lookup"><span data-stu-id="0ccc6-102">Fixing the Microsoft 365 apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="0ccc6-103">Da biste ispravili ovu grešku, isprobajte sledeće opcije na računaru na koji to utiče:</span><span class="sxs-lookup"><span data-stu-id="0ccc6-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="0ccc6-104">Otvorite Office aplikaciju i izaberite **Stavku**  >  **Nalog datoteke**  >  **Odjavi se sa svih naloga**.</span><span class="sxs-lookup"><span data-stu-id="0ccc6-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="0ccc6-105">Prijavite se ponovo koristeći korisnički nalog sa važećom licencom.</span><span class="sxs-lookup"><span data-stu-id="0ccc6-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="0ccc6-106">Detaljne informacije potražite u članku [Nalozi u sistemu Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="0ccc6-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="0ccc6-107">[Obriši Office akredile pomoću](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows upravljača akreditima.</span><span class="sxs-lookup"><span data-stu-id="0ccc6-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="0ccc6-108">**Napomogućeno:** Putanje registratora za Office 2016 promenjene su u 16.0.</span><span class="sxs-lookup"><span data-stu-id="0ccc6-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="0ccc6-109">Na primer, \Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="0ccc6-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="0ccc6-110">Ako dođe do greške prilikom povezivanja sa uslugom Office 365 pomoću sistema Office 2013, omogućite [modernu](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) potvrdu identiteta za Office klijent.</span><span class="sxs-lookup"><span data-stu-id="0ccc6-110">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="0ccc6-111">Dodatne informacije potražite u članku Rešavanje problema sa aplikacijama koje nisu pregledači i koje ne mogu da se prijade u [Microsoft 365, Azure ili Intune.](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)</span><span class="sxs-lookup"><span data-stu-id="0ccc6-111">For more information, see [How to troubleshoot non-browser apps that can't sign in to Microsoft  365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

