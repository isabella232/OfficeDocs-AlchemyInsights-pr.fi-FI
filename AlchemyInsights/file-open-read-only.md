---
title: Tiedosto avoinna vain luku-tilassa
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 2fdb4f048c2bee022a49c2cca2ce9770f42a87a2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745577"
---
# <a name="file-open-read-only"></a><span data-ttu-id="06588-102">Tiedosto avoinna vain luku-tilassa</span><span class="sxs-lookup"><span data-stu-id="06588-102">File open read-only</span></span>

<span data-ttu-id="06588-103">Saatat huomata, että kun avaat tiedostoja, ne avautuvat vain luku-tilassa.</span><span class="sxs-lookup"><span data-stu-id="06588-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="06588-104">Joissain tapa uksissa tämä on lisäturvallisuus, esimerkiksi kun avaat tiedostoja Inter netistä, ja toisinaan se voi johtua muutetuista asetuksista.</span><span class="sxs-lookup"><span data-stu-id="06588-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="06588-105">Seuraavassa on joitakin tilanteita, joissa tiedosto avautuu vain luku-tilassa, ja joitakin vaiheita, jotka voit tehdä sen muuttamiseksi.</span><span class="sxs-lookup"><span data-stu-id="06588-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="06588-106">**Virustentorjuntaohjelmasi aiheuttaa niiden avaamisen vain luku-tilassa**</span><span class="sxs-lookup"><span data-stu-id="06588-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="06588-107">Jotkin virustentorjuntaohjelmat saattavat suojata sinua mahdollisesti haitallisista tiedostoista avaamalla ne vain luku-tilassa.</span><span class="sxs-lookup"><span data-stu-id="06588-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="06588-108">Sinun on ehkä tarkistettava virustentorjuntaohjelmasi tarjoajalta, miten voit muuttaa näitä asetuksia.</span><span class="sxs-lookup"><span data-stu-id="06588-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="06588-109">BitDefender-sovelluksessa on esimerkiksi sisältöä sovelluksen poissulkemisten lisäämiseen: [sovellusten tai prosessien poissulkemisten lisääminen BitDefender Control Centerissä](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="06588-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="06588-110">**Onko tiedoston ominaisuudet vain luku-tilassa?**</span><span class="sxs-lookup"><span data-stu-id="06588-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="06588-111">Voit tarkistaa tiedoston ominaisuudet napsauttamalla tiedostoa hiiren kakkos painikkeella ja valitsemalla Ominaisuudet.</span><span class="sxs-lookup"><span data-stu-id="06588-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="06588-112">Jos vain luku-määrite on valittuna, voit poistaa sen valinnan ja valita OK.</span><span class="sxs-lookup"><span data-stu-id="06588-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="06588-113">**Sisältö on suojatussa näkymässä**</span><span class="sxs-lookup"><span data-stu-id="06588-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="06588-114">Tiedostot Inter netistä ja muista mahdollisesti vaarallisista sijainneista voivat sisältää viruksia, matoja tai muunlaisia haitta ohjelmia, jotka voivat vahingoittaa tieto konettasi.</span><span class="sxs-lookup"><span data-stu-id="06588-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="06588-115">Tämä koskee usein myös ladattuja Sähkö posti liitteitä tai tiedostoja.</span><span class="sxs-lookup"><span data-stu-id="06588-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="06588-116">Tieto koneen suojaamiseksi tiedostot näistä mahdollisesti vaarallisista sijainneista avataan suojatussa näkymässä.</span><span class="sxs-lookup"><span data-stu-id="06588-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="06588-117">Suojatun näkymän avulla voit lukea tiedoston ja nähdä sen sisällön ja pienentää riskejä.</span><span class="sxs-lookup"><span data-stu-id="06588-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="06588-118">Lisä tietoja Suojatusta näkymästä ja asetusten muuttamisesta on tässä artikkelissa: [mikä on suojattu näkymä?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="06588-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="06588-119">**Onko OneDrive täynnä?**</span><span class="sxs-lookup"><span data-stu-id="06588-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="06588-120">Jos tiedosto on tallennettu OneDriveen ja OneDrive-tallennus tilasi on täynnä, et voi tallentaa tiedostoa, ennen kuin olet varatun tilan alapuolella.</span><span class="sxs-lookup"><span data-stu-id="06588-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="06588-121">Voit tarkistaa OneDrive-tila uksen vapaan tilan napsauttamalla ilmaisin keskuksessa olevaa OneDrive-kuvaketta ja valitsemalla Hallitse tallennus tilaa, tai voit siirtyä kohtaan [https://onedrive.live.com](https://onedrive.live.com) , kirja utua sisään ja huomata käytetyn tilan määrän näytön vasemmassa alakulmassa.</span><span class="sxs-lookup"><span data-stu-id="06588-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="06588-122">**Onko Office aktivoitu?**</span><span class="sxs-lookup"><span data-stu-id="06588-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="06588-123">Jos Officea ei ole aktivoitu tai jos tilauksesi on vanhentunut, voit olla vain luku-tilassa.</span><span class="sxs-lookup"><span data-stu-id="06588-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="06588-124">Lisä tietoja Officen Akti voinnista on kohdassa Office-käyttö oikeuden [Lisensoimattomat tuote-ja aktivointi virheet](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="06588-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="06588-125">**Jos mikään muu ei auta...**</span><span class="sxs-lookup"><span data-stu-id="06588-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="06588-126">Käynnistä tieto kone uudelleen</span><span class="sxs-lookup"><span data-stu-id="06588-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="06588-127">Office-päivitysten asentaminen</span><span class="sxs-lookup"><span data-stu-id="06588-127">Install Office updates</span></span>
    
- <span data-ttu-id="06588-128">Officen online-korjauksen suorittaminen</span><span class="sxs-lookup"><span data-stu-id="06588-128">Perform an Online repair of Office</span></span>
    

