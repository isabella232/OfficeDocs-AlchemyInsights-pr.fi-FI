---
title: Luoda ja käyttää jaetun postilaatikon
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 1825cfd0a78a29734d0a5128e19acbfba9115d32
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/04/2019
ms.locfileid: "34717344"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Vianmääritys ongelma - käyttäjän kansiota ei löydy

<p>Jos käyttäjät saavat virhesanoman <strong> &ldquo; &hellip;käyttäjä voi&rsquo;t löydy hakemistosta. Yritä uudelleen&hellip; </strong> jossa on seurantakohteen tyyppi <strong> &ldquo;käyttäjä ei ole kansio.&rdquo;</strong>, voi suorittaa ongelman vianmäärityksen seuraavasti.</p> <ol> <li>Varmista tilin, email-kutsu on sama tili, jota käytetään Jos haluat kirjautua sisään myöhemmin. Varmista, että käyttäjä käyttää samaa tiliä, Kirjaudu sivustoon ja hyväksy kutsu. <br /><br />Saat lisätietoja- <a href="https://support.microsoft.com/en-us/help/12407/microsoft-account-how-to-manage-aliases">hallinnasta Microsoft-tilin aliaksia</a> hallinta Office 365-kirjautuminen. <br /><br /></li> <li>Selaa kunkin teillä, jossa käyttäjä vastaanottaa virheen. <br /><br />a. Lisää <strong> &ldquo;/_layouts/15/people.aspx/membershipgroupid=0&rdquo; </strong> (sisällä lainausmerkit) sivuston URL-Osoitteen loppuun. <br /><br />Esimerkki: https://&lt;contoso&gt;.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0 <br /><br />b. Valitse käyttäjä luettelosta. <br /><br />c. Valitse <strong>Poista käyttöoikeudet valintanauhasta</strong>. <br /><br />d. Lisää edellinen käyttäjä ja Lähetä kutsu käyttäjä.</li> </ol>

