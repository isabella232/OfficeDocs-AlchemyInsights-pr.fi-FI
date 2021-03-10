---
title: SAML-allekirjoitusvarmenteen ongelmien vianmääritys
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693420"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a><span data-ttu-id="6fd96-102">SAML-allekirjoitusvarmenteen ongelmien vianmääritys</span><span class="sxs-lookup"><span data-stu-id="6fd96-102">Troubleshoot SAML Signing certificate issues</span></span>

<span data-ttu-id="6fd96-103">Voit ratkaista SAML-allekirjoitusvarmenneongelman noudattamalla seuraavia suositeltuja ohjeita:</span><span class="sxs-lookup"><span data-stu-id="6fd96-103">To resolve SAML Signing certificate issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="6fd96-104">Kun lisäät yrityssovelluksen, joka tukee SSO:tä, Azure luo varmenteen, jonka nimi on [SAML-allekirjoitusvarmenne.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications)</span><span class="sxs-lookup"><span data-stu-id="6fd96-104">When you add an enterprise application which supports SSO, Azure will generate a certificate which is called the [SAML Signing certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span></span> <span data-ttu-id="6fd96-105">Tämän varmenteen vanhentumispäivä on kolme vuotta.</span><span class="sxs-lookup"><span data-stu-id="6fd96-105">This certificate has an expiration date of 3 years.</span></span> <span data-ttu-id="6fd96-106">Jos haluat muuttaa varmenteen vanhentumispäivää, katso lisätietoja liittoutumisvarmenteen vanhenemispäivän mukauttamisesta ja sen uudesta [varmenteesta.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate)</span><span class="sxs-lookup"><span data-stu-id="6fd96-106">To change the expiration date of your certificate, see [Customize the expiration date for your federation certificate and roll it over to a new certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span></span>
2. <span data-ttu-id="6fd96-107">Azure allekirjoittaa sovelluksen pyytämät SAML-tunnukset tämän varmenteen avulla ja lähettää sen sovellukseen onnistuneen SSO:n käyttöä varten.</span><span class="sxs-lookup"><span data-stu-id="6fd96-107">Azure will use this certificate to sign the SAML tokens requested by the application and send it over to the application for a successful SSO.</span></span> <span data-ttu-id="6fd96-108">Jotta tämä on valmis, lataa varmenne Azure-portaalista ja lähetä se sovelluksen toimittajalle SSO-prosessin viimeistelemiseksi.</span><span class="sxs-lookup"><span data-stu-id="6fd96-108">In order for this to complete, download the certificate from the Azure portal and send it to the application vendor to complete the SSO process.</span></span>

<span data-ttu-id="6fd96-109">Kun tämä prosessi on valmis, sovellus luottaa tähän varmenteeseen, ja sovellus hyväksyy kaikki tällä varmenteella allekirjoitetut SAML-tunnukset.</span><span class="sxs-lookup"><span data-stu-id="6fd96-109">After this process completes your application will trust this certificate and all the SAML tokens signed by this certificate will be accepted by the application.</span></span>

3. <span data-ttu-id="6fd96-110">Jos tämä varmenne vanhenee, luo uusi varmenne, päivitä se sovelluksen toimittajalle ja tee siitä aktiivinen Azure-puolella.</span><span class="sxs-lookup"><span data-stu-id="6fd96-110">If this certificate expires, create a new certificate, update it to the application vendor and then make it active on the Azure side.</span></span> <span data-ttu-id="6fd96-111">Lisätietoja on kohdassa Pian [vanhentuvan varmenteen uusiminen.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire)</span><span class="sxs-lookup"><span data-stu-id="6fd96-111">For more information, see [Renew a certificate that will soon expire](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span></span>

> [!NOTE]
> <span data-ttu-id="6fd96-112">Jos varmenne vanhenee, käyttäjää ei estetä.</span><span class="sxs-lookup"><span data-stu-id="6fd96-112">If the certificate expires, the user will not be blocked.</span></span>

4. <span data-ttu-id="6fd96-113">[Lisää sähköpostiosoite, jonka ilmoitukset](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) vastaanotetaan ennen nykyisen varmenteen vanhenemista.</span><span class="sxs-lookup"><span data-stu-id="6fd96-113">[Add an email address for notifications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) to be received before the current certificate expires.</span></span>

> [!NOTE]
> <span data-ttu-id="6fd96-114">Vaihe 4 on valinnainen vaihe.</span><span class="sxs-lookup"><span data-stu-id="6fd96-114">Step-4 is an optional one.</span></span>

5. <span data-ttu-id="6fd96-115">Muuta sovelluksen SAML-varmenteen allekirjoitusasetuksia ja varmenteen allekirjoitusalgoritmia.</span><span class="sxs-lookup"><span data-stu-id="6fd96-115">Change an application's SAML certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="6fd96-116">Lisätietoja on kohdassa Varmenteen [allekirjoitusasetusten ja allekirjoitusalgoritmin muuttaminen.](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)</span><span class="sxs-lookup"><span data-stu-id="6fd96-116">For more information, see [Change certificate signing options and signing algorithm](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>

