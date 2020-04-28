---
title: Ehkäise Sovellusta ei tunnistettu -virhe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: e07c6b128a39f1fb1c998d051aafe72205d8cbee
ms.sourcegitcommit: 82155846ce771c18050e6113d6c199b34a1504ff
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/24/2020
ms.locfileid: "43810481"
---
# <a name="mitigate-the-application-was-not-detected-error"></a><span data-ttu-id="41f65-102">Ehkäise “Sovellusta ei tunnistettu” -virhe</span><span class="sxs-lookup"><span data-stu-id="41f65-102">Mitigate "The application was not detected" error</span></span>

<span data-ttu-id="41f65-103">Sovelluksen asennusvirhe: “Sovellusta ei tunnistettu, kun asennus on suoritettu onnistuneesti” Intunen raportoimana. Se saattaa näkyä kaikissa tärkeimmissä OS-ympäristöissä (Windows, iOS ja Android).</span><span class="sxs-lookup"><span data-stu-id="41f65-103">The app installation error, “The application was not detected after installation completed successfully,” reported by Intune, may occur on all major OS platforms (Windows, iOS and Android).</span></span>

<span data-ttu-id="41f65-104">Tämän virheen aiheuttavat yleisimmät skenaariot ovat seuraavat:</span><span class="sxs-lookup"><span data-stu-id="41f65-104">The most common scenarios that generate this error include:</span></span>

- <span data-ttu-id="41f65-105">Sovellus on päivitetty Intunen ulkopuolella (kolmannen osapuolen sovelluskaupasta) ensimmäisen käyttöönoton jälkeen.</span><span class="sxs-lookup"><span data-stu-id="41f65-105">The app has been updated outside of Intune (from a third-party app store) after the initial deployment.</span></span> <span data-ttu-id="41f65-106">Esimerkiksi jotkin sovellukset, kuten Google Chrome, voivat tehdä automaattisia päivityksiä.</span><span class="sxs-lookup"><span data-stu-id="41f65-106">For example some applications such as Google Chrome may perform auto updates.</span></span>
- <span data-ttu-id="41f65-107">Käyttäjä on poistanut sovelluksen asennuksen ensimmäisen asennuksen jälkeen.</span><span class="sxs-lookup"><span data-stu-id="41f65-107">A user has uninstalled the app after the initial install.</span></span>

<span data-ttu-id="41f65-108">Jos haluat estää ongelman, tee ensin arvio siitä, mitä laitteita on tarkasteltava, jotta voit määrittää, missä skenaariossa virhe ilmenee.</span><span class="sxs-lookup"><span data-stu-id="41f65-108">To mitigate this issue, first perform a review of the affected devices to determine the scenario in which the error occurs.</span></span>

- <span data-ttu-id="41f65-109">Jos sovellus on päivitetty Intunen ulkopuolella, sovelluksen käyttöönoton voi määrittää ohittamaan sovellusversion.</span><span class="sxs-lookup"><span data-stu-id="41f65-109">If the app has been updated outside of Intune, the app deployment can be set to ignore the application version.</span></span> <span data-ttu-id="41f65-110">Se tapahtuu määrittämällä kohdassa **Sovelluksen määritys > Sovelluksen tiedot** **Hylkää sovellus** valinta **Kyllä**.</span><span class="sxs-lookup"><span data-stu-id="41f65-110">To do so, under **App Configuration > App Information**, set **Ignore App** version to **Yes**.</span></span>
- <span data-ttu-id="41f65-111">Asiakasta kohdennettaessa saattaa olla tarpeen ottaa sovellus käyttöön pakolliseksi ja varmistaa, että uusin versio on otettu käyttöön.</span><span class="sxs-lookup"><span data-stu-id="41f65-111">When targeting the client, it may be appropriate to deploy the application as “required,” and to ensure that the latest version is deployed.</span></span>
- <span data-ttu-id="41f65-112">Vaihtoehtoisesti voit käyttää iOS-ympäristössä **Automaattinen päivitys** -toimintoa, joka on liitetty Applen volyymiosto-ohjelmaan, joka voidaan määrittää päivittämään automaattisesti uusiin sovellusversioihin, kun ne ovat saatavilla.</span><span class="sxs-lookup"><span data-stu-id="41f65-112">Alternatively, on the iOS platform, it is possible to use the **autoupdate** functionality associated with the Apple Volume Purchase Program, which can be configured to automatically update to new application versions as they become available.</span></span>

<span data-ttu-id="41f65-113">Jos haluat lisätietoja sovellusten asennusongelmien vianmäärityksestä, lue [Sovellusten asennusongelmien vianmääritys](https://docs.microsoft.com/intune/troubleshoot-app-install).</span><span class="sxs-lookup"><span data-stu-id="41f65-113">For more information about troubleshooting app installation issues, please see [Troubleshoot app installation issues](https://docs.microsoft.com/intune/troubleshoot-app-install).</span></span>
