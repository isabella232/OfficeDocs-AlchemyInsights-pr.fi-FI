---
title: Applen MDM Push -varmennetta ei ole määritetty
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439384"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a><span data-ttu-id="86c05-102">Applen MDM Push -varmennetta ei ole määritetty</span><span class="sxs-lookup"><span data-stu-id="86c05-102">Apple MDM Push Certificate has not been set up</span></span>

<span data-ttu-id="86c05-103">Applen MDM Push Certificate -varmennetta (tunnetaan myös nimellä Applen push-ilmoituspalvelu (APNS) -varmennetta) ei ole määritetty tilaukseesi.</span><span class="sxs-lookup"><span data-stu-id="86c05-103">An Apple MDM Push Certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured for your subscription.</span></span> <span data-ttu-id="86c05-104">Ilman Applen MDM Push Certificate -sertifikaattia et voi rekisteröidä ja hallita iOS- ja Mac OS -laitteita.</span><span class="sxs-lookup"><span data-stu-id="86c05-104">Without an Apple MDM Push Certificate configured, you are unable to enroll and manage iOS and Mac OS devices.</span></span> <span data-ttu-id="86c05-105">Kun olet lisännyt varmenteen Intuneen, käyttäjät voivat rekisteröidä iOS-laitteensa asentamalla Yritysportaali-sovelluksen.</span><span class="sxs-lookup"><span data-stu-id="86c05-105">After you add the certificate to Intune, users can install the Company Portal app to enroll their iOS devices.</span></span>

1. <span data-ttu-id="86c05-106">Valitse **"Olen samaa mieltä".**</span><span class="sxs-lookup"><span data-stu-id="86c05-106">Select **"I agree."**</span></span> <span data-ttu-id="86c05-107">antaa Microsoftille lupa lähettää tietoja Applelle.</span><span class="sxs-lookup"><span data-stu-id="86c05-107">to give Microsoft permission to send data to Apple.</span></span>

2. <span data-ttu-id="86c05-108">Valitse **Lataa csr** Intune-varmenteen allekirjoituspyyntö, joka tarvitaan Applen MDM-push-varmenteen luomiseen.</span><span class="sxs-lookup"><span data-stu-id="86c05-108">Select **Download your CSR** the Intune certificate signing request required to create an Apple MDM push certificate.</span></span> <span data-ttu-id="86c05-109">Tiedoston avulla pyydetään luottamussuhdevarmennetta Applen push-varmenteiden portaalista.</span><span class="sxs-lookup"><span data-stu-id="86c05-109">The file is used to request a trust relationship certificate from the Apple Push Certificates Portal.</span></span>

3. <span data-ttu-id="86c05-110">Siirry Applen push-varmenteiden portaaliin valitsemalla **Luo MDM-push-varmenne.**</span><span class="sxs-lookup"><span data-stu-id="86c05-110">Select **Create your MDM push Certificate** to go to the Apple Push Certificates Portal.</span></span> <span data-ttu-id="86c05-111">Kirjaudu sisään yrityksen Apple ID:llä ja valitse luo **varmenne**.</span><span class="sxs-lookup"><span data-stu-id="86c05-111">Sign in with your company Apple ID, and then select **Create a Certificate**.</span></span> <span data-ttu-id="86c05-112">Valitse **Valitse tiedosto**, siirry varmenteen allekirjoituspyyntötiedoston kohtaan ja valitse sitten **Lataa**.</span><span class="sxs-lookup"><span data-stu-id="86c05-112">Select **Choose File**, browse to the certificate signing request file, and then choose **Upload**.</span></span> <span data-ttu-id="86c05-113">Lataa varmennetiedosto (.pem) valitsemalla Vahvistus-sivulla **Lataa** ja tallenna tiedosto paikallisesti.</span><span class="sxs-lookup"><span data-stu-id="86c05-113">On the Confirmation page, choose **Download** to download the certificate (.pem) file, and save the file locally.</span></span>
 
<span data-ttu-id="86c05-114">**Huomautus:** Varmenne liittyy sen luomiseen käytettyyn Apple ID:hen.</span><span class="sxs-lookup"><span data-stu-id="86c05-114">**Note**: The certificate is associated with the Apple ID used to create it.</span></span> <span data-ttu-id="86c05-115">Käytä parhaana käytäntönä yrityksen Apple ID:tä hallintatehtäviin ja varmista, että postilaatikkoa valvoo useampi kuin yksi henkilö tai jakeluluetteloa.</span><span class="sxs-lookup"><span data-stu-id="86c05-115">As a best practice, use a company Apple ID for management tasks, and make sure the mailbox is monitored by more than one person or by using a distribution list.</span></span> <span data-ttu-id="86c05-116">Älä koskaan käytä henkilökohtaista Apple ID:tä.</span><span class="sxs-lookup"><span data-stu-id="86c05-116">Never use a personal Apple ID.</span></span> <span data-ttu-id="86c05-117">Käytä samaa Apple ID:tä Apple Push -varmenteen uusimiseen 12 kuukauden välein.</span><span class="sxs-lookup"><span data-stu-id="86c05-117">Use the same Apple ID to renew the Apple Push Certificate every 12 months.</span></span>
 
4. <span data-ttu-id="86c05-118">Anna Apple ID, jota käytetään Applen MDM-push-varmenteen luomiseen.</span><span class="sxs-lookup"><span data-stu-id="86c05-118">Enter the Apple ID used to create your Apple MDM push certificate.</span></span> <span data-ttu-id="86c05-119">Tallenna tämä tunnus muistutuksena, kun varmenne on uusittava.</span><span class="sxs-lookup"><span data-stu-id="86c05-119">Record this ID as a reminder for when you need to renew the certificate.</span></span>

5. <span data-ttu-id="86c05-120">Siirry varmennetiedostoon (.pem), valitse **Avaa**ja valitse sitten **Lataa**.</span><span class="sxs-lookup"><span data-stu-id="86c05-120">Go to the certificate (.pem) file, choose **Open**, and then choose **Upload**.</span></span> <span data-ttu-id="86c05-121">Push-varmenteella Intune voi rekisteröidä ja hallita Apple-laitteita.</span><span class="sxs-lookup"><span data-stu-id="86c05-121">With the push certificate, Intune can enroll and manage Apple devices.</span></span>