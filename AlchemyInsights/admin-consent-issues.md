---
title: Problemi sa administratorom administracije
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901510"
---
# <a name="admin-consent-issues"></a><span data-ttu-id="3c7f0-102">Problemi sa administratorom administracije</span><span class="sxs-lookup"><span data-stu-id="3c7f0-102">Admin consent issues</span></span>

1. <span data-ttu-id="3c7f0-103">Omogućavanje [toka posla "administrator](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) " da biste omogućili korisnicima da zahtevaju odobravanje administratora direktno sa ekrana "pristanak".</span><span class="sxs-lookup"><span data-stu-id="3c7f0-103">Enable the [admin consent workflow](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) to allow users to request administrator approval directly from the consent screen.</span></span>

1. <span data-ttu-id="3c7f0-104">Ako vi ili korisnici aplikacije vidite neočekivane greške tokom procesa pristanka, pogledajte ovaj članak za korake za rešavanje problema: [neočekivanu grešku prilikom izvršavanja pristanka na aplikaciju](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span><span class="sxs-lookup"><span data-stu-id="3c7f0-104">If you or your application's users are seeing unexpected errors during the consent process, see this article for troubleshooting steps: [Unexpected error when performing consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>

1. <span data-ttu-id="3c7f0-105">Saznajte više o [saglasnosti administracije na Microsoft platformi identiteta](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), kako funkcioniše [odziv za pristanak](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) i kako da [procenite zahtev za saglasnost za administratore za celu zakupcu](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span><span class="sxs-lookup"><span data-stu-id="3c7f0-105">Learn more about [Admin consent on the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), how the [consent prompt](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) works, and how to [evaluate a request for tenant-wide admin consent](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span></span>

1. <span data-ttu-id="3c7f0-106">Aplikacije koje se integrišu sa Microsoft platformom za identifikaciju slede model identiteta koji korisnicima i administratori pružaju kontrolu nad načinom na koji se podaci mogu pristupiti.</span><span class="sxs-lookup"><span data-stu-id="3c7f0-106">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="3c7f0-107">Primena modela autorizacije ažurirana je na krajnjoj tački Microsoft platforme identiteta i menja kako aplikacija mora da komunicira sa Microsoft platformom identiteta.</span><span class="sxs-lookup"><span data-stu-id="3c7f0-107">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint, and it changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="3c7f0-108">Pogledajte [dozvole i pristanak na krajnje tačke Microsoft platforme za identifikaciju](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) za pregled ovog modela autorizacije, uključujući opsege, dozvole i saglasnost.</span><span class="sxs-lookup"><span data-stu-id="3c7f0-108">See [Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) for an overview of this authorization model, including scopes, permissions, and consent.</span></span>