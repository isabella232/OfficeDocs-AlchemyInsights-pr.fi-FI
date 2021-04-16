---
title: Sormenjälkilukituksen käyttö Windows 10:ssä
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
- "9001689"
- "3765"
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796674"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="66324-102">Sormenjälkilukituksen käyttö Windows 10:ssä</span><span class="sxs-lookup"><span data-stu-id="66324-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="66324-103">**Windows Hellon sormenjäljen ottaminen käyttöön**</span><span class="sxs-lookup"><span data-stu-id="66324-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="66324-104">Jotta voit poistaa Windows 10:n lukituksen sormenjäljen avulla, sinun on määritettävä Windows Hello Fingerprint lisäämällä (antamalla Windowsin opetella tunnistamaan) vähintään yksi sormi.</span><span class="sxs-lookup"><span data-stu-id="66324-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="66324-105">Siirry asetukset **> tilit > kirjautumisasetukset** (tai napsauta [tätä).](ms-settings:signinoptions?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="66324-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="66324-106">Käytettävissä olevat kirjautumisvaihtoehdot tulevat luetteloon.</span><span class="sxs-lookup"><span data-stu-id="66324-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="66324-107">Esimerkiksi:</span><span class="sxs-lookup"><span data-stu-id="66324-107">For example:</span></span>

    ![Kirjautumisasetukset.](media/sign-in-options.png)

2. <span data-ttu-id="66324-109">Napsauta tai napauta **Windows Hellon sormenjälkeä** ja **valitse sitten Määritä**.</span><span class="sxs-lookup"><span data-stu-id="66324-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="66324-110">Valitse Windows Hellon määritysikkunassa **Aloita käyttö.**</span><span class="sxs-lookup"><span data-stu-id="66324-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="66324-111">Sormenjälkitunnistin aktivoituu, ja sinua pyydetään asetamaan sormesi tunnistimeen:</span><span class="sxs-lookup"><span data-stu-id="66324-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Sormenjälkitunnistin.](media/fingerprint-sensor.png)

3. <span data-ttu-id="66324-113">Noudata ohjeita, jotka pyytävät sinua skannaamaan sormella toistuvasti.</span><span class="sxs-lookup"><span data-stu-id="66324-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="66324-114">Kun tämä on valmis, voit lisätä muita sormia, joita haluat ehkä käyttää kirjautumiseen.</span><span class="sxs-lookup"><span data-stu-id="66324-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="66324-115">Kun seuraavan kerran kirjaudut Windows 10:ssä, voit käyttää sormenjälkeäsi.</span><span class="sxs-lookup"><span data-stu-id="66324-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="66324-116">**Windows Hellon sormenjälki ei ole käytettävissä kirjautumisvaihtoehtona**</span><span class="sxs-lookup"><span data-stu-id="66324-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="66324-117">Jos Windows Hello Fingerprint ei näy kirjautumisasetusten vaihtoehtona, Windows ei ole tietoinen tietokoneeseen liitetystä sormenjälkilukijasta tai että järjestelmäkäytäntö estää sen käytön (jos esimerkiksi työpaikkasi hallinnoi tietokonetta).</span><span class="sxs-lookup"><span data-stu-id="66324-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="66324-118">Vianmääritys:</span><span class="sxs-lookup"><span data-stu-id="66324-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="66324-119">Valitse **tehtäväpalkin** Käynnistä-painike ja etsi **Laitehallinta.**</span><span class="sxs-lookup"><span data-stu-id="66324-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="66324-120">Avaa Laitehallinta **napsauttamalla tai napauttamalla**.</span><span class="sxs-lookup"><span data-stu-id="66324-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="66324-121">Laajenna Laitehallinnassa Biometriset laitteet napsauttamalla sen chevron-kohtaa.</span><span class="sxs-lookup"><span data-stu-id="66324-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Biometriset laitteet.](media/biometric-devices.png)

4. <span data-ttu-id="66324-123">Sormenjälkiskannerilla pitäisi olla biometrinen laite, kuten Synaptics WBDI -skanneri:</span><span class="sxs-lookup"><span data-stu-id="66324-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Biometriset laitteet.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="66324-125">Jos sormenjälkilukija ei ole näkyvissä ja skanneri on integroitu tietokoneeseen, siirry tietokoneen valmistajan sivustoon.</span><span class="sxs-lookup"><span data-stu-id="66324-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="66324-126">Etsi PC-mallin teknisestä tuesta Windows 10 -ohjainta, jonka voit asentaa.</span><span class="sxs-lookup"><span data-stu-id="66324-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="66324-127">Jos skanneri on erillinen tietokoneesta (USB:n kautta liitettynä), etsi ja asenna Windows 10 :n laiteohjainohjelmisto skannerimallia varten skannerivalmistajan sivustosta.</span><span class="sxs-lookup"><span data-stu-id="66324-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
