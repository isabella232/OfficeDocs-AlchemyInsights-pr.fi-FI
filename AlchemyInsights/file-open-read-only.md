---
title: Tiedosto avoinna vain luku -tiedostotunnisteena
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: e478572ea82e5ea11bac9fd7eacafb833253235d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813181"
---
# <a name="file-open-read-only"></a><span data-ttu-id="4d124-102">Tiedosto avoinna vain luku -tiedostotunnisteena</span><span class="sxs-lookup"><span data-stu-id="4d124-102">File open read-only</span></span>

<span data-ttu-id="4d124-103">Saatat tietää, että kun avaat tiedostoja, ne avautuvat vain luku -muodossa.</span><span class="sxs-lookup"><span data-stu-id="4d124-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="4d124-104">Joissakin tapauksissa tämä on tietoturvasyistä, kuten silloin, kun avaat tiedostoja Internetistä, ja toisinaan se voi johtua siitä, että asetusta voi muuttaa.</span><span class="sxs-lookup"><span data-stu-id="4d124-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="4d124-105">Seuraavassa on joitakin tilanteita, joissa tiedosto avautuu vain luku -muodossa, ja joitakin vaiheita, joilla voit muuttaa tätä.</span><span class="sxs-lookup"><span data-stu-id="4d124-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="4d124-106">**Virustentorjuntaohjelmani aiheuttaa sen, että virustentorjuntaohjelma avaa vain luku -oikeuden**</span><span class="sxs-lookup"><span data-stu-id="4d124-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="4d124-107">Jotkin virustentorjuntaohjelmat saattavat suojata sinua mahdollisesti epäluotetslta tiedostolta avaamalla ne vain luku -tiedostoina.</span><span class="sxs-lookup"><span data-stu-id="4d124-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="4d124-108">Sinun on ehkä opetella virustentorjuntaohjelman tarjoajaa muokkaamaan näitä asetuksia.</span><span class="sxs-lookup"><span data-stu-id="4d124-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="4d124-109">BitDefenderilla on esimerkiksi sisältöä sovelluksen poikkeusten lisäämisestä täältä: Sovelluksen tai prosessin poissulkemisen lisääminen [Bitdefenderin hallintakeskuksessa.](https://aka.ms/AA6098i)</span><span class="sxs-lookup"><span data-stu-id="4d124-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="4d124-110">**Onko tiedoston ominaisuuksissa vain luku -ominaisuudeksi määritetty?**</span><span class="sxs-lookup"><span data-stu-id="4d124-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="4d124-111">Voit tarkistaa tiedoston ominaisuudet napsauttamalla tiedostoa hiiren kakkospainikkeella ja valitsemalla Ominaisuudet.</span><span class="sxs-lookup"><span data-stu-id="4d124-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="4d124-112">Jos vain luku -määrite on valittuna, voit poistaa sen valinnan ja valita OK.</span><span class="sxs-lookup"><span data-stu-id="4d124-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="4d124-113">**Sisältö on suojatussa näkymässä**</span><span class="sxs-lookup"><span data-stu-id="4d124-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="4d124-114">Internetistä ja muista mahdollisesti epäluotettamattomista paikoista tulevat tiedostot voivat sisältää viruksia, matoja tai muunlaisia haittaohjelmia, jotka voivat vahingoittaa tietokonettasi.</span><span class="sxs-lookup"><span data-stu-id="4d124-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="4d124-115">Tämä koskee usein myös sähköpostiliitteita tai lataamiasi tiedostoja.</span><span class="sxs-lookup"><span data-stu-id="4d124-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="4d124-116">Tietokoneen suojaamiseksi näistä mahdollisesti epäluotettamattomista sijainnista peräisinvat tiedostot avataan suojatussa näkymässä.</span><span class="sxs-lookup"><span data-stu-id="4d124-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="4d124-117">Suojatun näkymän avulla voit lukea tiedoston ja tarkastella sen sisältöä ja vähentää samalla sen riskejä.</span><span class="sxs-lookup"><span data-stu-id="4d124-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="4d124-118">Lisätietoja suojatusta näkymästä ja asetusten muuttuesta on tässä artikkelissa: Mikä on [suojattu näkymä?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="4d124-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="4d124-119">**Onko OneDrive täynnä?**</span><span class="sxs-lookup"><span data-stu-id="4d124-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="4d124-120">Jos tiedosto on tallennettu OneDriveen ja OneDrive-tallennustilasi on täynnä, et voi tallentaa tiedostoa, ennen kuin olet määritetyn tilan alla.</span><span class="sxs-lookup"><span data-stu-id="4d124-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="4d124-121">Voit tarkistaa OneDriven vapaan tilan napsauttamalla ilmoituskeskuksen OneDrive-kuvaketta ja valitsemalla Tallennustilan hallinta. Voit myös valita , kirjautua sisään ja nähdä käytetyn tilan määrän näytön vasemmassa [https://onedrive.live.com](https://onedrive.live.com) alakulmassa.</span><span class="sxs-lookup"><span data-stu-id="4d124-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="4d124-122">**Onko Office aktivoitu?**</span><span class="sxs-lookup"><span data-stu-id="4d124-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="4d124-123">Jos Officea ei ole aktivoitu tai jos tilauksesi on päättynyt, voit olla rajoitetun toiminnan vain luku -tilassa.</span><span class="sxs-lookup"><span data-stu-id="4d124-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="4d124-124">Lisätietoja Officen aktivoimisesta on kohdassa: [Ei käyttöomista -virheet ja aktivointivirheet Officessa.](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)</span><span class="sxs-lookup"><span data-stu-id="4d124-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="4d124-125">**Jos kaikki muu epäonnistuu...**</span><span class="sxs-lookup"><span data-stu-id="4d124-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="4d124-126">Yritä käynnistää tietokone uudelleen</span><span class="sxs-lookup"><span data-stu-id="4d124-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="4d124-127">Office-päivitysten asentaminen</span><span class="sxs-lookup"><span data-stu-id="4d124-127">Install Office updates</span></span>
    
- <span data-ttu-id="4d124-128">Officen Online-korjauksen korjaaminen</span><span class="sxs-lookup"><span data-stu-id="4d124-128">Perform an Online repair of Office</span></span>
    

