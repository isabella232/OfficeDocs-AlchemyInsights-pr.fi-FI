---
title: Intune Exchange yhdistin
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6732"
- "9003775"
ms.openlocfilehash: 744758739c2ca839823d2c8b440ed7b0d9dd4f06ebbb6f19fe52041a6710c4b4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013961"
---
# <a name="intune-exchange-on-premise-connector"></a>Intune Exchange yhdistin

Lisätietoja Intunen ja paikallisen Exchange välisen yhdistimen määrittämisestä on seuraavissa ohjeissa:

[Paikallisen Intunen Exchange yhdistimen Microsoft Intune Azuressa](https://docs.microsoft.com/intune/exchange-connector-install)

**Usein kysytyt kysymykset:**

K: Näyttöön tulee virhesanoma, kuten "Exchange Connector -versiota ei tueta", kun yritän määrittää Exchange yhdistimen. Mikä voi olla syy?

V: Käyttämälläsi tilillä on käyttöoikeus asianmukaisesti – sillä on oltava aktiivinen Intune-käyttöoikeus

K: Onko mahdollista käyttää useita Exchange yhdistimiä?

A: Voit määrittää vain yhden Exchange intune-vuokraajaa kohden organisaatiota Exchange kohden. Yhdistin voidaan asentaa vain yhteen palvelimeen usean palvelimen Exchange-organisaatiossa.

Et voi myöskään määrittää yhdistimiä sekä Exchange että Exchange Online määritettyäsi samaan vuokraajaan.

K: Voiko yhdistin käyttää CAS-matriisia yhteydenä Exchange?

V: CAS-matriisin määrittäminen ei ole tuettu määritys yhdistimen määrityksessä. Vain yksi palvelin tulisi määrittää ja sen pitäisi olla hardcoded yhdistimen määritystiedostossa, joka löytyy

program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml

Etsi seuraava merkintä ja ```<ExchangeWebServiceURL />``` korvaa URL-osoite Exchange-palvelimella.

**Esimerkki:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Katso lisätietoja vianmäärityksestä seuraavista ohjeista: [Paikallisen Intune-yhdistimen Exchange vianmääritys](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Yksityiskohtaisen kirjaamisen ottaminen käyttöön Exchange yhdistintä varten**

1. Avaa Exchange Yhdistimen jäljityksen määritystiedosto muokkausta varten.  
Tiedosto sijaitsee kohteessa : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Esimerkki:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Etsi TraceSourceLine seuraavalla avaimella: OnPremisesExchangeConnectorService  
  
3. Muuta Lähdetasoinen solmu -arvo Information ActivityTracing (oletus) -arvosta Yksityiskohtainen toiminta -arvoksi  

**Esimerkki:**
```
<TraceSourceLine>  
<Key xsi:type="xsd:string">OnPremisesExchangeConnectorService</Key>  
<Value xsi:type="TraceSource">  
<SourceLevel>All</SourceLevel>  
<Listeners>  
<Listener>  
<ListenerType>CircularTraceListener</ListenerType>
<SourceLevel>Verbose ActivityTracing</SourceLevel>
```
4. Käynnistä Microsoft Intune Exchange uudelleen  
5. Täydellinen synkronointi Intune-portaalissa, kunnes se on valmis, ja muuta sitten XML takaisin Tietotoiminta-määritykseksi ja käynnistä Microsoft Intune Exchange uudelleen.  
6. Lokien sijainti on: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`