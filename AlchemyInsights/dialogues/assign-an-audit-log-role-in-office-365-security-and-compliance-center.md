---
title: Dodeljivanje uloge evidencije nadzora u sistemu Office 365 Security & centar za usaglašenost
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7363"
- "9000722"
ms.openlocfilehash: 0eb470b6c17def5517db2f866ef40898b36662ed
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/05/2021
ms.locfileid: "50526528"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a><span data-ttu-id="2d64c-102">Dodeljivanje uloge evidencije nadzora u sistemu Office 365 Security & centar za usaglašenost</span><span class="sxs-lookup"><span data-stu-id="2d64c-102">Assign an Audit Log role in the Office 365 Security & Compliance Center</span></span>

<span data-ttu-id="2d64c-103">Da biste pretražili Office 365 evidenciju nadzora, administratoru mora biti dodeljena uloga **samo za prikaz nadgledanja za praćenje** ili uloga za **evidentiranje** u usluzi Exchange online.</span><span class="sxs-lookup"><span data-stu-id="2d64c-103">To search the Office 365 audit log, an administrator must be assigned the **View-Only Audit Logs** role or the **Audit Logs** role in Exchange Online.</span></span> <span data-ttu-id="2d64c-104">Ove uloge su podrazumevano dodeljene grupama za upravljanje usaglašenosti i grupama za upravljanje organizacijama.</span><span class="sxs-lookup"><span data-stu-id="2d64c-104">These roles are assigned to the Compliance Management and Organization Management role groups by default.</span></span> <span data-ttu-id="2d64c-105">Globalni administratori u sistemu Office 365 i Microsoft 365 automatski se dodaju kao članovi grupe za upravljanje organizacijom.</span><span class="sxs-lookup"><span data-stu-id="2d64c-105">Global administrators in Office 365 and Microsoft 365 are automatically added as members of the Organization Management role group.</span></span>

<span data-ttu-id="2d64c-106">Da biste omogućili korisniku da pretražuje minimalan nivo privilegija, kreirajte prilagođenu grupu uloga u usluzi Exchange online, Dodajte uloge za **Praćenje samo za prikaz** ili ulogu **evidentiranja** , a zatim dodajte korisnika kao člana nove grupe uloga.</span><span class="sxs-lookup"><span data-stu-id="2d64c-106">To enable a user to search with the minimum level of privileges, create a custom role group in Exchange Online, add the **View-Only Audit Logs** role or **Audit Logs** role, and then add the user as a member of the new role group.</span></span>

<span data-ttu-id="2d64c-107">Više informacija potražite u članku [Upravljanje grupama uloga u usluzi Exchange online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) i [pretraživanje evidencije nadzora u centru za zaštitu &](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span><span class="sxs-lookup"><span data-stu-id="2d64c-107">For more information, see [Manage role groups in Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) and [Search the audit log in the Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>