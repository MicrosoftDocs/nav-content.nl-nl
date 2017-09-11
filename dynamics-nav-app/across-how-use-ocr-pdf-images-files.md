---
title: 'Procedure: OCR gebruiken om PDF- en afbeeldingsbestanden te converteren naar elektronische documenten'
author: SorenGP
ms.custom: na
ms.date: 10/06/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 96b1baf3554d3647e75223bb4cb1ee08dc21eb6d
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-use-ocr-to-turn-pdf-and-image-files-into-electronic-documents"></a>Procedure: OCR gebruiken om PDF- en afbeeldingsbestanden te converteren naar elektronische documenten
Vanuit PDF- of afbeeldingsbestanden die u ontvangt van uw handelspartners, kunt u elektronische documenten laten genereren door een externe OCR-service (Optical Character Recognition - optische tekenherkenning), die kunnen worden geconverteerd naar documentrecords in Dynamics NAV. Bijvoorbeeld, wanneer u facturen in PDF-indeling van uw leverancier ontvangt, kunt u deze naar de OCR-service verzenden vanuit het venster **Inkomende documenten**. Dit wordt in de eerste procedure beschreven.

Als alternatief voor het verzenden van het bestand vanuit het venster **Inkomende documenten**, kunt u het bestand naar de OCR-service sturen via e-mail. Wanneer u het elektronische document terug ontvangt, wordt automatisch een gerelateerde inkomende documentrecord gemaakt. Dit wordt in de tweede procedure beschreven.

Na enkele seconden krijgt u het bestand weer terug van de OCR-service als een elektronische factuur die kan worden geconverteerd naar een inkoopfactuur voor de leverancier. Dit wordt in de derde procedure beschreven.

Omdat OCR is gebaseerd op optische herkenning, is het waarschijnlijk dat de OCR-service tekens in uw PDF- of afbeeldingsbestanden verkeerd interpreteert wanneer bijvoorbeeld de documenten van een bepaalde leverancier voor het eerst worden verwerkt. De service interpreteert het bedrijfslogo mogelijk niet als de naam van de leverancier of interpreteert het totaalbedrag op een ontvangstbewijs verkeerd vanwege de lay-out ervan. Als u deze fouten voortaan wilt voorkomen, kunt u ze corrigeren in een aparte versie van het venster **Inkomende documenten**. Vervolgens stuurt u de correcties terug naar de OCR-service om deze te trainen in het interpreteren van de specifieke tekens wanneer de volgende keer een PDF- of afbeeldingsbestand voor dezelfde leverancier wordt ontvangen. Zie voor meer informatie het gedeelte "De OCR-service trainen om fouten te voorkomen".

Het verkeer van bestanden van en naar de OCR-service wordt verwerkt door een specifiek taakwachtrij-item, dat automatisch wordt gemaakt als u de gerelateerde serviceverbinding inschakelt. Zie [Procedure: Inkomende documenten instellen](across-how-setup-income-documents.md) voor meer informatie.

## <a name="to-send-a-pdf-or-image-file-to-the-ocr-service-from-the-incoming-documents-window"></a>Een PDF-of afbeeldingsbestand verzenden naar de OCR-service vanuit het venster **Inkomende documenten**
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Inkomende documenten** in en kies vervolgens de gerelateerde koppeling.
2. Maak een nieuwe inkomende documentrecord en koppel het bestand eraan. Zie [Procedure: Inkomende documentrecords maken](across-how-create-income-document-records.md) voor meer informatie.  
3. Selecteer in het venster **Inkomende documenten** een of meer regels en kies vervolgens de actie **Verzenden naar taakwachtrij**.

    De waarde in het veld **OCR-status** verandert in **Gereed**. Het bijgevoegde PDF- of afbeeldingsbestand wordt naar de OCR-service verzonden door de taakwachtrij, volgens de planning, op voorwaarde dat er geen fouten zijn.
5. Of selecteer in het venster **Inkomende documenten** een of meer regels en kies vervolgens de actie **Verzenden naar OCR-service**.

De waarde in het veld **OCR-status** verandert in Verzonden als er geen fouten zijn.

## <a name="to-send-a-pdf-or-image-file-to-the-ocr-service-by-email"></a>Een PDF- of afbeeldingsbestand naar de OCR-service verzenden per e-mail
Vanuit uw e-mailtoepassing kunt u een e-mailbericht verzenden naar de aanbieder van de OCR-service met het PDF- of afbeeldingsbestand als bijlage. Zie de website van de provider van de OCR-service voor meer informatie over het e-mailadres waarnaar het bericht moet worden verzonden.

Omdat er geen inkomende documentrecord bestaat voor het bestand, wordt automatisch een nieuwe record gemaakt in het venster **Inkomende documenten** wanneer u het resulterende elektronische document ontvangt van de OCR-service. Zie [Procedure: Inkomende documentrecords maken](across-how-create-income-document-records.md) voor meer informatie.

**Opmerking**: als u op een tablet of telefoon werkt, kunt u het bestand naar de OCR-service verzenden zodra u een foto van het document hebt gemaakt, of u kunt rechtstreeks een inkomend document maken. Zie voor meer informatie het gedeelte "Inkomende documentrecords maken door een foto te maken" in [Procedure: Inkomende documentrecords maken](across-how-create-income-document-records.md).

## <a name="to-receive-the-resulting-electronic-document-from-the-ocr-service"></a>Het resulterende elektronische document ontvangen van de OCR-service
Het elektronische document dat door de OCR-service van het PDF- of het afbeeldingsbestand wordt gemaakt, wordt automatisch ontvangen in het **venster Inkomende documenten** door de verwerkingswachtrijpost die wordt ingesteld wanneer u de OCR-service inschakelt.

Als u geen verwerkingswachtrij gebruikt of een voltooid OCR-document eerder wilt ontvangen dan volgens het verwerkingswachtrijschema wordt verwacht, kunt u de knop**Ontvangen van OCR-service**kiezen. Hiermee worden alle documenten opgehaald die door de OCR-service zijn voltooid.

**Opmerking**: als de OCR-service zo is ingesteld dat handmatige verificatie van verwerkte documenten is vereist, bevat het veld **OCR-status** de waarde **In afwachting van verificatie**. In dat geval voert u de volgende stappen uit om u aan te melden bij de website van de OCR-service om een OCR-document handmatig te verifiëren.

1. Kies in het veld**OCR-status**de hyperlink **In afwachting van verificatie**. Kies de tegel **In afwachting van verificatie**op de startpagina.
2. Meld u bij de website van de OCR-service aan met de aanmeldgegevens van uw OCR-serviceaccount. Dit zijn de aanmeldgegevens die ook bij het instellen van de service worden gebruikt. Zie het gedeelte "Een OCR-service instellen"in [Procedure: Inkomende documenten instellen](across-how-setup-income-documents.md)voor meer informatie.

    Als u de website via het veld **OCR-status**opent, wordt het desbetreffende document direct na aanmelding weergegeven. Als u de website opent door de tegel op de startpagina te kiezen, moet u op de eerste OCR-servicepagina die wordt geopend, de knop **Start**op het tabblad **Verifiëren**kiezen of dubbelklikken op het document dat u wilt verifiëren.

    De gegevens voor het OCR-document worden weergegeven met zowel de broninhoud van het PDF- of afbeeldingsbestand als de resulterende OCR-veldwaarden.
3. Controleer handmatig de verschillende veldwaarden en bewerk of typ handmatig waarden in de velden die de OCR-service heeft gemarkeerd als onbepaald.
4. Kies de knop **Ok**. Het OCR-proces is voltooid en het resulterende elektronische document wordt verzonden naar het venster **Inkomende documenten** in Dynamics NAV in overeenstemming met het verwerkingswachtrijschema.

    Als u de website opent door de tegel op de startpaginate kiezen, wordt elk ander OCR-document dat moet worden geverifieerd, automatisch op de website weergegeven.
5. Herhaal stap 4 voor elk ander OCR-document dat moet worden geverifieerd.

U kunt nu doorgaan met het, handmatig of automatisch, maken van documentrecords voor de ontvangen elektronische documenten in Dynamics NAV. Zie het gedeelte "Een documentrecord in Dynamics NAV maken op basis van een ontvangen OCR-document"voor meer informatie. U kunt ook de nieuwe inkomende documentrecord aan een bestaand geboekt of niet-geboekt document koppelen zodat het bronbestand gemakkelijk toegankelijk is vanuit Dynamics NAV. Zie [Procedure: Inkomende documenten verwerken](across-process-income-documents.md) voor meer informatie.

## <a name="to-create-a-purchase-invoice-from-an-electronic-document-received-from-the-ocr-service"></a>Een inkoopfactuur op basis van een elektronisch document ontvangen van de OCR-service maken
Met de volgende procedure wordt beschreven hoe u een inkoopfactuurrecord maakt op basis van een leveranciersfactuur die is ontvangen als een elektronisch document van de OCR-service. De procedure is hetzelfde wanneer u bijvoorbeeld een dagboekregel van een kostenontvangst maakt.

**Opmerking**: de velden**Omschrijving** en**Nr.** op de gemaakte documentregels worden alleen ingevuld als u eerst tekst die is gevonden in het OCR-document, hebt toegewezen aan de twee velden in Dynamics NAV. U kunt dit doen als artikelkruisverwijzingen, documentregels van het soort Artikel of als tekst-aan-rekening toewijzingen voor document- of dagboekregels van het soort Grootboekrekening. Zie voor meer informatie de knopinfo voor de actie **Kruisverwijzingen**op artikelkaarten en de gerelateerde procedure [Procedure: Tekst in terugkerende betalingen toewijzen aan accounts voor automatisch reconciliëren](receivables-how-map-text-recurring-payments-accounts-auto-reconcilliation.md).

Voor inkomende documenten gebruikt u meestal de actie **Tekst toewijzen aan rekening**om te definiëren daten bepaalde tekst op een leveranciersfactuurontvangen van OCR-service, is toegewezen aan een bepaalde leveranciersrekening. In elk onderdeel van de omschrijving van het binnenkomende document dat als een toewijzingstekst aanwezig is, wordt in het veld**Nr.** in het resulterende document of de resulterende dagboekregels van het soort grootboekrekening ingevuld met de desbetreffende leverancier.

U kunt niet alleen aan een leveranciersrekening of aan grootboekrekeningen toewijzen, maar ook aan een bankrekening. Dit is bijvoorbeeld handig voor elektronische documenten voor kosten die al zijn betaald en waarvoor u een dagboekregel wilt maken die kan worden geboekt naar een bankrekening.

1. Selecteer de regel van het inkomende document voor het elektronische leveranciersdocument dat is ontvangen van de OCR-service.
2. Als u tekst in het document aan de rekening van de leverancier wilt toewijzen, een debetrekening, kiest u de actie **Tekst aan rekening toewijzen**en vult u vervolgens het venster **Toewijzing tekst aan rekening**met gegevens die voortaan op de leverancier worden toegepast. Zie [Procedure: Tekst op herhalende betalingen aan rekeningen toewijzen voor automatisch reconciliëren](receivables-how-map-text-recurring-payments-accounts-auto-reconcilliation.md) voor meer informatie.
3. Als u de artikelnummers in het document aan uw omschrijvingen van de leveranciersartikelen wilt toewijzen, opent u de kaart en kiest u vervolgens de actie **Kruisverwijzingen** om kruisverwijzingen tussen uw artikelomschrijvingen en die van de leverancier in te stellen.
4. Kies in het venster **Inkomende documenten** de actie **Document maken**.

In Dynamics NAV wordt een inkoopfactuur gemaakt op basis van de gegevens in het elektronische leveranciersdocument dat u van de OCR-service hebt ontvangen.

Eventuele validatiefouten, die meestal worden veroorzaakt door onjuiste of ontbrekende mastergegevens in Dynamics NAV, worden weergegeven op het sneltabblad**Fouten en waarschuwingen**. Zie het gedeelte "Fouten afhandelen bij de ontvangst van elektronische documenten"voor meer informatie.

## <a name="to-handle-errors-when-receiving-electronic-documents"></a>Fouten afhandelen bij de ontvangst van elektronische documenten
1. Selecteer in het venster **Inkomende documenten** de regel voor een elektronisch document dat met fouten is ontvangen van de OCR-service. Dit wordt aangegeven door de waarde Fout in het veld **OCR-status**.
2. Kies de actie **Bewerken**om het venster**Inkomende documenten** te openen.
3. Selecteer op het sneltabblad **Fouten en waarschuwingen** het bericht en kies vervolgens de actie **Gerelateerde record openen**.
4. Het venster dat de verkeerde of ontbrekende gegevens bevat, zoals een leverancierskaart waarop een veldwaarde ontbreekt, wordt geopend.
5. Corrigeer de fout of fouten zoals in elke foutmelding wordt beschreven.
6. Ga door met de verwerking van het inkomende elektronische document door nogmaals de actie **Handmatig maken** te kiezen.
7. Herhaal stap 5 en 6 voor eventuele andere fouten tot het elektronische document probleemloos kan worden ontvangen.

## <a name="to-train-the-ocr-service-to-avoid-errors"></a>De OCR-service trainen om fouten te voorkomen
Omdat OCR is gebaseerd op optische herkenning, is het waarschijnlijk dat de OCR-service tekens in uw PDF- of afbeeldingsbestanden verkeerd interpreteert wanneer bijvoorbeeld de documenten van een bepaalde leverancier voor het eerst worden verwerkt. De service interpreteert het bedrijfslogo mogelijk niet als de naam van de leverancier of interpreteert het totaalbedrag op een onkostenbewijs verkeerd vanwege de lay-out ervan. Als u dergelijke fouten voortaan wilt voorkomen, kunt u gegevens die van de OCR-service worden ontvangen, corrigeren en de feedback vervolgens terugsturen naar de service.

Het venster **Correctie OCR-gegevens**, dat u opent vanuit het venster **Inkomend document**, bevat de velden van het sneltabblad **Financiële informatie** in twee kolommen. Een kolom met de bewerkbare OCR-gegevens en een kolom met de alleen-lezen OCR-gegevens. Wanneer u de knop **OCR-feedback verzenden** kiest, wordt de inhoud van het venster **Correctie OCR-gegevens** naar de OCR-service verzonden. De volgende keer dat de service PDF- of afbeeldingsbestanden verwerkt die de betreffende gegevens bevatten, worden uw correcties meegenomen om dezelfde fouten te voorkomen.

1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Inkomende documenten** in en kies vervolgens de gerelateerde koppeling.
2. Open een inkomende documentrecord die gegevens bevat die van de OCR-service zijn ontvangen en die u wilt corrigeren.
3. Kies in het venster **Inkomend document** de actie **Correctie OCR-gegevens**.
4. Overschrijf in het venster **Correctie OCR-gegevens** de gegevens in de bewerkbare kolom voor elk veld dat een onjuiste waarde heeft.
5. Als u correcties ongedaan wilt maken die u hebt aangebracht sinds u het venster **Correctie OCR-gegevens** hebt geopend, kiest u de actie **OCR-gegevens opnieuw instellen**.
6. Als u de correcties naar de OCR-service wilt sturen, kiest u de actie **OCR-feedback verzenden**.
7. Als u de correcties wilt opslaan, sluit u het venster **Correctie OCR-gegevens**.

De velden op het sneltabblad **Financiële informatie** in het venster **Inkomende documenten** worden bijgewerkt met nieuwe waarden die u in stap 4 hebt ingevoerd.

## <a name="see-also"></a>Zie ook  
[Inkomende documenten verwerken](across-process-income-documents.md)  
[Inkomende documenten](across-income-documents.md)  
[Inkoop beheren](purchasing-manage-purchasing.md)  
[Werken met Dynamics NAV](ui-work-product.md)

