---
title: Kirjautuminen Windows 10:een ilman salasanaa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1f325eb7afb1e88457296e8187f8ba6dff2ebfe0
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588278"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="81060-102">Kirjautuminen Windows 10:een ilman salasanaa</span><span class="sxs-lookup"><span data-stu-id="81060-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="81060-103">Jotta sinun ei tarvitsisi kirjoittaa salasanaa Windowsin käynnistyksen yhteydessä, suosittelemme, että käytät jotakin Windows Hello -suojatun kirjautumisvaihtoehdon, kuten PIN-koodin, kasvojentunnistuksen tai sormenjäljen, jos se on käytettävissä.</span><span class="sxs-lookup"><span data-stu-id="81060-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="81060-104">Jos haluat todella poistaa suojatun kirjautumisen käytöstä, katso alla olevat "Kirjaudu automaattisesti Windows 10:een" -ohjeet.</span><span class="sxs-lookup"><span data-stu-id="81060-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="81060-105">**Suojaa Windows Hello vaihtoehtoja tilin salasana**</span><span class="sxs-lookup"><span data-stu-id="81060-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="81060-106">Siirry **kohtaan Asetukset > Tilit > kirjautumisasetukset** (tai klikkaa [tästä](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="81060-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="81060-107">Käytettävissä olevat kirjautumisvaihtoehdot näkyvät luettelossa.</span><span class="sxs-lookup"><span data-stu-id="81060-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="81060-108">Esimerkki:</span><span class="sxs-lookup"><span data-stu-id="81060-108">For example:</span></span>

![Kirjautumisasetukset.](media/sign-in-options.png)

<span data-ttu-id="81060-110">Määritä se napsauttamalla tai napauttamalla jotakin vaihtoehtoa.</span><span class="sxs-lookup"><span data-stu-id="81060-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="81060-111">Kun seuraavan kerran käynnistät Windowsin tai avaat sen lukituksen, voit käyttää uutta vaihtoehtoa salasanan sijaan.</span><span class="sxs-lookup"><span data-stu-id="81060-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="81060-112">**Kirjautuminen automaattisesti Windows 10:een**</span><span class="sxs-lookup"><span data-stu-id="81060-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="81060-113">**Huomautus:** Automaattinen sisäänkirjautuminen on kätevää, mutta siinä on tietoturvariski, varsinkin jos useat henkilöt ovat käytettävissä tietokoneessasi.</span><span class="sxs-lookup"><span data-stu-id="81060-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="81060-114">Napsauta tai napauta **tehtäväpalkin** Käynnistä-painiketta.</span><span class="sxs-lookup"><span data-stu-id="81060-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="81060-115">Kirjake **netplwiz** ja humauttaa Astua avain jotta auki Käyttäjä Selittää asian akkuna.</span><span class="sxs-lookup"><span data-stu-id="81060-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="81060-116">Valitse **Käyttäjätilit**-kohdassa tili, johon haluat kirjautua automaattisesti, kun Windows käynnistyy.</span><span class="sxs-lookup"><span data-stu-id="81060-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="81060-117">Poista "Käyttäjien on annettava käyttäjänimi ja salasana käyttää tätä tietokonetta" -valintaruudun valinta.</span><span class="sxs-lookup"><span data-stu-id="81060-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Käyttäjien on annettava käyttäjänimi ja salasana -vaihtoehto.](media/users-must-enter-username.png)

5. <span data-ttu-id="81060-119">Valitse **OK**.</span><span class="sxs-lookup"><span data-stu-id="81060-119">Click **OK**.</span></span> <span data-ttu-id="81060-120">Sinua pyydetään antamaan ja vahvistamaan valitsemasi tilin salasana.</span><span class="sxs-lookup"><span data-stu-id="81060-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="81060-121">Lopeta valitsemalla **OK.**</span><span class="sxs-lookup"><span data-stu-id="81060-121">Click **OK** to finish.</span></span> <span data-ttu-id="81060-122">Kun Windows 10 käynnistyy seuraavan kerran, se kirjautuu automaattisesti valitsemaasi tiliin.</span><span class="sxs-lookup"><span data-stu-id="81060-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
