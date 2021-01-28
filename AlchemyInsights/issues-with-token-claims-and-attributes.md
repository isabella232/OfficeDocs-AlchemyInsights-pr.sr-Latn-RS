---
title: Problemi sa Simbomnim tvrdnjama i atributima
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
- "9004347"
- "7761"
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035971"
---
# <a name="issues-with-token-claims-and-attributes"></a><span data-ttu-id="e78c3-102">Problemi sa Simbomnim tvrdnjama i atributima</span><span class="sxs-lookup"><span data-stu-id="e78c3-102">Issues with Token Claims and Attributes</span></span>

<span data-ttu-id="e78c3-103">**Ažuriranje, konfigurisanje ili uklanjanje simbola simbola**</span><span class="sxs-lookup"><span data-stu-id="e78c3-103">**Update, configure or remove token claims**</span></span>

1. <span data-ttu-id="e78c3-104">Pomoću Azure aktivnog direktorijuma (Azure AD) možete da [prilagodite tip zahteva za pretenzije](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) na oznaku za odgovor koji primite kada odobrite aplikaciju.</span><span class="sxs-lookup"><span data-stu-id="e78c3-104">By using Azure Active Directory (Azure AD), you can [customize the claim type for the role claim](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) in the response token that you receive after you authorize an app.</span></span>
2. <span data-ttu-id="e78c3-105">Programeri aplikacije mogu da koriste opcionalne zahteve u svojim Azure AD aplikacijama da bi naveli koje tvrdnje žele u željama koje su poslate u aplikaciju.</span><span class="sxs-lookup"><span data-stu-id="e78c3-105">Application developers can use optional claims in their Azure AD applications to specify which claims they want in tokens sent to their application.</span></span> <span data-ttu-id="e78c3-106">Više informacija potražite u članku [obezbeđivanje opcionalnih tvrdnji za aplikaciju](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span><span class="sxs-lookup"><span data-stu-id="e78c3-106">For more information, see [Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span></span>
3. <span data-ttu-id="e78c3-107">[Podesite grupne zahteve za aplikacije pomoću usluge Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span><span class="sxs-lookup"><span data-stu-id="e78c3-107">[Configure group claims for applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span></span>
4. <span data-ttu-id="e78c3-108">Ako koristite Nesmetna jedinstveno prijavljivanje u aplikaciji, pogledajte članak [Prilagođavanje tvrdnji izdatih u znaku semla za preduzeća](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span><span class="sxs-lookup"><span data-stu-id="e78c3-108">If using Seamless Single Sign-on in your application, see [customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span></span>

<span data-ttu-id="e78c3-109">**Mapiranje atributa potraživanja**</span><span class="sxs-lookup"><span data-stu-id="e78c3-109">**Claims Attribute Mapping**</span></span>

1. <span data-ttu-id="e78c3-110">Da biste konfigurisali smernice za mapiranje potraživanja pomoću programa PowerShell, pogledajte članak [Prilagođavanje tvrdnji koje se automatski emituje za određenu aplikaciju u zakupcu (pregled)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span><span class="sxs-lookup"><span data-stu-id="e78c3-110">To configure claims mapping policy using PowerShell, see [Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span></span>
2. <span data-ttu-id="e78c3-111">Atributi proširenja šeme direktorijuma obezbeđuju način skladištenja dodatnih podataka u usluzi Azure Active Directory na korisničkim objektima i drugim objektima direktorijuma kao što su grupe, detalji zakupca, direktori usluga.</span><span class="sxs-lookup"><span data-stu-id="e78c3-111">Directory schema extension attributes provide a way to store additional data in Azure Active Directory on user objects and other directory objects such as groups, tenant details, service principals.</span></span> <span data-ttu-id="e78c3-112">Samo produženi atributi na korisničkim objektima mogu da se koriste za emitovanje tvrdnji u aplikacijama.</span><span class="sxs-lookup"><span data-stu-id="e78c3-112">Only extension attributes on user objects can be used for emitting claims to applications.</span></span> <span data-ttu-id="e78c3-113">[Korišćenje atributa proširenja šeme direktorijuma u tvrdnjama](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) objašnjava kako se koriste atributi proširenja šeme direktorijuma za slanje korisničkih podataka u aplikacije u zahtevima za Token.</span><span class="sxs-lookup"><span data-stu-id="e78c3-113">[Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) describes how to use directory schema extension attributes for sending user data to applications in token claims.</span></span>

<span data-ttu-id="e78c3-114">Više informacija o simbomnoj tvrdnji potražite u članku:</span><span class="sxs-lookup"><span data-stu-id="e78c3-114">For more information on token claims, see:</span></span>

- [<span data-ttu-id="e78c3-115">Potraživanja u Access tokenima</span><span class="sxs-lookup"><span data-stu-id="e78c3-115">Claims in access tokens</span></span>](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [<span data-ttu-id="e78c3-116">Zahtevi u id_token</span><span class="sxs-lookup"><span data-stu-id="e78c3-116">Claims in an id_token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- <span data-ttu-id="e78c3-117">[Tvrdnje](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) koje možete OČEKIVATI od ID-ova i Access tokena koje izda AZURE AD B2C</span><span class="sxs-lookup"><span data-stu-id="e78c3-117">[Claims](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) that you can expect in ID tokens and access tokens issued by Azure AD B2C</span></span>
- [<span data-ttu-id="e78c3-118">Zahtev za SEML Token</span><span class="sxs-lookup"><span data-stu-id="e78c3-118">SAML token claims reference</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
