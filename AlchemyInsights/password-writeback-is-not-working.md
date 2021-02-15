---
title: Vraćanje lozinki ne radi
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243521"
---
# <a name="password-writeback-is-not-working"></a><span data-ttu-id="31458-102">Vraćanje lozinki ne radi</span><span class="sxs-lookup"><span data-stu-id="31458-102">Password Writeback is not working</span></span>

<span data-ttu-id="31458-103">**Imam problema sa konfigurisanjem sinhronizacijom lozinki**</span><span class="sxs-lookup"><span data-stu-id="31458-103">**I'm having problems configuring password writeback**</span></span>

- <span data-ttu-id="31458-104">Ponovno upisivanje lozinki je Premium funkcija.</span><span class="sxs-lookup"><span data-stu-id="31458-104">Password writeback is a premium feature.</span></span>
- <span data-ttu-id="31458-105">Uverite se da razumete zahteve licenciranja:</span><span class="sxs-lookup"><span data-stu-id="31458-105">Make sure that you understand the licensing requirements:</span></span>
  - <span data-ttu-id="31458-106">Morate imati bar jednu licencu dodeljenu u organizaciji</span><span class="sxs-lookup"><span data-stu-id="31458-106">You must have at least one license assigned in your organization</span></span>
  - <span data-ttu-id="31458-107">**Samo oblaci korisnici** – bilo koji Office 365 (O365) plaćeni MJ ili AZURE AD Basic</span><span class="sxs-lookup"><span data-stu-id="31458-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
  - <span data-ttu-id="31458-108">**Cloud i/ili lokalno korisnici** – AZURE AD Premium P1 ili P2, Enterprise mobilnost + Security (Ems) ili bezbedno preduzeće (SPE)</span><span class="sxs-lookup"><span data-stu-id="31458-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="31458-109">Da biste saznali više o zahtevima licenciranja, pogledajte članak [licenciranje zahteva za Azure AD samouslužno poništavanje lozinke](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="31458-109">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span></span>
- <span data-ttu-id="31458-110">Imate najmanje jedan administratorski nalog i jedan probni korisnički nalog sa jednom od odgovarajućih licenci.</span><span class="sxs-lookup"><span data-stu-id="31458-110">You have at least one administrator account and one test user account with one of the appropriate license.</span></span>
- <span data-ttu-id="31458-111">Morate da povežete Azure AD se poveže sa glavnim Emulatorom kontrolora domena za upisivanje lozinki na posao.</span><span class="sxs-lookup"><span data-stu-id="31458-111">You must connect Azure AD Connect to the Primary Domain Controller Emulator for password writeback to work.</span></span> <span data-ttu-id="31458-112">Možete da konfigurišete Azure AD Connect da biste koristili primarni kontroler domena tako što ćete kliknuti desnim tasterom miša na **Svojstva** konektora za sinhronizaciju aktivnog direktorijuma, a zatim izabrati stavku **Podešavanje Particija direktorijuma**.</span><span class="sxs-lookup"><span data-stu-id="31458-112">You can configure Azure AD Connect to use a Primary Domain Controller by right clicking on the **properties** of the Active Directory synchronization connector, then selecting **configure directory partitions**.</span></span> <span data-ttu-id="31458-113">Odatle potražite odeljak **Postavke veze sa kontrolerom domena** i potvrdite izbor u polju za potvrdu pod naslovom **samo koristite željene kontrolore domena**.</span><span class="sxs-lookup"><span data-stu-id="31458-113">From there, look for the **domain controller connection settings** section and check the box titled **only use preferred domain controllers**.</span></span>
  > [!NOTE]
  > <span data-ttu-id="31458-114">Ako centar za željeni centar nije PDC Emulator, Azure AD Connect i dalje dostižu PDC-u za ponovno upisivanje lozinki.</span><span class="sxs-lookup"><span data-stu-id="31458-114">If the preferred DC is not a PDC emulator, Azure AD Connect will still reach out to the PDC for password writeback.</span></span>
- <span data-ttu-id="31458-115">Poništavanje lozinke je podešeno i omogućeno u vašem zakupcu.</span><span class="sxs-lookup"><span data-stu-id="31458-115">Password reset has been configured and enabled in your tenant.</span></span> <span data-ttu-id="31458-116">Više informacija potražite u članku [Omogućavanje korisnicima da resetuju svoje Azure oglase lozinke](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span><span class="sxs-lookup"><span data-stu-id="31458-116">For more information, see [Enable users to reset their Azure AD passwords](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span></span>
- <span data-ttu-id="31458-117">Uverite se da je administratorski nalog koji se koristi za omogućavanje ispravnosti lozinki administratorski nalog (kreiran u okviru Azure AD nije lokalni AD)</span><span class="sxs-lookup"><span data-stu-id="31458-117">Make sure that the administrator account being used to enable Password Writeback is a cloud administrator account (created in Azure AD not on-premises AD)</span></span>
- <span data-ttu-id="31458-118">Imate jedan ili više šuma OGLAŠAVANJE na lokalnom sajtu koji radi pod operativnim sistemom Windows Server 2008 R2, Windows Server 2012 ili Windows Server 2012 R2 sa instaliranim najsavremenijim servisnim paketima</span><span class="sxs-lookup"><span data-stu-id="31458-118">You have a single or multi-forest AD on-premises deployment running Windows Server 2008 R2, Windows Server 2012, or Windows Server 2012 R2 with the latest service packs installed</span></span>
- <span data-ttu-id="31458-119">Imate instaliranu alatku Azure AD Connect i pripremili ste reklamu za sinhronizaciju u oblaku.</span><span class="sxs-lookup"><span data-stu-id="31458-119">You have the Azure AD Connect tool installed and you have prepared your AD environment for synchronization to the cloud.</span></span> <span data-ttu-id="31458-120">Pre nego što testirate poništavanje lozinki, uverite se da ste prvi put dovršili sa sinhronizacijom kompletne i potpune sinhronizacije iz AD i Azure AD u usluzi Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="31458-120">Before testing password writeback, make sure that you first complete a full import and full sync from both AD and Azure AD in Azure AD Connect.</span></span>
- <span data-ttu-id="31458-121">Da biste saznali više, pogledajte članak kako se radi [potpuna sinhronizacija i kompletan uvoz u usluzi Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span><span class="sxs-lookup"><span data-stu-id="31458-121">To learn more, see how to do a [full sync and full import in Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span></span>

<span data-ttu-id="31458-122">**Imam problem sa mogućnošću povezivanja lozinki**</span><span class="sxs-lookup"><span data-stu-id="31458-122">**I'm having a problem with password writeback connectivity**</span></span>

1. <span data-ttu-id="31458-123">Preuzmite i omogućite najnoviju verziju usluge [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span><span class="sxs-lookup"><span data-stu-id="31458-123">Download and enable the latest version of [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span></span>
2. <span data-ttu-id="31458-124">Konfiguracija zaštitnog zida: alatka Azure AD Connect (1.1.443 i iznad) Trebaće im **HTTPS** pristup na:</span><span class="sxs-lookup"><span data-stu-id="31458-124">Firewall configuration: The Azure AD Connect tool (1.1.443 and above) will need **outbound HTTPS** access to:</span></span>
    - <span data-ttu-id="31458-125">passwordreset.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="31458-125">passwordreset.microsoftonline.com</span></span>
    - <span data-ttu-id="31458-126">servicebus. Windows. mreže</span><span class="sxs-lookup"><span data-stu-id="31458-126">servicebus.windows.networks</span></span>
3. <span data-ttu-id="31458-127">Omogući da veza sa nepristupačnošću potraje najmanje 2-3 minuta</span><span class="sxs-lookup"><span data-stu-id="31458-127">Allow idle connections to persist for at least 2-3 minutes</span></span>

<span data-ttu-id="31458-128">**Još uvek imam problema sa lozinkom sinhronizacijom**</span><span class="sxs-lookup"><span data-stu-id="31458-128">**I'm still having problems with password writeback**</span></span>

- <span data-ttu-id="31458-129">Ako i dalje imate poteškoća, pokušajte da onemogućite i ponovo omogućite uslugu "ispravnost lozinke" u alatki Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="31458-129">If you are still having difficulty, try disabling and re-enabling the password writeback service in the Azure AD Connect tool</span></span>
- <span data-ttu-id="31458-130">Da biste saznali više, pogledajte kako da [onemogućite i ponovo omogućite poništavanje lozinki.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="31458-130">To learn more, see how to [disable and re-enable password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span></span>
