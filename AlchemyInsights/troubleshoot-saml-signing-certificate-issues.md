---
title: Rešavanje problema sa certifikatom za SAML potpisivanje
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694448"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a><span data-ttu-id="ccce0-102">Rešavanje problema sa certifikatom za SAML potpisivanje</span><span class="sxs-lookup"><span data-stu-id="ccce0-102">Troubleshoot SAML Signing certificate issues</span></span>

<span data-ttu-id="ccce0-103">Da biste rešili problem sa certifikatom za SEML, obavite sledeće preporučene korake:</span><span class="sxs-lookup"><span data-stu-id="ccce0-103">To resolve SAML Signing certificate issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="ccce0-104">Kada dodate poslovnu aplikaciju koja podržava SSO, Azure će generisati certifikat koji se zove " [certifikat potpisa Sema](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications)".</span><span class="sxs-lookup"><span data-stu-id="ccce0-104">When you add an enterprise application which supports SSO, Azure will generate a certificate which is called the [SAML Signing certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span></span> <span data-ttu-id="ccce0-105">Ovaj certifikat ima datum isteka 3 godine.</span><span class="sxs-lookup"><span data-stu-id="ccce0-105">This certificate has an expiration date of 3 years.</span></span> <span data-ttu-id="ccce0-106">Da biste promenili datum isteka certifikata, pogledajte članak [Prilagođavanje datuma isteka za certifikat Federacije i vraćanje na novi certifikat](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span><span class="sxs-lookup"><span data-stu-id="ccce0-106">To change the expiration date of your certificate, see [Customize the expiration date for your federation certificate and roll it over to a new certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span></span>
2. <span data-ttu-id="ccce0-107">Azure će koristiti ovaj certifikat za potpisivanje SAML Toksa koje je aplikacija zatražila i šalje ga aplikaciji za uspešan SSO.</span><span class="sxs-lookup"><span data-stu-id="ccce0-107">Azure will use this certificate to sign the SAML tokens requested by the application and send it over to the application for a successful SSO.</span></span> <span data-ttu-id="ccce0-108">Da biste ovo dovršili, preuzmite certifikat sa Azure portala i pošaljite ga prodavcu aplikacije da biste dovršili SSO proces.</span><span class="sxs-lookup"><span data-stu-id="ccce0-108">In order for this to complete, download the certificate from the Azure portal and send it to the application vendor to complete the SSO process.</span></span>

<span data-ttu-id="ccce0-109">Pošto ovaj proces dovrši aplikaciju vjeruje ovaj certifikat i svi željeni simboli koje potpiše ovaj certifikat primiće aplikacija.</span><span class="sxs-lookup"><span data-stu-id="ccce0-109">After this process completes your application will trust this certificate and all the SAML tokens signed by this certificate will be accepted by the application.</span></span>

3. <span data-ttu-id="ccce0-110">Ako ovaj certifikat istekne, kreirajte novi certifikat, ažurirajte ga na prodavca aplikacije, a zatim ga učinite aktivnim na stranici Azure.</span><span class="sxs-lookup"><span data-stu-id="ccce0-110">If this certificate expires, create a new certificate, update it to the application vendor and then make it active on the Azure side.</span></span> <span data-ttu-id="ccce0-111">Više informacija potražite u članku obnova [certifikata koji će uskoro isteći](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span><span class="sxs-lookup"><span data-stu-id="ccce0-111">For more information, see [Renew a certificate that will soon expire](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span></span>

> [!NOTE]
> <span data-ttu-id="ccce0-112">Ako certifikat istekne, korisnik neće biti blokiran.</span><span class="sxs-lookup"><span data-stu-id="ccce0-112">If the certificate expires, the user will not be blocked.</span></span>

4. <span data-ttu-id="ccce0-113">[Dodajte e-adresu za obaveštenja](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) koja će biti primljena pre isteka trenutnog certifikata.</span><span class="sxs-lookup"><span data-stu-id="ccce0-113">[Add an email address for notifications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) to be received before the current certificate expires.</span></span>

> [!NOTE]
> <span data-ttu-id="ccce0-114">Korak-4 je opcionalan.</span><span class="sxs-lookup"><span data-stu-id="ccce0-114">Step-4 is an optional one.</span></span>

5. <span data-ttu-id="ccce0-115">Promenite opcije za potpisivanje certifikata za SEML certifikat i algoritam za potpisivanje certifikata.</span><span class="sxs-lookup"><span data-stu-id="ccce0-115">Change an application's SAML certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="ccce0-116">Više informacija potražite u članku [Promena opcija potpisivanja certifikata i potpisivanja algoritma](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span><span class="sxs-lookup"><span data-stu-id="ccce0-116">For more information, see [Change certificate signing options and signing algorithm](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>

