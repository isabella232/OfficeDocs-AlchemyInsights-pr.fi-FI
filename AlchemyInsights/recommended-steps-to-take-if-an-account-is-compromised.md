---
title: Suositellut toimet, kun tili on vaarantunut
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom:
- "957"
- "3100016"
ms.openlocfilehash: 08904708dd19104179c3f97f6734d8af725a4512
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/25/2019
ms.locfileid: "36745430"
---
# <a name="recommended-steps-to-take-if-an-account-is-compromised"></a><span data-ttu-id="a2d3e-102">Suositellut toimet, kun tili on vaarantunut</span><span class="sxs-lookup"><span data-stu-id="a2d3e-102">Recommended steps to take if an account is compromised</span></span>

[<span data-ttu-id="a2d3e-103">VIDEO: Väärinkäytetyn Office 365 -tilin korjaaminen</span><span class="sxs-lookup"><span data-stu-id="a2d3e-103">VIDEO: Fixing a compromised Office 365 account</span></span>](https://www.microsoft.com/videoplayer/embed/RE2jvOb?pid=ocpVideo0-innerdiv-oneplayer&amp;postJsllMsg=true&amp;maskLevel=20&amp;autoplay=true)
  
1. <span data-ttu-id="a2d3e-104">[Palauta käyttäjän salasana](https://docs.microsoft.com/office365/admin/add-users/reset-passwords) välittömästi.</span><span class="sxs-lookup"><span data-stu-id="a2d3e-104">[Reset the user's password](https://docs.microsoft.com/office365/admin/add-users/reset-passwords) immediately.</span></span> <span data-ttu-id="a2d3e-105">Älä lähetä uutta salasanaa sähköpostitse loppukäyttäjälle.</span><span class="sxs-lookup"><span data-stu-id="a2d3e-105">Do not communicate the new password through email to the end user.</span></span>

2. <span data-ttu-id="a2d3e-106">Poista kaikki postilaatikkotasolle määritetyt epäilyttävät [edelleenlähetysosoitteet](https://docs.microsoft.com/office365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="a2d3e-106">Remove any suspicious [forwarding addresses](https://docs.microsoft.com/office365/admin/email/configure-email-forwarding) set at the mailbox level.</span></span>

3. <span data-ttu-id="a2d3e-107">Poista kaikki postilaatikkoon määritetyt epäilyttävät [Saapuneet-kansion säännöt](https://support.office.com/article/1433E3A0-7FB0-4999-B536-50E05CB67FED).</span><span class="sxs-lookup"><span data-stu-id="a2d3e-107">Remove any suspicious [inbox rules](https://support.office.com/article/1433E3A0-7FB0-4999-B536-50E05CB67FED) set within the mailbox.</span></span>

4. <span data-ttu-id="a2d3e-108">Jos käyttäjää on estetty lähettämästä sähköpostia, [poista esto siirtymällä kohtaan Rajoitetut käyttäjät](https://protection.office.com/?hash=/restrictedusers).</span><span class="sxs-lookup"><span data-stu-id="a2d3e-108">If the user is blocked from sending email, [go to the Restricted Users to unblock the account](https://protection.office.com/?hash=/restrictedusers).</span></span> <span data-ttu-id="a2d3e-109">Kun esto on poistettu, käyttäjän pitäisi pystyä lähettämään viestejä tunnin kuluessa.</span><span class="sxs-lookup"><span data-stu-id="a2d3e-109">Once done, the user should be able to resume sending messages within 1 hour.</span></span>

5. <span data-ttu-id="a2d3e-110">Poista käyttäjätili kaikista [ryhmistä, joissa käyttäjällä on järjestelmänvalvojan rooli](https://docs.microsoft.com//office365/admin/add-users/assign-admin-roles), kunnes olet varma, ettei tili ole enää vaarantunut.</span><span class="sxs-lookup"><span data-stu-id="a2d3e-110">Remove the user account from any [administrative role groups](https://docs.microsoft.com//office365/admin/add-users/assign-admin-roles) until you are confident that the account is no longer compromised.</span></span>

<span data-ttu-id="a2d3e-111">Artikkelista [Office 365:n tietoturvasuunnitelma](https://docs.microsoft.com//office365/securitycompliance/security-roadmap) saat lisätietoja siitä, miten voit minimoida mahdolliset tietomurrot ja tilien väärinkäytökset tulevaisuudessa.</span><span class="sxs-lookup"><span data-stu-id="a2d3e-111">To minimize the potential of a data breach or a compromised account in the future, we recommend reading our [Office 365 Security best practices article](https://docs.microsoft.com//office365/securitycompliance/security-roadmap).</span></span>
  