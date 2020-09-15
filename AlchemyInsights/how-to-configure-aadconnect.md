---
title: 646 kako se konfiguriše AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704503"
---
# <a name="configure-sync-features"></a><span data-ttu-id="1afb9-102">Konfigurisanje funkcija sinhronizacije</span><span class="sxs-lookup"><span data-stu-id="1afb9-102">Configure sync features</span></span>

<span data-ttu-id="1afb9-103">Azure AD Connect obuhvata nekoliko funkcija koje su podrazumevano omogućene ili koje možete da omogućite kasnije.</span><span class="sxs-lookup"><span data-stu-id="1afb9-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="1afb9-104">Neke funkcije zahtevaju dodatnu konfiguraciju u određenim okruženjima.</span><span class="sxs-lookup"><span data-stu-id="1afb9-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="1afb9-105">Ograničenja [filtriranja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) objekti se sinhronizuju sa uslugom AZURE AD.</span><span class="sxs-lookup"><span data-stu-id="1afb9-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="1afb9-106">Svi korisnici, kontakti, grupe i Windows 10 nalozi su podrazumevano sinhronizovani.</span><span class="sxs-lookup"><span data-stu-id="1afb9-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="1afb9-107">Objekte na osnovu domena, use ili drugih atributa možete da uključite ili isključite.</span><span class="sxs-lookup"><span data-stu-id="1afb9-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="1afb9-108">[Sinhronizacija lozinki](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sinhronizuje hash lozinku iz lokalnog aktivnog direktorijuma u AZURE AD.</span><span class="sxs-lookup"><span data-stu-id="1afb9-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="1afb9-109">To omogućava upravljanju lozinkama na jednoj lokaciji, ali korišćenje iste lozinke u lokalnim i Cloud okruženju.</span><span class="sxs-lookup"><span data-stu-id="1afb9-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="1afb9-110">Budući da je Active Directory autoritativni izvor, možete da koristite sopstvene smernice za lozinku.</span><span class="sxs-lookup"><span data-stu-id="1afb9-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="1afb9-111">[Samouslužno poništavanje lozinke (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) omogućava korisnicima da resetuju sopstvene lozinke u oblaku dok se primenjuju smernice za lokalne lozinke.</span><span class="sxs-lookup"><span data-stu-id="1afb9-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="1afb9-112">[Ponovno upisivanje uređaja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) omogućava da se registrovani uređaji u usluzi AZURE AD vrati u lokalnu fasciklu Active Directory tako da mogu da se koriste za uslovno pristup.</span><span class="sxs-lookup"><span data-stu-id="1afb9-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="1afb9-113">[Sprečavanje slučajno brišu](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) se podrazumevano omogućava da se spreče previše istovremenih brisanja objekata (više od 500 objekata po sinhronizaciji).</span><span class="sxs-lookup"><span data-stu-id="1afb9-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="1afb9-114">Ovu postavku možete da promenite da biste ispunili potrebe organizacije.</span><span class="sxs-lookup"><span data-stu-id="1afb9-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="1afb9-115">[Automatsko nadogradnja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) je podrazumevano omogućena za ekspresne instalacije i pomaže da se osigura da je vaša verzija usluge AZURE AD Connect uvek aktuelna.</span><span class="sxs-lookup"><span data-stu-id="1afb9-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
