---
title: Konfigurisanje mesta povezivanja usluge (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037287"
---
# <a name="configure-service-connection-point-scp"></a><span data-ttu-id="25ef7-102">Konfigurisanje mesta povezivanja usluge (SCP)</span><span class="sxs-lookup"><span data-stu-id="25ef7-102">Configure Service connection Point (SCP)</span></span>

<span data-ttu-id="25ef7-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span><span class="sxs-lookup"><span data-stu-id="25ef7-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span></span>

- <span data-ttu-id="25ef7-104">**Razlog**: nije moguće čitati objekat SCP i dobiti informacije o AZURE AD zakupcu</span><span class="sxs-lookup"><span data-stu-id="25ef7-104">**Reason**: Unable to read the SCP object and get the Azure AD tenant information</span></span>
- <span data-ttu-id="25ef7-105">**Rezolucija**: pogledajte odeljak [Konfigurisanje mesta povezivanja usluge](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span><span class="sxs-lookup"><span data-stu-id="25ef7-105">**Resolution**: Refer to the section [Configure a Service Connection Point](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span></span>


<span data-ttu-id="25ef7-106">**Akcioni plan**</span><span class="sxs-lookup"><span data-stu-id="25ef7-106">**Action plan**</span></span>

- <span data-ttu-id="25ef7-107">Provera da li je uređaj primio GPO za kontrolisanu validaciju.</span><span class="sxs-lookup"><span data-stu-id="25ef7-107">Check whether the device has received the GPO for the controlled validation.</span></span>
- <span data-ttu-id="25ef7-108">Uverite se da je GPO kreirao registarske ključeve.</span><span class="sxs-lookup"><span data-stu-id="25ef7-108">Ensure that the GPO has created the registry keys.</span></span>
- <span data-ttu-id="25ef7-109">Uverite se da imate 2 ključa kreirane pomoću direktorijuma ID-a i onkosistema.</span><span class="sxs-lookup"><span data-stu-id="25ef7-109">Ensure that you have 2 keys created with your Directory ID and onmicrosoft domain.</span></span>

<span data-ttu-id="25ef7-110">**Konfigurisanje postavke registra na strani klijenta za SCP**</span><span class="sxs-lookup"><span data-stu-id="25ef7-110">**Configure client-side registry setting for SCP**</span></span>

<span data-ttu-id="25ef7-111">Koristite sledeći primer da biste kreirali objekat smernica grupe (GPO) za primenu postavki registratora koje konfiguriše stavku SCP u registratoru uređaja.</span><span class="sxs-lookup"><span data-stu-id="25ef7-111">Use the following example to create a Group Policy Object (GPO) to deploy a registry setting that configures an SCP entry in the registry of your devices.</span></span>

1. <span data-ttu-id="25ef7-112">Otvorite konzolu za upravljanje smernicama grupe i kreirajte novi GPO u domenu.</span><span class="sxs-lookup"><span data-stu-id="25ef7-112">Open a Group Policy Management console and create a new GPO in your domain.</span></span>
     - <span data-ttu-id="25ef7-113">Navedite novo GPO ime (na primer, Clientsidep)</span><span class="sxs-lookup"><span data-stu-id="25ef7-113">Provide your newly created GPO a name (for example, ClientSideSCP)</span></span>

2. <span data-ttu-id="25ef7-114">Uredite GPO i pronađite sledeću putanju: **Konfiguracija računara > željene postavke > Windows postavkama > registratoru**.</span><span class="sxs-lookup"><span data-stu-id="25ef7-114">Edit the GPO and locate the following path: **Computer Configuration > Preferences > Windows Settings > Registry**.</span></span>

3. <span data-ttu-id="25ef7-115">Kliknite desnim tasterom miša na **registrator** i izaberite **stavku nova > registratora**.</span><span class="sxs-lookup"><span data-stu-id="25ef7-115">Right-click on **Registry** and select **New > Registry Item**.</span></span>

4. <span data-ttu-id="25ef7-116">Na kartici **Opšte** podesite sledeće:</span><span class="sxs-lookup"><span data-stu-id="25ef7-116">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="25ef7-117">**Radnja**: ispravka</span><span class="sxs-lookup"><span data-stu-id="25ef7-117">**Action**: Update</span></span>
    
- <span data-ttu-id="25ef7-118">**Saće: HKEY_LOCAL_MACHINE**</span><span class="sxs-lookup"><span data-stu-id="25ef7-118">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="25ef7-119">**Ključna putanja**: Software\microsoft\windows\currentversion\cdj\aad</span><span class="sxs-lookup"><span data-stu-id="25ef7-119">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="25ef7-120">**Ime vrednosti**: tenanti</span><span class="sxs-lookup"><span data-stu-id="25ef7-120">**Value name**: TenantId</span></span>
    
- <span data-ttu-id="25ef7-121">**Tip vrednosti**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="25ef7-121">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="25ef7-122">**Podaci o vrednostima**: GUID ili ID direktorijuma vaše AURE instance oglasa (Ova vrednost se može pronaći u usluzi **Azure > Azure Active Directory > svojstvima > ID direktorijuma**)</span><span class="sxs-lookup"><span data-stu-id="25ef7-122">**Value data**: The GUID or Directory ID of your Azure AD instance (This value can be found in **Azure portal > Azure Active Directory > Properties > Directory ID**)</span></span>
 
- <span data-ttu-id="25ef7-123">Kliknite na dugme **U redu**.</span><span class="sxs-lookup"><span data-stu-id="25ef7-123">Click **OK**.</span></span>
 
5. <span data-ttu-id="25ef7-124">Kliknite desnim tasterom miša na **registrator** i izaberite **stavku nova > registratora**.</span><span class="sxs-lookup"><span data-stu-id="25ef7-124">Right-click on **Registry** and select **New > Registry Item**.</span></span>

6. <span data-ttu-id="25ef7-125">Na kartici **Opšte** podesite sledeće:</span><span class="sxs-lookup"><span data-stu-id="25ef7-125">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="25ef7-126">**Radnja**: ispravka</span><span class="sxs-lookup"><span data-stu-id="25ef7-126">**Action**: Update</span></span>
    
- <span data-ttu-id="25ef7-127">**Saće: HKEY_LOCAL_MACHINE**</span><span class="sxs-lookup"><span data-stu-id="25ef7-127">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="25ef7-128">**Ključna putanja**: Software\microsoft\windows\currentversion\cdj\aad</span><span class="sxs-lookup"><span data-stu-id="25ef7-128">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="25ef7-129">**Ime vrednosti**: ime tenanga</span><span class="sxs-lookup"><span data-stu-id="25ef7-129">**Value name**: TenantName</span></span>
    
- <span data-ttu-id="25ef7-130">**Tip vrednosti**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="25ef7-130">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="25ef7-131">**Podaci o vrednosti**: verifikovano ime domena ako koristite federirani ambijent kao što je AD FS.</span><span class="sxs-lookup"><span data-stu-id="25ef7-131">**Value data**: Your verified domain name if you are using federated environment such as AD FS.</span></span> <span data-ttu-id="25ef7-132">Verifikovano ime domena ili onmicrosoft.com ime domena (na primer, comtoso. onmicrosoft). com ako koristite kontrolisano okruženje</span><span class="sxs-lookup"><span data-stu-id="25ef7-132">Your verified domain name or your onmicrosoft.com domain name (for example, contoso.onmicrosoft).com if you are using managed environment</span></span>

- <span data-ttu-id="25ef7-133">Kliknite na dugme **U redu**.</span><span class="sxs-lookup"><span data-stu-id="25ef7-133">Click **OK**.</span></span>

7. <span data-ttu-id="25ef7-134">Zatvorite uređivač za novi kreirani GPO.</span><span class="sxs-lookup"><span data-stu-id="25ef7-134">Close the editor for the newly created GPO.</span></span>

8. <span data-ttu-id="25ef7-135">Povežite novi kreirani GPO na željeni računar koji sadrži domen koji pripadaju vašem kontrolisanom broju stanovnika.</span><span class="sxs-lookup"><span data-stu-id="25ef7-135">Link the newly created GPO to the desired OU containing domain-joined computers that belong to your controlled rollout population.</span></span>

<span data-ttu-id="25ef7-136">Više informacija potražite u članku [kontrolisana validacija hibridnog AZURE AD JOIN-Azure AD | Microsoft docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) i  [Rešavanje problema hibridnog Azure aktivnog direktorijuma su spojeni | Microsoft docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span><span class="sxs-lookup"><span data-stu-id="25ef7-136">For more information, see [Controlled validation of hybrid Azure AD join - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) and  [Troubleshooting hybrid Azure Active Directory joined devices | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span></span>









