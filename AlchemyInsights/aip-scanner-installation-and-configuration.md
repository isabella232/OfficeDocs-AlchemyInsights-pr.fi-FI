---
title: 'AIP-skanneri: asennus ja konfigurointi'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: d059d411aef03ca57662b71fbd7d27aecd3e0e57
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/23/2020
ms.locfileid: "44357663"
---
# <a name="aip-scanner-installation-and-configuration"></a>AIP-skanneri: asennus ja konfigurointi

**Asenna AIP-skanneri noudattamalla suositeltuja ohjeita:**

1. Jos päivität etkä suorita puhdasta asennusta, varmista, että olet noudattanut [Azure Information Protection -skannerin](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) ja yhtenäisen tarrausasiakkaan päivitysohjeita, katso [Azure Information Protection -skannerin päivittäminen](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).
2. Varmista, että noudatat kaikkia [palomuurien ja verkkoinfrastruktuurin asetuksia koskevia vaatimuksia.](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)
3. Varmista, että [käytännöt on määritetty](https://docs.microsoft.com/azure/information-protection/configure-policy) automaattiseksi otsikoksi tai että käytännössä on oletusotsikko.
4. Varmista, että asianmukainen tiedostotyyppi on määritetty tarraa/suojausta varten [azure-tietojen suojausasiakkaan tukemien tiedostotyyppien mukaisesti.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection) Jos haluat lisäksi muuttaa oletustoimintaa, noudata seuraavia ohjeita: [Tiedostojen oletussuojaustason muuttaminen](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. Varmista, että skanneripalvelun suorittamiseen määritetyllä käyttäjätilillä on oikeudet käyttää kaikkia määritettyjä tietovarastoja.
6. Jos ongelmat jatkuvat, vie skannerilokit ja lisää ne tukilippuusi.

**Azure Information Protection Scanner -lokien vieminen**

1. Siirry kansioon %localappdata%\Microsoft\MSIP skanneripalvelua suorittavassa käyttäjäkontekstissa.
2. Zip kaikki sisältö MSIP kansioon.
3. Tallenna lokit haluamaasi sijaintiin ja liitä ne palvelupyyntöösi.
4. Voit käyttää myös [Export-AIPLogs -OnBehalfOf -käyttöoikeutta.](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps)

**Lisätietoja on kohdassa**:
- [Azure Information Protection -skannerin käyttöönotto tiedostojen luokittelemiseksi ja suojaamiseksi automaattisesti](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Määritä Token-parametri set-AIPAuthentication-määritykselle ja käytä sitä](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Etsintäjakson suorittaminen ja skannerin raporttien tarkasteleminen](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Azure Information Protectionin dokumentaation tarkasteleminen](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Azure-tietojen suojausta koskevat vaatimukset](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Lataa Azure Information Protection -asiakasohjelma](https://www.microsoft.com/download/details.aspx?id=53018)
