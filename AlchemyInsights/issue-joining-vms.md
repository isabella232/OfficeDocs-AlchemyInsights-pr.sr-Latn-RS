---
title: Problem sa uključivanja funkcija Vims
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885663"
---
# <a name="issue-joining-vms"></a><span data-ttu-id="6b8ee-102">Problem sa uključivanja funkcija Vims</span><span class="sxs-lookup"><span data-stu-id="6b8ee-102">Issue joining VMs</span></span>

<span data-ttu-id="6b8ee-103">Da biste rešili probleme koji se javljaju prilikom pokušaja pridruživanja funkcija Vims, obavite sledeće korake:</span><span class="sxs-lookup"><span data-stu-id="6b8ee-103">To resolve issues that occur while trying to join VMs, perform the following steps:</span></span>

1. <span data-ttu-id="6b8ee-104">Pokušajte da se prijavite pomoću **UPN** formata (na primer "joeuser@contoso.com") umesto formata **Samaccountname** (' CONTOSO\joeuser ').</span><span class="sxs-lookup"><span data-stu-id="6b8ee-104">Try to sign in using the **UPN** format (for example, 'joeuser@contoso.com') instead of the **SAMAccountName** format ('CONTOSO\joeuser').</span></span>
2. <span data-ttu-id="6b8ee-105">Uverite se da ste omogućili sinhronizaciju lozinki u skladu sa koracima *iznetim iz vodiča za* pokretanje.</span><span class="sxs-lookup"><span data-stu-id="6b8ee-105">Ensure that you have enabled password synchronization in accordance with the steps outlined in the *Getting Started* guide.</span></span>
3. <span data-ttu-id="6b8ee-106">Proverite da li korisnički nalog koji utiče na stavku nije spoljni nalog u Azure AD zakupcu.</span><span class="sxs-lookup"><span data-stu-id="6b8ee-106">Ensure that the affected user account is not an external account in the Azure AD tenant.</span></span> <span data-ttu-id="6b8ee-107">Spoljni korisnici ne mogu da se prijave u kontrolisani domen od kako Azure AD Domain Services Domain nije imala akreditive za takve korisničke naloge.</span><span class="sxs-lookup"><span data-stu-id="6b8ee-107">External users cannot sign in to the managed domain since Azure AD Domain Services does not have credentials for such user accounts.</span></span>
4. <span data-ttu-id="6b8ee-108">Ako je korisnički nalog koji utiče na utiču samo na korisnički nalog, uverite se da su korisnici promenili lozinku kada ste omogućili Azure AD Domain usluge domena.</span><span class="sxs-lookup"><span data-stu-id="6b8ee-108">If the affected user account is a cloud-only user account, ensure that users have changed their password after you enabled Azure AD Domain Services.</span></span> <span data-ttu-id="6b8ee-109">Ovaj niz prouzrokuje hašove akreditiva za generisane usluge Azure AD Domain.</span><span class="sxs-lookup"><span data-stu-id="6b8ee-109">This step causes the credential hashes required for Azure AD Domain Services to be generated.</span></span>
5. <span data-ttu-id="6b8ee-110">Ako su korisnici koje utiču na korisnike sinhronizovane iz lokalnog direktorijuma, proverite da li je preporučeno izdanje Azure AD Connect konfigurisano da obavi kompletnu sinhronizaciju.</span><span class="sxs-lookup"><span data-stu-id="6b8ee-110">If the affected user accounts are synchronized from an on-premises directory, verify that the recommended release of Azure AD Connect has been configured to perform a full synchronization.</span></span>
6. <span data-ttu-id="6b8ee-111">Ako problemi budu i dalje u okviru stavke 4. koraka, izvršite sledeće komande sa sinhronizovane mašine:</span><span class="sxs-lookup"><span data-stu-id="6b8ee-111">If issues persists after confirming Step 4, execute the following commands from your sync machine:</span></span>
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     <span data-ttu-id="6b8ee-112">`"net start 'Microsoft Azure AD Sync'"`.</span><span class="sxs-lookup"><span data-stu-id="6b8ee-112">`"net start 'Microsoft Azure AD Sync'"`.</span></span>