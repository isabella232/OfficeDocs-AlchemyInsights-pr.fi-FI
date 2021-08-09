---
title: 'AIP-skanneri: asennus ja määritys'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: 75fd61e18503292bd5fa9e48c7cdba7692282925a419b3230d17448eab928ba0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934254"
---
# <a name="aip-scanner-installation-and-configuration"></a>AIP-skanneri: asennus ja määritys

**Asenna AIP-skanneri noudattamalla suositeltuja ohjeita:**

1. Jos päivität ja et suorita puhdasta asennusta, varmista, että olet noudattanut [Ohjeita Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) -skannerin päivittämiseen ja yhdistetyn osoitetarrasovelluksen päivittämiseen, katso Azure Information Protection [-skannerin päivittäminen.](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)
2. Varmista, että noudatat kaikkia [palomuurien ja verkkoinfrastruktuurin asetusten vaatimuksia.](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)
3. Varmista, että [käytäntöihin on](https://docs.microsoft.com/azure/information-protection/configure-policy) määritetty automaattinen selite tai että käytäntö sisältää oletusotsikot.
4. Varmista, että asianmukainen tiedostotyyppi on määritetty selite-/suojausta varten artikkelissa Azure Information Protection -asiakasohjelman tukemat [tiedostotyypit kuvatulla tavalla.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection) Jos haluat muuttaa oletusasetuksia, noudata seuraavia ohjeita: [Tiedostojen oletussuojaustason muuttaminen.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)
5. Varmista, että skanneripalvelun suorittamiseen määritetyllä käyttäjätilillä on oikeus käyttää kaikkia määritettyjä säilöjä.
6. Jos ongelmia ilmenee edelleen, vie skannerilokit ja lisää ne tukipalveluun.

**Azure Information Protection Scanner -lokien vieminen**

1. Siirry kohtaan %localappdata%\Microsoft\MSIP skanneripalvelun suorittaman käyttäjäkontekstin mukaisesti.
2. Pakkaa kaikki MSIP-kansion sisältö.
3. Tallenna lokit haluamaasi sijaintiin ja liitä ne palvelupyyntöösi.
4. Voit käyttää myös [Export-AIPLogs -OnBehalfOf-sovellusta.](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps)

**Lisätietoja on kohdassa:**
- [Azure Information Protection -skannerin käyttöönotto tiedostojen automaattista luokittelemista ja suojaamista varten](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Set-AIPAuthentication-parametrin määritäminen ja käyttö](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Suorita etsintäjakso ja tarkastele skannerin raportteja](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Tutustu Azure Information Protection -ohjeisiin](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Azure Information Protectionin vaatimukset](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Lataa Azure Information Protection -asiakasohjelma](https://www.microsoft.com/download/details.aspx?id=53018)
