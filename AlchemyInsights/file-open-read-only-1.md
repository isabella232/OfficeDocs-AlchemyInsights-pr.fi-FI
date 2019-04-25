---
title: Avaa vain luku-tiedosto
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 69705825-723a-4c1e-ae85-d16b5051d2fe
ms.openlocfilehash: 117b1e24d6250a1d5eb092a01a0d5146d09ea2e5
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32401634"
---
# <a name="file-open-read-only"></a><span data-ttu-id="81b67-102">Avaa vain luku-tiedosto</span><span class="sxs-lookup"><span data-stu-id="81b67-102">File open read-only</span></span>

<span data-ttu-id="81b67-103">Saatat huomata, että kun avaat tiedostoja, avaamista vain luku-muodossa.</span><span class="sxs-lookup"><span data-stu-id="81b67-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="81b67-104">Joissakin tapauksissa tämä on suojauksen, kuten kun avaat tiedostoja Internetistä ja muina aikoina, se johtua, joka voi muuttaa asetusta.</span><span class="sxs-lookup"><span data-stu-id="81b67-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="81b67-105">Seuraavassa on joitakin skenaarioita, jossa tiedosto avataan vain luku-tilassa ja voit muuttaa joitakin toimia.</span><span class="sxs-lookup"><span data-stu-id="81b67-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="81b67-106">**Oma antivirus aiheuttaa ne Avaa vain luku-tilassa**</span><span class="sxs-lookup"><span data-stu-id="81b67-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="81b67-107">Jotkin virustentorjuntaohjelmat saattavat suojaamaan mahdollisen tietoturvariskin sisältävien tiedostojen avaamalla ne vain luku-tilassa.</span><span class="sxs-lookup"><span data-stu-id="81b67-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="81b67-108">Saatat joutua Tarkista virustentorjuntaohjelman toimittajalta lisätietoja näiden asetusten kanssa.</span><span class="sxs-lookup"><span data-stu-id="81b67-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="81b67-109">BitDefender, esimerkiksi, on sisällön lisäämisestä sovelluksen poikkeukset tähän: [Voit lisätä sovelluksen tai prosessin poissulkemiset Bitdefender Control Center](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span><span class="sxs-lookup"><span data-stu-id="81b67-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span></span>
  
 <span data-ttu-id="81b67-110">**Tiedosto-ominaisuudet määritetään vain luku-tilassa?**</span><span class="sxs-lookup"><span data-stu-id="81b67-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="81b67-111">Voit tarkistaa tiedoston ominaisuuksia napsauttamalla tiedostoa hiiren kakkospainikkeella ja valitsemalla Ominaisuudet.</span><span class="sxs-lookup"><span data-stu-id="81b67-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="81b67-112">Jos vain luku-määrite on valittuna, voit poista sen valinta ja valitse OK.</span><span class="sxs-lookup"><span data-stu-id="81b67-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="81b67-113">**Sisältö on suojattu näkymä**</span><span class="sxs-lookup"><span data-stu-id="81b67-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="81b67-114">Internetistä ja muista paikoista mahdollisesti haitalliset tiedostot voivat sisältää viruksia, matoja tai muunlaisia haittaohjelmia, jotka voivat vahingoittaa tietokonettasi.</span><span class="sxs-lookup"><span data-stu-id="81b67-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="81b67-115">Näin myös usein sähköpostin liitetiedostot ja lataamasi tiedostot.</span><span class="sxs-lookup"><span data-stu-id="81b67-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="81b67-116">Suojaa tietokoneesi näistä sijainneista mahdollisesti haitalliset tiedostot avataan suojatussa näkymässä.</span><span class="sxs-lookup"><span data-stu-id="81b67-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="81b67-117">Suojatun näkymän avulla voit lukea tiedoston ja tarkastella sen sisältöä, pienentäen riskit.</span><span class="sxs-lookup"><span data-stu-id="81b67-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="81b67-118">Lisätietoja suojatun näkymän ja asetusten muuttamisesta on tässä artikkelissa: [Mikä on suojattu näkymä?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="81b67-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="81b67-119">**OneDrive on täynnä?**</span><span class="sxs-lookup"><span data-stu-id="81b67-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="81b67-120">Jos tiedosto on tallennettu OneDrive ja OneDrive-tallennustila on täynnä, et voi tallentaa asiakirjan, kunnes olet kohdassa varattuun tilaan.</span><span class="sxs-lookup"><span data-stu-id="81b67-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="81b67-121">Voit tarkistaa vapaan tilan OneDrive OneDrive kuvaketta ilmoitus keskellä klikkaamalla ja valitsemalla Hallitse varastointi, tai voit siirtyä [http://onedrive.live.com](http://onedrive.live.com), kirjaudu sisään ja Huomaa näytön vasemmassa alaosassa käytetyn levytilan määrän.</span><span class="sxs-lookup"><span data-stu-id="81b67-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [http://onedrive.live.com](http://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="81b67-122">**Office on aktivoitu?**</span><span class="sxs-lookup"><span data-stu-id="81b67-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="81b67-123">Jos Office ei ole aktivoitu tai jos tilauksesi on vanhentunut, voi olla vain luku-rajoitetun toiminnan tilassa.</span><span class="sxs-lookup"><span data-stu-id="81b67-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="81b67-124">Lisätietoja siitä, kuinka voit aktivoida Office: [varastettu tuote ja Office activation virheitä](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="81b67-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="81b67-125">**Jos mikään muu ei auta...**</span><span class="sxs-lookup"><span data-stu-id="81b67-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="81b67-126">Käynnistä tietokone uudelleen</span><span class="sxs-lookup"><span data-stu-id="81b67-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="81b67-127">Asenna Office-päivitykset</span><span class="sxs-lookup"><span data-stu-id="81b67-127">Install Office updates</span></span>
    
- <span data-ttu-id="81b67-128">Suorita Office Online korjauspalvelut</span><span class="sxs-lookup"><span data-stu-id="81b67-128">Perform an Online repair of Office</span></span>
    

