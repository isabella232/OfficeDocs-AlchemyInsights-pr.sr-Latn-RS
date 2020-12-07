---
title: Omogućavanje pisanja lozinke u Azure AD Connect
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 0eecd89b2558359702935379d7ffbd8b7508f4cd
ms.sourcegitcommit: 62a83a1c6bd9779a1a11b749490bd11670d4b063
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 12/02/2020
ms.locfileid: "49560454"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="8bb91-102">Omogućavanje pisanja lozinke u Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="8bb91-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="8bb91-103">Da biste omogućili samouslužno poništavanje vraćanja, prvo omogućite opciju „vraćanje početnih usluga“ u usluzi Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="8bb91-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="8bb91-104">Na serveru Azure AD Connect, dovršite sledeće korake:</span><span class="sxs-lookup"><span data-stu-id="8bb91-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="8bb91-105">Prijavite se na Azure AD Connect server i pokrenite **Azure AD Connect** čarobnjaka za konfiguraciju.</span><span class="sxs-lookup"><span data-stu-id="8bb91-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="8bb91-106">Na stranici **dobrodošlice** kliknite na dugme **Konfiguriši**.</span><span class="sxs-lookup"><span data-stu-id="8bb91-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="8bb91-107">Na stranici **Dodatni zadaci** izaberite stavku **Prilagodi opcije sinhronizacije**, a zatim kliknite na dugme **Sledeće**.</span><span class="sxs-lookup"><span data-stu-id="8bb91-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="8bb91-108">Na stranici **Povežite se sa Azure AD** unesite akreditiv globalnog administratora za Azure zakupca, a zatim kliknite **Sledeće**.</span><span class="sxs-lookup"><span data-stu-id="8bb91-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="8bb91-109">Na stranicama za filtriranje **Povezivanje direktorijuma** i **Domen/OU**, kliknite na **Sledeće**.</span><span class="sxs-lookup"><span data-stu-id="8bb91-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="8bb91-110">Na stranici **Opcionalne funkcije** potvrdite izbor u polju pored stavke **Pisanje lozinke** i kliknite na dugme **Sledeće**.</span><span class="sxs-lookup"><span data-stu-id="8bb91-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="8bb91-111">Na stranici **Spremno za konfiguraciju**, kliknite na **Konfiguriši** i sačekajte da se proces završi.</span><span class="sxs-lookup"><span data-stu-id="8bb91-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="8bb91-112">Kada vidite da se konfiguracija završila, kliknite na **Izlaz**.</span><span class="sxs-lookup"><span data-stu-id="8bb91-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="8bb91-113">Uz omogućeno pisanje lozinke u Azure AD Connect, konfigurišite Azure AD SSPR za generisanje.</span><span class="sxs-lookup"><span data-stu-id="8bb91-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="8bb91-114">Da biste omogućili pisanje lozinke u usluzi SSPR, dovršite sledeće korake:</span><span class="sxs-lookup"><span data-stu-id="8bb91-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="8bb91-115">Prijavite se na Azure portal pomoću globalnog administratorskog naloga.</span><span class="sxs-lookup"><span data-stu-id="8bb91-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="8bb91-116">Potražite i izaberite stavku **Azure Active Directory**, kliknite na **Poništi lozinku**, a zatim kliknite na **Lokalna integracija**.</span><span class="sxs-lookup"><span data-stu-id="8bb91-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="8bb91-117">Postavite opciju za **Želite li da pišete lozinke na lokalnom direktorijumu?** na **„Da“**.</span><span class="sxs-lookup"><span data-stu-id="8bb91-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="8bb91-118">Postavite opciju za **Želite li da omogućite korisnicima da otključavaju naloge bez poništavanja lozinke?** na **„Da“**.</span><span class="sxs-lookup"><span data-stu-id="8bb91-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="8bb91-119">Kada budete spremni, kliknite na dugme **Sačuvaj**.</span><span class="sxs-lookup"><span data-stu-id="8bb91-119">When ready, click **Save**.</span></span>

<span data-ttu-id="8bb91-120">Više informacija potražite u članku [Omogući Azure Active Directory samouslužno poništavanje vraćanja u lokalno okruženje](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="8bb91-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="8bb91-121">Kada administrator poništi korisničku lozinku na Azure portalu, ako je taj korisnik ujedinjen ili je sinhronizovan heš lozinke, lozinka se ponovo piše lokalno.</span><span class="sxs-lookup"><span data-stu-id="8bb91-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="8bb91-122">Ova funkcionalnost trenutno nije podržana na Office portalu za administraciju.</span><span class="sxs-lookup"><span data-stu-id="8bb91-122">This functionality is currently not supported in the Office Admin portal.</span></span>