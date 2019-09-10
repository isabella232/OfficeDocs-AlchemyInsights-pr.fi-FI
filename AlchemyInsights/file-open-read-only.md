---
title: Tiedoston avaaminen vain luku-tilassa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: eddd427b159a782abf53adda934de8b15a02ed00
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822231"
---
# <a name="file-open-read-only"></a><span data-ttu-id="12143-102">Tiedoston avaaminen vain luku-tilassa</span><span class="sxs-lookup"><span data-stu-id="12143-102">File open read-only</span></span>

<span data-ttu-id="12143-103">Saatat huomata, että kun avaat tiedostoja, ne avautuvat vain luku-muodossa.</span><span class="sxs-lookup"><span data-stu-id="12143-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="12143-104">Joissakin tapa uksissa tämä on lisä suojausta, esimerkiksi kun avaat tiedostoja Inter netistä, ja toisinaan se voi johtua asetuksesta, jota voidaan muuttaa.</span><span class="sxs-lookup"><span data-stu-id="12143-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="12143-105">Seuraavassa on joitakin tilanteita, joissa tiedosto avaa vain luku-tilan ja joitakin vaiheita, joita voit muuttaa.</span><span class="sxs-lookup"><span data-stu-id="12143-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="12143-106">**Virustentorjuntaohjelmaani aiheuttaa sen, että he avaavat vain luku-**</span><span class="sxs-lookup"><span data-stu-id="12143-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="12143-107">Jotkin virustentorjuntaohjelmat saattavat suojata sinua mahdollisesti vaarallisilta tiedostoilta avaamalla ne vain luku-tilassa.</span><span class="sxs-lookup"><span data-stu-id="12143-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="12143-108">Sinun on ehkä tarkistettava virustentorjuntaohjelmasi kanssa, miten voit muuttaa näitä asetuksia.</span><span class="sxs-lookup"><span data-stu-id="12143-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="12143-109">BitDefender, esimerkiksi, on sisältöä lisäämällä sovelluksen poissulkemisia tässä: [Miten lisätä sovelluksen tai prosessin poissulkemisia BitDefender Control Center](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="12143-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="12143-110">**Onko tiedosto-ominaisuudet määritetty vain luku-tilassa?**</span><span class="sxs-lookup"><span data-stu-id="12143-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="12143-111">Voit tarkistaa tiedoston ominaisuudet napsauttamalla tiedostoa hiiren kakkos painikkeella ja valitsemalla Ominaisuudet.</span><span class="sxs-lookup"><span data-stu-id="12143-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="12143-112">Jos vain luku-määrite on valittuna, voit poistaa sen valinnan ja napsauttaa OK.</span><span class="sxs-lookup"><span data-stu-id="12143-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="12143-113">**Sisältö on suojattu näkymä**</span><span class="sxs-lookup"><span data-stu-id="12143-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="12143-114">Inter netistä ja muista mahdollisesti vaarallisista sijainneista olevat tiedostot voivat sisältää viruksia, matoja tai muunlaisia haitta ohjelmia, jotka voivat vahingoittaa tieto konetta.</span><span class="sxs-lookup"><span data-stu-id="12143-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="12143-115">Tämä on yleisesti myös Sähkö posti liitteiden tai lataamasi tiedostojen tapa uksessa.</span><span class="sxs-lookup"><span data-stu-id="12143-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="12143-116">Tieto koneen suojaamiseksi nämä mahdollisesti vaaralliset sijainnit avautuvat suojatussa näkymässä.</span><span class="sxs-lookup"><span data-stu-id="12143-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="12143-117">Suojatun näkymän avulla voit lukea tiedoston ja tarkastella sen sisältöä ja pienentää samalla riskejä.</span><span class="sxs-lookup"><span data-stu-id="12143-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="12143-118">Lisä tietoja Suojatusta näkymästä ja asetusten muuttamisesta on tässä artikkelissa: [mikä on suojattu näkymä?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="12143-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="12143-119">**Onko OneDrive täynnä?**</span><span class="sxs-lookup"><span data-stu-id="12143-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="12143-120">Jos tiedosto on tallennettu OneDriveen ja OneDrive-tallennus tilasi on täynnä, et voi tallentaa asia kirjaa, ennen kuin olet varattuun tilaan.</span><span class="sxs-lookup"><span data-stu-id="12143-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="12143-121">Voit tarkistaa vapaan tilasi OneDrivessa napsauttamalla OneDrive-kuvaketta ilmoitus keskuksessa ja valitsemalla Hallitse tallennus tilaa tai voit siirtyä [http://onedrive.live.com](http://onedrive.live.com), kirja utua sisään ja huomata käytetyn tilan määrän näytön vasemmassa alakulmassa.</span><span class="sxs-lookup"><span data-stu-id="12143-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [http://onedrive.live.com](http://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="12143-122">**Onko Office aktivoitu?**</span><span class="sxs-lookup"><span data-stu-id="12143-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="12143-123">Jos Officea ei ole aktivoitu tai jos tilauksesi on vanhentunut, voit käyttää vain luku-tilassa rajoitetun toiminnan tilaa.</span><span class="sxs-lookup"><span data-stu-id="12143-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="12143-124">Lisä tietoja Officen Akti voimisesta on kohdassa Office- [tuotteiden käyttö oikeuden ja aktivointi virheiden poistaminen](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="12143-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="12143-125">**Jos kaikki muu epäonnistuu...**</span><span class="sxs-lookup"><span data-stu-id="12143-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="12143-126">Yritä käynnistää tieto kone uudelleen</span><span class="sxs-lookup"><span data-stu-id="12143-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="12143-127">Office-päivitysten asentaminen</span><span class="sxs-lookup"><span data-stu-id="12143-127">Install Office updates</span></span>
    
- <span data-ttu-id="12143-128">Suorita Officen online-korjaus</span><span class="sxs-lookup"><span data-stu-id="12143-128">Perform an Online repair of Office</span></span>
    

