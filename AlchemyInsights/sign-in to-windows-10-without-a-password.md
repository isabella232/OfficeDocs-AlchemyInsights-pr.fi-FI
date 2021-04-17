---
title: Kirjautuminen Windows 10:ssä ilman salasanaa
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830543"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="b6b3d-102">Kirjautuminen Windows 10:ssä ilman salasanaa</span><span class="sxs-lookup"><span data-stu-id="b6b3d-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="b6b3d-103">Voit välttää salasanan kirjoittamisen Windowsin käynnistyksen yhteydessä käyttämällä Windows Hellon suojattua kirjautumisvaihtoehtoa, kuten PIN-koodia, kasvojentunnistusta tai sormenjälkeä, jos sellainen on käytettävissä.</span><span class="sxs-lookup"><span data-stu-id="b6b3d-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="b6b3d-104">Jos haluat poistaa suojatun kirjautumisen käytöstä, katso alla olevat Windows 10:lle kirjautuminen automaattisesti -ohjeet.</span><span class="sxs-lookup"><span data-stu-id="b6b3d-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="b6b3d-105">**Suojaa Windows Hellon vaihtoehtoja tilin salasanalle**</span><span class="sxs-lookup"><span data-stu-id="b6b3d-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="b6b3d-106">Siirry asetukset **> tilit > kirjautumisasetukset** (tai napsauta [tätä).](ms-settings:signinoptions?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="b6b3d-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="b6b3d-107">Käytettävissä olevat kirjautumisvaihtoehdot tulevat luetteloon.</span><span class="sxs-lookup"><span data-stu-id="b6b3d-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="b6b3d-108">Esimerkiksi:</span><span class="sxs-lookup"><span data-stu-id="b6b3d-108">For example:</span></span>

![Kirjautumisasetukset.](media/sign-in-options.png)

<span data-ttu-id="b6b3d-110">Määritä jokin vaihtoehdoista napsauttamalla tai napauttamalla sitä.</span><span class="sxs-lookup"><span data-stu-id="b6b3d-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="b6b3d-111">Kun seuraavan kerran käynnistät Windowsin tai poistat sen lukituksen, voit käyttää uutta vaihtoehtoa salasanan sijaan.</span><span class="sxs-lookup"><span data-stu-id="b6b3d-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="b6b3d-112">**Windows 10:ksi kirjautuminen automaattisesti**</span><span class="sxs-lookup"><span data-stu-id="b6b3d-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="b6b3d-113">**Huomautus:** Automaattinen kirjautuminen on kätevää, mutta sisältää tietoturvariskin etenkin, jos tietokone on useiden käyttäjien käytettävissä.</span><span class="sxs-lookup"><span data-stu-id="b6b3d-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="b6b3d-114">Napsauta tai napauta **tehtäväpalkin** Käynnistä-painiketta.</span><span class="sxs-lookup"><span data-stu-id="b6b3d-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="b6b3d-115">Kirjoita **netplwiz** ja avaa Käyttäjätilit-ikkuna painamalla Enter-näppäintä.</span><span class="sxs-lookup"><span data-stu-id="b6b3d-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="b6b3d-116">Valitse **Käyttäjätilit-kohdassa** tili, johon haluat kirjautua automaattisesti, kun Windows käynnistyy.</span><span class="sxs-lookup"><span data-stu-id="b6b3d-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="b6b3d-117">Poista käyttäjien on annettava käyttäjänimi ja salasana tämän tietokoneen käyttöä varten -valintaruudun valinta.</span><span class="sxs-lookup"><span data-stu-id="b6b3d-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Käyttäjien on annettava käyttäjänimi- ja salasana-vaihtoehto.](media/users-must-enter-username.png)

5. <span data-ttu-id="b6b3d-119">Valitse **OK**.</span><span class="sxs-lookup"><span data-stu-id="b6b3d-119">Click **OK**.</span></span> <span data-ttu-id="b6b3d-120">Sinua pyydetään antamaan ja vahvistamaan valitsemasi tilin salasana.</span><span class="sxs-lookup"><span data-stu-id="b6b3d-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="b6b3d-121">Lopeta **valitsemalla OK.**</span><span class="sxs-lookup"><span data-stu-id="b6b3d-121">Click **OK** to finish.</span></span> <span data-ttu-id="b6b3d-122">Seuraavan kerran, kun Windows 10 käynnistyy, se kirjautuu automaattisesti valitsemallesi tilille.</span><span class="sxs-lookup"><span data-stu-id="b6b3d-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
