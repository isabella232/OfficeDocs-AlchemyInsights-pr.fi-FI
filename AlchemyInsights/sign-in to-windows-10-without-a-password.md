---
title: 'Kirjautuminen Windows 10: een ilman Sala sanaa'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 839b945c457cb007f13605c5b903ded75dadd1d7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719950"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="1a020-102">Kirjautuminen Windows 10: een ilman Sala sanaa</span><span class="sxs-lookup"><span data-stu-id="1a020-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="1a020-103">Jos haluat välttyä kirjoittamasta Sala sanaa Windowsin käynnistyessä, suosittelemme, että käytät jotakin Windows Hello-kirjautumisvaihtoehtoa, kuten PIN-koodi, kasvojentunnistus tai sormen jälki, jos se on käytettävissä.</span><span class="sxs-lookup"><span data-stu-id="1a020-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="1a020-104">Jos haluat todella poistaa suojatun kirjautumisen käytöstä, Lue ohjeet kohdasta "Kirjautuminen Windows 10: een automaattisesti".</span><span class="sxs-lookup"><span data-stu-id="1a020-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="1a020-105">**Secure Windows Hello-vaihto ehdot tilin Sala sanaksi**</span><span class="sxs-lookup"><span data-stu-id="1a020-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="1a020-106">Siirry kohtaan **asetukset > asiakkaat > kirjautumisvaihtoehdot** (tai napsauta [tätä](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="1a020-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="1a020-107">Käytettävissä olevat kirjautumisvaihtoehdot näkyvät luettelossa.</span><span class="sxs-lookup"><span data-stu-id="1a020-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="1a020-108">Esimerkiksi:</span><span class="sxs-lookup"><span data-stu-id="1a020-108">For example:</span></span>

![Kirjautumisvaihtoehdot.](media/sign-in-options.png)

<span data-ttu-id="1a020-110">Voit määrittää sen napsauttamalla tai napauttamalla jotakin vaihto ehtoa.</span><span class="sxs-lookup"><span data-stu-id="1a020-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="1a020-111">Kun seuraavan kerran käynnistät tai avaat Windowsin, voit käyttää uutta vaihto ehtoa Sala sanan sijaan.</span><span class="sxs-lookup"><span data-stu-id="1a020-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="1a020-112">**Kirjautuminen automaattisesti Windows 10: een**</span><span class="sxs-lookup"><span data-stu-id="1a020-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="1a020-113">**Huomautus**: Automaattinen sisäänkirjautuminen on kätevää, mutta se sisältää tieto turva riskin etenkin, jos tieto koneesi on usean henkilön käytettävissä.</span><span class="sxs-lookup"><span data-stu-id="1a020-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="1a020-114">Napsauta tai napauta tehtävä palkin **Käynnistä** -painiketta.</span><span class="sxs-lookup"><span data-stu-id="1a020-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="1a020-115">Kirjoita **netplwiz** ja avaa käyttäjä tunnukset-ikkuna painamalla ENTER-näppäintä.</span><span class="sxs-lookup"><span data-stu-id="1a020-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="1a020-116">Valitse **käyttäjä tilit**-kohdassa tili, johon haluat kirja utua automaattisesti, kun Windows käynnistyy.</span><span class="sxs-lookup"><span data-stu-id="1a020-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="1a020-117">Poista "käyttäjien on annettava käyttäjä nimi ja sala sana, jotta voit käyttää tätä tieto konetta"-valinta neliötä.</span><span class="sxs-lookup"><span data-stu-id="1a020-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Käyttäjien on annettava käyttäjä nimi ja sala sana-vaihto ehto.](media/users-must-enter-username.png)

5. <span data-ttu-id="1a020-119">Valitse **OK**.</span><span class="sxs-lookup"><span data-stu-id="1a020-119">Click **OK**.</span></span> <span data-ttu-id="1a020-120">Sinua pyydetään antamaan ja vahvistamaan valitsemasi tilin sala sana.</span><span class="sxs-lookup"><span data-stu-id="1a020-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="1a020-121">Valitse **OK** , jos haluat viimeistellä.</span><span class="sxs-lookup"><span data-stu-id="1a020-121">Click **OK** to finish.</span></span> <span data-ttu-id="1a020-122">Kun Windows 10 käynnistetään seuraavan kerran, se kirjautuu automaattisesti valitsemaasi tiliin.</span><span class="sxs-lookup"><span data-stu-id="1a020-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
