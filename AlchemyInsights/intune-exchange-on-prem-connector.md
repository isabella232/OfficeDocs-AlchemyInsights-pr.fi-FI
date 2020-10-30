---
title: Intune Exchangen paikallinen yhdistin
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
ms.openlocfilehash: 8b470655efa2dfb460c29b6b840fa793ed2aa448
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807650"
---
# <a name="intune-exchange-on-premise-connector"></a><span data-ttu-id="c29a1-102">Intune Exchangen paikallinen yhdistin</span><span class="sxs-lookup"><span data-stu-id="c29a1-102">Intune Exchange on-premise Connector</span></span>

<span data-ttu-id="c29a1-103">Jos haluat lisä tietoja yhdistimen määrittämisestä Intune-toiminnon ja paikallisen Exchange-sovelluksen välillä, tutustu seuraaviin ohje isiin:</span><span class="sxs-lookup"><span data-stu-id="c29a1-103">For details of setting up the connector between Intune and Exchange which is hosted on-premises please see the following documentation:</span></span>

[<span data-ttu-id="c29a1-104">Paikallisen Exchange-yhdistimen määrittäminen Intunella Microsoft Intune Azure-sovelluksessa</span><span class="sxs-lookup"><span data-stu-id="c29a1-104">Set up the Intune on-premises Exchange connector in Microsoft Intune Azure</span></span>](https://docs.microsoft.com/intune/exchange-connector-install)

<span data-ttu-id="c29a1-105">**USEIN kysytyt kysymykset**</span><span class="sxs-lookup"><span data-stu-id="c29a1-105">**FAQ:**</span></span>

<span data-ttu-id="c29a1-106">K: näyttöön tulee virhe, kuten "Exchange Connector-versiota ei voi käyttää", kun yrität määrittää Exchange Connectoria.</span><span class="sxs-lookup"><span data-stu-id="c29a1-106">Q: I see an error such as "The Exchange Connector version is not supported" when attempting to set up the Exchange connector.</span></span> <span data-ttu-id="c29a1-107">Mikä voi olla syynä?</span><span class="sxs-lookup"><span data-stu-id="c29a1-107">What could be the cause?</span></span>

<span data-ttu-id="c29a1-108">A: käyttämäsi tilin käyttö oikeus on oikein-sillä on oltava aktiivinen Intune-käyttö oikeus</span><span class="sxs-lookup"><span data-stu-id="c29a1-108">A: The account you are using is licensed appropriately - it must have an active Intune license</span></span>

<span data-ttu-id="c29a1-109">K: Onko mahdollista käyttää useita Exchange-yhdistimiä?</span><span class="sxs-lookup"><span data-stu-id="c29a1-109">Q: Is it possible to have multiple Exchange connectors?</span></span>

<span data-ttu-id="c29a1-110">A: voit määrittää vain yhden Exchange Connector/Intune-vuokra ajan Exchange-organisaatiota kohden.</span><span class="sxs-lookup"><span data-stu-id="c29a1-110">A: You can only set up one Exchange connector per Intune tenant per Exchange organization.</span></span> <span data-ttu-id="c29a1-111">Yhdistin voidaan asentaa vain yhteen palvelimeen usean palvelimen Exchange-organisaatiossa.</span><span class="sxs-lookup"><span data-stu-id="c29a1-111">The connector can only be installed on one server in a multi server exchange organization.</span></span>

<span data-ttu-id="c29a1-112">Et voi myöskään määrittää samassa vuokra ajassa määritettyä sekä Exchange Onlinea että Exchange Onlinen yhdistimiä.</span><span class="sxs-lookup"><span data-stu-id="c29a1-112">Also you cannot have connectors configured for both Exchange on-premise and Exchange Online configured in the same tenant.</span></span>

<span data-ttu-id="c29a1-113">K: Voiko yhdistin käyttää CAS-matriisia Exchangen yhteydessä?</span><span class="sxs-lookup"><span data-stu-id="c29a1-113">Q: Can the connector use a CAS array as its connection to Exchange?</span></span>

<span data-ttu-id="c29a1-114">A: CAS-matriisin määrittäminen ei ole yhteensopiva kokoonpano yhdistimen määrityksessä.</span><span class="sxs-lookup"><span data-stu-id="c29a1-114">A: Specifying a CAS array is not a supported configuration in the connector setup.</span></span> <span data-ttu-id="c29a1-115">Vain yksittäinen palvelin pitäisi määrittää, ja sen pitäisi olla kovakoodattu yhdistimen määritys tiedostossa, joka löytyy</span><span class="sxs-lookup"><span data-stu-id="c29a1-115">Only a single server should be specified and should be hardcoded in the connector configuration file which can be found in</span></span>

<span data-ttu-id="c29a1-116">ohjelmadata\microsoft\microsoft Intunen paikallinen Exchange Connector \ OnpremiseExchangeConnectorServiceConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="c29a1-116">program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml</span></span>

<span data-ttu-id="c29a1-117">Etsi seuraava merkintä ```<ExchangeWebServiceURL />``` ja Vaihda URL-osoite Exchange-palvelimeen.</span><span class="sxs-lookup"><span data-stu-id="c29a1-117">Locate the following entry ```<ExchangeWebServiceURL />``` and replace the URL with the exchange server.</span></span>

<span data-ttu-id="c29a1-118">**Esimerkiksi**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span><span class="sxs-lookup"><span data-stu-id="c29a1-118">**Example:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span></span>

<span data-ttu-id="c29a1-119">Lisä tietoja vian määrityksestä on seuraavissa ohjeissa: [Intune-paikallisen Exchange Connectorin vian määritys](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span><span class="sxs-lookup"><span data-stu-id="c29a1-119">Please see the following documentation for additional troubleshooting: [Troubleshoot the Intune on-premises Exchange connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span></span>

<span data-ttu-id="c29a1-120">**Selväkielisen kirjaamisen ottaminen käyttöön Exchange Connectorissa**</span><span class="sxs-lookup"><span data-stu-id="c29a1-120">**Enabling Verbose logging for the Exchange connector**</span></span>

1. <span data-ttu-id="c29a1-121">Avaa Exchange Connector-jäljityksen määritys tiedosto muokkaamista varten.</span><span class="sxs-lookup"><span data-stu-id="c29a1-121">Open the Exchange Connector tracing configuration file for editing.</span></span>  
<span data-ttu-id="c29a1-122">Tiedosto sijaitsee osoitteessa:%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="c29a1-122">The file is located at : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span></span>  

<span data-ttu-id="c29a1-123">**Esimerkiksi**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span><span class="sxs-lookup"><span data-stu-id="c29a1-123">**Example:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span></span>
  
2. <span data-ttu-id="c29a1-124">Etsi TraceSourceLine seuraavalla avaimella: opremisesexchangecontactorservice</span><span class="sxs-lookup"><span data-stu-id="c29a1-124">Locate the TraceSourceLine with the following key: OnPremisesExchangeConnectorService</span></span>  
  
3. <span data-ttu-id="c29a1-125">SourceLevel-solmun arvon muuttaminen tietojen activerttracing (oletus)-kentän arvoksi verbose-pikatoimintojen jäljitys</span><span class="sxs-lookup"><span data-stu-id="c29a1-125">Change the SourceLevel node value from Information ActivityTracing (the default) to Verbose ActivityTracing</span></span>  

<span data-ttu-id="c29a1-126">**Esimerkiksi**</span><span class="sxs-lookup"><span data-stu-id="c29a1-126">**Example:**</span></span>
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
4. <span data-ttu-id="c29a1-127">Microsoft Intune Exchange-palvelun käynnistäminen uudelleen</span><span class="sxs-lookup"><span data-stu-id="c29a1-127">Restart the Microsoft Intune Exchange Service</span></span>  
5. <span data-ttu-id="c29a1-128">Täysi synkronointi Intune-portaalissa, kunnes se on valmis, ja muuta sitten XML takaisin "Information Activitystracing" ja Käynnistä Microsoft Intune Exchange-palvelu uudelleen.</span><span class="sxs-lookup"><span data-stu-id="c29a1-128">Full sync in Intune Portal until it finishes and then change the XML back to "Information ActivityTracing" and restart the Microsoft Intune Exchange Service.</span></span>  
6. <span data-ttu-id="c29a1-129">Lokien sijainti on: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span><span class="sxs-lookup"><span data-stu-id="c29a1-129">Location of the logs is : `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span></span>