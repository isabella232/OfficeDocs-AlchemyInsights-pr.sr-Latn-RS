---
title: Sinhronizacija lozinki
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/04/2021
ms.locfileid: "50483082"
---
# <a name="password-synchronization"></a><span data-ttu-id="9085a-102">Sinhronizacija lozinki</span><span class="sxs-lookup"><span data-stu-id="9085a-102">Password synchronization</span></span>

<span data-ttu-id="9085a-103">**Hash sinhronizacija lozinki uopšte ne funkcioniše**</span><span class="sxs-lookup"><span data-stu-id="9085a-103">**Password Hash Synchronization does not work at all**</span></span>

<span data-ttu-id="9085a-104">Neki uobičajeni problemi sa kojima se suočavaju klijenti kada hash sinhronizacija lozinki ne radi su:</span><span class="sxs-lookup"><span data-stu-id="9085a-104">Some common issues customers encounter when Password Hash Synchronization does not work are:</span></span>

- <span data-ttu-id="9085a-105">Korisnički nalog usluge Active Directory koji koristi Azure AD Connect za komunikaciju sa lokalnim aktivnim direktorijumom nije odobren **replikaciju promena direktorijuma** i **replicirati promene direktorijuma sve** dozvole, koje su potrebne za sinhronizaciju lozinki – potrebno je da to rešite tako što ćete ove dozvole dodeliti usluzi Active Directory.</span><span class="sxs-lookup"><span data-stu-id="9085a-105">The Active Directory account used by Azure AD Connect to communicate with on-premises Active Directory is not granted **Replicate Directory Changes** and **Replicate Directory Changes All** permissions, which are required for password synchronization - You need to fix this by granting these permissions to the Active Directory account.</span></span>
- <span data-ttu-id="9085a-106">Sinhronizacija lozinki je onemogućiti kada je administrator promenio metod korisničkog Sign-In iz **sinhronizacije lozinki** na drugu opciju kao što je **Federacija sa AD FS** u ČAROBNJAKU "Azure AD Connect" – to možete da popravite tako što ćete ponovo omogućiti funkciju **hash sinhronizacije lozinki** u čarobnjaku "Azure a.d. za povezivanje".</span><span class="sxs-lookup"><span data-stu-id="9085a-106">Password hash synchronization is disabled after an administrator changed the User Sign-In method from **Password Synchronization** to another option such as **Federation with AD FS** in the Azure AD Connect wizard - You can fix this by re-enabling the **password hash synchronization** feature in the Azure AD Connect wizard.</span></span>
- <span data-ttu-id="9085a-107">Problem sa povezivanjem sa lokalnim aktivnim direktorijumom.</span><span class="sxs-lookup"><span data-stu-id="9085a-107">Connectivity issue with on-premises Active Directory.</span></span> <span data-ttu-id="9085a-108">Na primer, neki kontrolori domena nisu pristupačni na lokaciji Azure AD Connect ili je zabranjen pristup [Portovom](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) zaštitnog zida – potrebno vam je da to rešite tako što ćete osigurati da se veza između AZURE AD Connect server i lokalnog aktivnog direktorijuma ispravno rade.</span><span class="sxs-lookup"><span data-stu-id="9085a-108">For example, some domain controllers are not accessible by Azure AD Connect, or the [ports required](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) are blocked by Firewall - You need to fix this by ensuring that the connectivity between the Azure AD Connect server and the on-premises Active Directory works correctly.</span></span>
- <span data-ttu-id="9085a-109">Azure AD Connect server se trenutno nalazi u režimu postavljanja, što će dovesti do toga da server ne može da gnjavi lozinke-da reši problem, da uradite korake opisane u odeljku [Rešavanje problema sa lozinkom sinhronizacija lozinki sa lokacijom AZURE AD Connect Sync – nijedna lozinka nije sinhronizovana](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="9085a-109">Azure AD Connect server currently being in staging mode, which will result the server not being able to the password hashes - To troubleshoot the issue, follow the steps described in section [Troubleshoot password synchronization with Azure AD Connect sync - No passwords are synchronized](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>

<span data-ttu-id="9085a-110">**Sinhronizacija lozinki ne radi za neke od mojih korisnika**</span><span class="sxs-lookup"><span data-stu-id="9085a-110">**Password Hash Synchronization does not work for some of my users**</span></span>

1. <span data-ttu-id="9085a-111">Ako ste primetili da se hash lozinka ne sinhronizuje za korisnika, koristite zadatak **Rešavanje problema** u okviru AZURE AD povezivanje da biste istražili i rešili problem.</span><span class="sxs-lookup"><span data-stu-id="9085a-111">If you noticed that password hash is not syncing for a user, use the **troubleshoot** task in the Azure AD Connect to investigate and resolve the issue.</span></span> <span data-ttu-id="9085a-112">Obavljanje sledećih zadataka:</span><span class="sxs-lookup"><span data-stu-id="9085a-112">Perform the following tasks:</span></span>

    <span data-ttu-id="9085a-113">Neko.</span><span class="sxs-lookup"><span data-stu-id="9085a-113">a.</span></span> [<span data-ttu-id="9085a-114">Pokreće zadatak rešavanja problema u čarobnjaku</span><span class="sxs-lookup"><span data-stu-id="9085a-114">Run the troubleshooting task in the wizard</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    <span data-ttu-id="9085a-115">-.</span><span class="sxs-lookup"><span data-stu-id="9085a-115">b.</span></span> [<span data-ttu-id="9085a-116">Korišćenje cmdlet problema za istraživanje problema sa hash sinhronizacijom lozinki za određenu upotrebu</span><span class="sxs-lookup"><span data-stu-id="9085a-116">Use the troubleshooting cmdlet to investigate the password hash syncing issue for a specific use</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. <span data-ttu-id="9085a-117">Omogućeno je da korisnik u lokalnom programu Active Directory **Promeni lozinku pri sledećoj prijavljivanju** .</span><span class="sxs-lookup"><span data-stu-id="9085a-117">The on-premises Active Directory User object is enabled for **User must change password at next logon** option.</span></span> <span data-ttu-id="9085a-118">Kada je ova opcija omogućena, korisniku se dodeljuje privremena lozinka i biće vam zatraženo da promenite lozinku na sledećem prijavljivanju.</span><span class="sxs-lookup"><span data-stu-id="9085a-118">When this option is enabled, the user is assigned a temporary password and will be prompted to change the password on the next logon.</span></span> <span data-ttu-id="9085a-119">Azure AD Connect ne sinhronizuje privremene lozinke u Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9085a-119">Azure AD Connect does not synchronize temporary passwords to Azure AD.</span></span>

<span data-ttu-id="9085a-120">Da biste rešili iznad problem, obavite sledeće zadatke:</span><span class="sxs-lookup"><span data-stu-id="9085a-120">To resolve the above issue, perform either of the following tasks:</span></span>

- <span data-ttu-id="9085a-121">Zamolite korisnika da se prijavi u lokalnu aplikaciju (na primer, Windows Desktop) i da promeni lozinku.</span><span class="sxs-lookup"><span data-stu-id="9085a-121">Ask the user to sign in to on-premises application (for example, Windows Desktop) and change the password.</span></span> <span data-ttu-id="9085a-122">Nova lozinka će se sinhronizovati sa uslugom Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9085a-122">The new password will be synchronized to Azure AD.</span></span>
- <span data-ttu-id="9085a-123">Neka administrator ažurira lozinku korisnika bez omogućavanja opcije **korisnik mora da promeni lozinku na sledećoj prijavi** i da deli novu lozinku sa korisnikom.</span><span class="sxs-lookup"><span data-stu-id="9085a-123">Have an administrator update the user's password without enabling the option **User must change password at next logon**, and share the new password with the user.</span></span>

3. <span data-ttu-id="9085a-124">Lokalni objekat aktivnog direktorijuma **nije ispravno konfigurisan** za sinhronizaciju objekta ili sinhronizaciju lozinki.</span><span class="sxs-lookup"><span data-stu-id="9085a-124">The on-premises Active Directory User object is **not correctly configured** for object synchronization or password synchronization.</span></span> <span data-ttu-id="9085a-125">Da biste rešili ovaj problem, slijedite korake opisane u [sinhronizaciji za rešavanje problema sa lozinkama lozinki pomoću usluge Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="9085a-125">To troubleshoot this issue, follow the steps described in the [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>







