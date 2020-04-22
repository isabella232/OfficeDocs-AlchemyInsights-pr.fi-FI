---
title: Tiedosto avaa vain luku -tilassa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: c045188af15fcec0f868eb0e5b399bd1fb42a09a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702771"
---
# <a name="file-open-read-only"></a><span data-ttu-id="f3630-102">Tiedosto avaa vain luku -tilassa</span><span class="sxs-lookup"><span data-stu-id="f3630-102">File open read-only</span></span>

<span data-ttu-id="f3630-103">Saatat huomata, että kun avaat tiedostoja, ne avautuvat vain luku -tilassa.</span><span class="sxs-lookup"><span data-stu-id="f3630-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="f3630-104">Joissakin tapauksissa tämä on lisäturvaa, kuten kun avaat tiedostoja Internetistä, ja muina aikoina, se voi johtua asetus, jota voidaan muuttaa.</span><span class="sxs-lookup"><span data-stu-id="f3630-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="f3630-105">Seuraavassa on joitakin tilanteita, joissa tiedosto avautuu vain luku -tilaan, ja joitakin vaiheita, joiden avulla voit muuttaa sitä.</span><span class="sxs-lookup"><span data-stu-id="f3630-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="f3630-106">**Minun antivirus on aiheuttava heidät jotta auki kuulua- ainoa**</span><span class="sxs-lookup"><span data-stu-id="f3630-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="f3630-107">Jotkin virustentorjuntaohjelmat saattavat suojata sinua mahdollisesti vaarallisilta tiedostoilta avaamalla ne vain luku -tilassa.</span><span class="sxs-lookup"><span data-stu-id="f3630-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="f3630-108">Sinun on ehkä tarkistettava virustentorjuntaohjelman tarjoajalta, miten voit muuttaa näitä asetuksia.</span><span class="sxs-lookup"><span data-stu-id="f3630-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="f3630-109">BitDefender, ajaksi esikuva, has tyytyväinen model after kartuttava ahkeruus poissulkeminen tähän: [Kuinka jotta kartuttaa ahkeruus eli jalostaa poissulkeminen kotona Bitdefender Hallita Keskittyä](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="f3630-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="f3630-110">**Onko tiedoston ominaisuuksiksi määritetty vain luku -asetus?**</span><span class="sxs-lookup"><span data-stu-id="f3630-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="f3630-111">Voit tarkistaa tiedoston ominaisuudet napsauttamalla tiedostoa hiiren kakkospainikkeella ja valitsemalla Ominaisuudet.</span><span class="sxs-lookup"><span data-stu-id="f3630-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="f3630-112">Jos Vain luku -määrite on valittuna, voit poistaa sen valinnan ja valita OK.</span><span class="sxs-lookup"><span data-stu-id="f3630-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="f3630-113">**Sisältö on suojatussa näkymässä**</span><span class="sxs-lookup"><span data-stu-id="f3630-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="f3630-114">Internetistä ja muista mahdollisesti vaarallisista sijainneista peräisin olevat tiedostot voivat sisältää viruksia, matoja tai muita haittaohjelmia, jotka voivat vahingoittaa tietokonettasi.</span><span class="sxs-lookup"><span data-stu-id="f3630-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="f3630-115">Tämä koskee yleensä myös sähköpostiliitteitä tai lataamiasi tiedostoja.</span><span class="sxs-lookup"><span data-stu-id="f3630-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="f3630-116">Tietokoneen suojaamiseksi näiden mahdollisesti vaarallisten sijaintien tiedostot avataan suojatussa näkymässä.</span><span class="sxs-lookup"><span data-stu-id="f3630-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="f3630-117">Suojatun näkymän avulla voit lukea tiedoston ja tarkastella sen sisältöä ja vähentää riskejä.</span><span class="sxs-lookup"><span data-stu-id="f3630-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="f3630-118">Lisätietoja suojatusta näkymästä ja asetusten muuttamisesta on tässä artikkelissa: [Mikä on suojattu näkymä?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="f3630-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="f3630-119">**Onko OneDrive täynnä?**</span><span class="sxs-lookup"><span data-stu-id="f3630-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="f3630-120">Jos tiedosto on tallennettu OneDriveen ja OneDrive-tallennustila on täynnä, et voi tallentaa asiakirjaa, ennen kuin olet varatun tilan alla.</span><span class="sxs-lookup"><span data-stu-id="f3630-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="f3630-121">Voit tarkistaa OneDriven vapaan tilan napsauttamalla ilmaisinkeskuksen OneDrive-kuvaketta ja valitsemalla Tallennustilan [https://onedrive.live.com](https://onedrive.live.com)hallinta tai valitsemalla , kirjaudu sisään ja merkitsemällä muistiin käytetyn tilan näytön vasemmassa alakulmassa.</span><span class="sxs-lookup"><span data-stu-id="f3630-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="f3630-122">**Onko Office aktivoitu?**</span><span class="sxs-lookup"><span data-stu-id="f3630-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="f3630-123">Jos Officea ei ole aktivoitu tai jos tilauksesi on vanhentunut, saatat olla vain luku -tilassa.</span><span class="sxs-lookup"><span data-stu-id="f3630-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="f3630-124">Lisätietoja Officen aktivoimisesta on kohdassa: [Käyttöoikeudettomat tuote- ja aktivointivirheet Officessa](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="f3630-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="f3630-125">**Jos kaikki muu epäonnistuu ...**</span><span class="sxs-lookup"><span data-stu-id="f3630-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="f3630-126">Yritä käynnistää tietokone uudelleen</span><span class="sxs-lookup"><span data-stu-id="f3630-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="f3630-127">Office-päivitysten asentaminen</span><span class="sxs-lookup"><span data-stu-id="f3630-127">Install Office updates</span></span>
    
- <span data-ttu-id="f3630-128">Officen online-korjauksen suorittaminen</span><span class="sxs-lookup"><span data-stu-id="f3630-128">Perform an Online repair of Office</span></span>
    

