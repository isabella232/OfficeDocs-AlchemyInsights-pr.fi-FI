---
title: 'Sormen jälkien lukituksen poistaminen Windows 10: ssä'
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
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795241"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="a9201-102">Sormen jälkien lukituksen poistaminen Windows 10: ssä</span><span class="sxs-lookup"><span data-stu-id="a9201-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="a9201-103">**Windows Hello-sormen jäljen ottaminen käyttöön**</span><span class="sxs-lookup"><span data-stu-id="a9201-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="a9201-104">Jos haluat poistaa Windows 10: n lukituksen sormen jäljen avulla, sinun on määritettävä Windows Hello-sormen jälki lisäämällä (antaen Windowsin oppia tunnistamaan) vähintään yhdellä sormella.</span><span class="sxs-lookup"><span data-stu-id="a9201-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="a9201-105">Siirry kohtaan **asetukset > asiakkaat > kirjautumisvaihtoehdot** (tai napsauta [tätä](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="a9201-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="a9201-106">Käytettävissä olevat kirjautumisvaihtoehdot näkyvät luettelossa.</span><span class="sxs-lookup"><span data-stu-id="a9201-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="a9201-107">Esimerkiksi:</span><span class="sxs-lookup"><span data-stu-id="a9201-107">For example:</span></span>

    ![Kirjautumisvaihtoehdot.](media/sign-in-options.png)

2. <span data-ttu-id="a9201-109">Napsauta tai napauta **Windows Hello-sormen jälki**ja valitse sitten **Määritä**.</span><span class="sxs-lookup"><span data-stu-id="a9201-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="a9201-110">Valitse Windows Hello Setup- **ikkunassa aloittaminen.**</span><span class="sxs-lookup"><span data-stu-id="a9201-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="a9201-111">Sormen jälki tunnistin aktivoituu, ja sinua pyydetään antamaan sormi tunnistimeen:</span><span class="sxs-lookup"><span data-stu-id="a9201-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Sormen jälki tunnistin.](media/fingerprint-sensor.png)

3. <span data-ttu-id="a9201-113">Noudata ohjeita, jotka pyytävät sinua skannaamaan sormella toistuvasti.</span><span class="sxs-lookup"><span data-stu-id="a9201-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="a9201-114">Kun tämä on valmis, voit halutessasi lisätä muita sormia, joita haluat käyttää kirjautumiseen.</span><span class="sxs-lookup"><span data-stu-id="a9201-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="a9201-115">Kun seuraavan kerran kirja udut sisään Windows 10: een, voit käyttää sormen jälkeä.</span><span class="sxs-lookup"><span data-stu-id="a9201-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="a9201-116">**Windows Hello-sormen jälki ei ole käytettävissä kirjautumisvaihtoehtona**</span><span class="sxs-lookup"><span data-stu-id="a9201-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="a9201-117">Jos Windows Hello-sormen jälki ei näy vaihto ehtona **kirjautumisasetuksissa**, Windows ei ole tietoinen tieto koneeseesi liitetystä sormenjälkilukijasta tai skannerista tai järjestelmä käytäntö estää sen käytön (Jos esimerkiksi työpaikkasi hallitsee tieto konettasi).</span><span class="sxs-lookup"><span data-stu-id="a9201-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="a9201-118">Vian määritys:</span><span class="sxs-lookup"><span data-stu-id="a9201-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="a9201-119">Valitse tehtävä palkin **Käynnistä** -painike ja Etsi **laite hallintaa**.</span><span class="sxs-lookup"><span data-stu-id="a9201-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="a9201-120">Avaa **laite hallintaa**napsauttamalla tai napauttamalla.</span><span class="sxs-lookup"><span data-stu-id="a9201-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="a9201-121">Laajenna laite hallinnasta biometriset laitteet napsauttamalla sen Chevron-merkkiä.</span><span class="sxs-lookup"><span data-stu-id="a9201-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Biometriset laitteet.](media/biometric-devices.png)

4. <span data-ttu-id="a9201-123">Sormenjälkiskannerin pitäisi näkyä biometrisenä laitteena, kuten Synaptics WFDI Scanner:</span><span class="sxs-lookup"><span data-stu-id="a9201-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Biometriset laitteet.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="a9201-125">Jos sormenjälkiskannerisi ei näy ja skanneri on integroitu tieto koneeseesi, siirry tieto koneen valmistajan sivustoon.</span><span class="sxs-lookup"><span data-stu-id="a9201-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="a9201-126">Etsi tieto koneen mallin teknisen tuen osasta Windows 10-ohjain asennettavia skannereita varten.</span><span class="sxs-lookup"><span data-stu-id="a9201-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="a9201-127">Jos skanneri on erillään tieto koneesta (liitetty USB-liitännän kautta), Etsi ja asenna Windows 10: n laite ohjain ohjelmisto skannerin mallia varten laitteen valmistajan sivustosta.</span><span class="sxs-lookup"><span data-stu-id="a9201-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
