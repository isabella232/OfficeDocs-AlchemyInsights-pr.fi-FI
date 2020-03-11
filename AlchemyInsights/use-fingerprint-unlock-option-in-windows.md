---
title: Sormenjälkilukituksen poistaminen -asetuksen käyttäminen Windows 10:ssä
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 8a5059c722c306ad79811140062cec7f52f31766
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588313"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="80c6f-102">Sormenjälkilukituksen poistaminen -asetuksen käyttäminen Windows 10:ssä</span><span class="sxs-lookup"><span data-stu-id="80c6f-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="80c6f-103">**Windows Hello Fingerprintin ottaminen käyttöön**</span><span class="sxs-lookup"><span data-stu-id="80c6f-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="80c6f-104">Jos haluat poistaa Windows 10:n lukituksen sormenjäljen avulla, sinun on määritettävä Windows Hello Fingerprint lisäämällä (antamalla Windowsin oppia tunnistamaan) vähintään yksi sormi.</span><span class="sxs-lookup"><span data-stu-id="80c6f-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="80c6f-105">Siirry **kohtaan Asetukset > Tilit > kirjautumisasetukset** (tai klikkaa [tästä](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="80c6f-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="80c6f-106">Käytettävissä olevat kirjautumisvaihtoehdot näkyvät luettelossa.</span><span class="sxs-lookup"><span data-stu-id="80c6f-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="80c6f-107">Esimerkki:</span><span class="sxs-lookup"><span data-stu-id="80c6f-107">For example:</span></span>

    ![Kirjautumisasetukset.](media/sign-in-options.png)

2. <span data-ttu-id="80c6f-109">Valitse **Windows Hello Fingerprint**ja valitse sitten **Määritä**.</span><span class="sxs-lookup"><span data-stu-id="80c6f-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="80c6f-110">Valitse Windows Hello -asennusikkunassa **Aloita**.</span><span class="sxs-lookup"><span data-stu-id="80c6f-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="80c6f-111">Sormenjälkitunnistin aktivoituu, ja sinua pyydetään sijoittamaan sormesi anturiin:</span><span class="sxs-lookup"><span data-stu-id="80c6f-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Sormenjälkitunnistin.](media/fingerprint-sensor.png)

3. <span data-ttu-id="80c6f-113">Noudata ohjeita, jotka pyytävät sinua toistuvasti skannata sormesi.</span><span class="sxs-lookup"><span data-stu-id="80c6f-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="80c6f-114">Kun tämä on valmis, voit lisätä muita sormia, joita haluat ehkä käyttää kirjautumiseen.</span><span class="sxs-lookup"><span data-stu-id="80c6f-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="80c6f-115">Kun seuraavan kerran kirjaudut Windows 10:een, voit käyttää sitä käyttämällä sormenjälkeäsi.</span><span class="sxs-lookup"><span data-stu-id="80c6f-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="80c6f-116">**Windows Hello Fingerprint ei ole käytettävissä kirjautumisvaihtoehtona**</span><span class="sxs-lookup"><span data-stu-id="80c6f-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="80c6f-117">Jos Windows Hello Fingerprint -toimintoa ei näytetä **vaihtoehtona kirjautumisasetuksissa**, Windows ei ole tietoinen tietokoneeseen liitetystä sormenjälkilukijasta/skannerista tai että järjestelmäkäytäntö estää sen käytön (jos esimerkiksi tietokoneesi on työpaikan hallinnassa).</span><span class="sxs-lookup"><span data-stu-id="80c6f-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="80c6f-118">Vianmääritys:</span><span class="sxs-lookup"><span data-stu-id="80c6f-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="80c6f-119">Valitse **tehtäväpalkin Aloitus-painike** ja etsi **Laitehallinta**.</span><span class="sxs-lookup"><span data-stu-id="80c6f-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="80c6f-120">Avaa **Laitehallinta**napsauttamalla tai napauttamalla .</span><span class="sxs-lookup"><span data-stu-id="80c6f-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="80c6f-121">Laajenna Laitehallinnassa Biometriset laitteet napsauttamalla sen nuolenta.</span><span class="sxs-lookup"><span data-stu-id="80c6f-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Biometriset laitteet.](media/biometric-devices.png)

4. <span data-ttu-id="80c6f-123">Sormenjälkiskannerin pitäisi olla biometrinen laite, kuten Synaptics WBDI -skanneri:</span><span class="sxs-lookup"><span data-stu-id="80c6f-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Biometriset laitteet.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="80c6f-125">Jos sormenjälkiskanneria ei näytetä ja skanneri on integroitu tietokoneeseen, siirry tietokoneen valmistajan verkkosivustoon.</span><span class="sxs-lookup"><span data-stu-id="80c6f-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="80c6f-126">Etsi asennettavaksi asennettavaskanneri tietokoneen mallista Windows 10 -ohjainta.</span><span class="sxs-lookup"><span data-stu-id="80c6f-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="80c6f-127">Jos skanneri on erillään tietokoneesta (liitetty USB:n kautta), siirry skannerin valmistajan verkkosivustoon ja etsi ja asenna Windows 10 -laiteohjainohjelmisto skannerimallillesi.</span><span class="sxs-lookup"><span data-stu-id="80c6f-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
