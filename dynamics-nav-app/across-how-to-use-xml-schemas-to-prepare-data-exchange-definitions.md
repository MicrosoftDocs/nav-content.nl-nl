---
title: XMLports maken op basis van XML-schema's
description: Gebruik XML-schema's om het kader voor gegevensuitwisseling in te stellen.
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 607d51d929e019662fdc4e17f7bbb064f806f32a
ms.contentlocale: nl-nl
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-use-xml-schemas-to-prepare-data-exchange-definitions"></a><span data-ttu-id="93bbf-103">Procedure: XML-schema's gebruiken om gegevensuitwisselingsdefinities voor te bereiden</span><span class="sxs-lookup"><span data-stu-id="93bbf-103">How to: Use XML Schemas to Prepare Data Exchange Definitions</span></span>
<span data-ttu-id="93bbf-104">Om het importeren/exporteren van gegevens in XML-bestanden via het kader voor gegevensuitwisseling in [!INCLUDE[d365fin](includes/d365fin_md.md)] mogelijk te maken, kunt u XML-schema's gebruiken om te bepalen welke gegevenselementen u wilt uitwisselen met [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="93bbf-104">To enable import/export of data in XML files through the data exchange framework in [!INCLUDE[d365fin](includes/d365fin_md.md)], you can use XML schemas to define which data elements you want to exchange with [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="93bbf-105">Hiervoor opent u het venster **XML-schemaviewer** en laadt u het XML-schemabestand, selecteert u de relevante gegevenselementen en initialiseert u vervolgens een definitie voor gegevensuitwisseling of een XMLport.</span><span class="sxs-lookup"><span data-stu-id="93bbf-105">You perform this work in the **XML Schema Viewer** window by loading the XML schema file, selecting the relevant data elements, and then initializing either a data exchange definition or an XMLport.</span></span>  

 <span data-ttu-id="93bbf-106">Wanneer u hebt gedefinieerd welke gegevenselementen worden opgenomen op basis van het XML-schema, kunt u de actie **XMLport genereren** gebruiken om het XMLport-object te maken.</span><span class="sxs-lookup"><span data-stu-id="93bbf-106">When you have defined which data elements to include based on the XML schema, you can use the **Generate XMLport** action to create the XMLport object.</span></span>  

 <span data-ttu-id="93bbf-107">U kunt ook de actie **Gegevensuitwisselingsdefinitie aanmaken** gebruiken om een definitie voor gegevensuitwisseling te initialiseren die is gebaseerd op de geselecteerde gegevenselementen, die u vervolgens voltooit in het kader voor gegevensuitwisseling.</span><span class="sxs-lookup"><span data-stu-id="93bbf-107">Alternatively, you can use the **Generate Data Exchange Definition** action to initialize a data exchange definition based on the selected data elements, which you then complete in the Data Exchange Framework.</span></span> <span data-ttu-id="93bbf-108">Hiermee wordt een record gemaakt in het venster **Uitwisselingsdefinitie van boeking** waar u verdergaat door te bepalen welke elementen in het bestand worden gekoppeld aan welke velden in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="93bbf-108">This creates a record in the **Posting Exchange Definition** window where you continue by defining which elements in the file map to which fields in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="93bbf-109">Zie [Procedure: Definities voor gegevensuitwisseling instellen](across-how-to-set-up-data-exchange-definitions.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="93bbf-109">For more information, see [How to: Set Up Data Exchange Definitions](across-how-to-set-up-data-exchange-definitions.md).</span></span>  

 <span data-ttu-id="93bbf-110">Dit onderwerp bevat de volgende procedures:</span><span class="sxs-lookup"><span data-stu-id="93bbf-110">This topic contains the following procedures:</span></span>  

-   <span data-ttu-id="93bbf-111">Een XML-schemabestand laden</span><span class="sxs-lookup"><span data-stu-id="93bbf-111">To load an XML schema file</span></span>  

-   <span data-ttu-id="93bbf-112">Knooppunten in een XML-schema selecteren of wissen</span><span class="sxs-lookup"><span data-stu-id="93bbf-112">To select or clear nodes in an XML schema</span></span>  

-   <span data-ttu-id="93bbf-113">De definitie van een gegevensuitwisseling genereren die is gebaseerd op een XML-schema</span><span class="sxs-lookup"><span data-stu-id="93bbf-113">To generate a data exchange definition that is based on an XML schema</span></span>  

-   <span data-ttu-id="93bbf-114">Een XMLport genereren voor het bestand dat is gebaseerd op een XML-schema</span><span class="sxs-lookup"><span data-stu-id="93bbf-114">To generate an XMLport for the file that is based on an XML schema</span></span>  

-   <span data-ttu-id="93bbf-115">Een XMLport in Object Designer importeren</span><span class="sxs-lookup"><span data-stu-id="93bbf-115">To import an XMLport into the Object Designer</span></span>  

### <a name="to-load-an-xml-schema-file"></a><span data-ttu-id="93bbf-116">Een XML-schemabestand laden</span><span class="sxs-lookup"><span data-stu-id="93bbf-116">To load an XML schema file</span></span>  

1.  <span data-ttu-id="93bbf-117">Zorg dat het relevante XML-schemabestand beschikbaar is.</span><span class="sxs-lookup"><span data-stu-id="93bbf-117">Make sure that the relevant XML schema file is available.</span></span> <span data-ttu-id="93bbf-118">De bestandextensie is .xsd.</span><span class="sxs-lookup"><span data-stu-id="93bbf-118">The file extension is .xsd.</span></span>  

2.  <span data-ttu-id="93bbf-119">Voer in het vak **Zoeken** **XML-schema's** in en kies de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="93bbf-119">In the **Search** box, enter **XML Schemas**, and then choose the related link.</span></span>  

3.  <span data-ttu-id="93bbf-120">Kies op het tabblad **Start** in de groep **Nieuw** de optie **Nieuw**.</span><span class="sxs-lookup"><span data-stu-id="93bbf-120">On the **Home** tab, in the **New** group, choose **New**.</span></span>  

4.  <span data-ttu-id="93bbf-121">Vul de velden in zoals beschreven in de volgende tabel.</span><span class="sxs-lookup"><span data-stu-id="93bbf-121">Fill the fields as described in the following table.</span></span>  

    |<span data-ttu-id="93bbf-122">Veld</span><span class="sxs-lookup"><span data-stu-id="93bbf-122">Field</span></span>|<span data-ttu-id="93bbf-123">Description</span><span class="sxs-lookup"><span data-stu-id="93bbf-123">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="93bbf-124">**Code**</span><span class="sxs-lookup"><span data-stu-id="93bbf-124">**Code**</span></span>|<span data-ttu-id="93bbf-125">Geef een code op ter identificatie van het XML-schema.</span><span class="sxs-lookup"><span data-stu-id="93bbf-125">Specify a code to identify the XML schema.</span></span>|  
    |<span data-ttu-id="93bbf-126">**Beschrijving**</span><span class="sxs-lookup"><span data-stu-id="93bbf-126">**Description**</span></span>|<span data-ttu-id="93bbf-127">Geef een omschrijving op van het XML-schema.</span><span class="sxs-lookup"><span data-stu-id="93bbf-127">Specify a description of the XML schema.</span></span>|  

     <span data-ttu-id="93bbf-128">Het veld **Doelnaamspace** bevat elke naamruimte in het XML-schemabestand dat is geladen voor de regel.</span><span class="sxs-lookup"><span data-stu-id="93bbf-128">The **Target Namespace** field specifies any namespace in the XML schema file that has been loaded for the line.</span></span>  

5.  <span data-ttu-id="93bbf-129">Kies op het tabblad **Start** in de groep **Verwerken** de optie **Schema laden** en selecteer vervolgens het XML-schemabestand.</span><span class="sxs-lookup"><span data-stu-id="93bbf-129">On the **Home** tab, in the **Process** group, choose **Load Schema**, and then select the XML schema file.</span></span>  

     <span data-ttu-id="93bbf-130">Wanneer het bestand is geladen, worden de overige velden op de regel gevuld met informatie uit het bestand en wordt het selectievakje **Schema is geladen** ingeschakeld.</span><span class="sxs-lookup"><span data-stu-id="93bbf-130">When the file is loaded, the rest of the fields on the line are filled with information from the file, and the **Schema is Loaded** check box is selected.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="93bbf-131">De structuur van het geladen XML-schema is standaard samengevouwen.</span><span class="sxs-lookup"><span data-stu-id="93bbf-131">The tree of the loaded XML schema is collapsed by default.</span></span> <span data-ttu-id="93bbf-132">U kunt een knooppunt uitvouwen door de knop **+** op het knooppunt te kiezen.</span><span class="sxs-lookup"><span data-stu-id="93bbf-132">You expand each node by choosing the **+** button on the node.</span></span> <span data-ttu-id="93bbf-133">Kies **Alles uitvouwen** op het lint om alle knooppunten uit te vouwen.</span><span class="sxs-lookup"><span data-stu-id="93bbf-133">To expand all nodes, choose **Expand All** on the ribbon.</span></span>  

### <a name="to-select-or-clear-nodes-in-an-xml-schema"></a><span data-ttu-id="93bbf-134">Knooppunten in een XML-schema selecteren of wissen</span><span class="sxs-lookup"><span data-stu-id="93bbf-134">To select or clear nodes in an XML schema</span></span>  

1.  <span data-ttu-id="93bbf-135">In het vak **Zoeken** voert u **XML-schemaviewer** in en vervolgens kiest u de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="93bbf-135">In the **Search** box, enter **XML Schema Viewer**, and then choose the related link.</span></span>  

2.  <span data-ttu-id="93bbf-136">Vul de velden in voor de kop, zoals in de volgende tabel is beschreven.</span><span class="sxs-lookup"><span data-stu-id="93bbf-136">Fill the fields on the header as described in the following table.</span></span>  

    |<span data-ttu-id="93bbf-137">Veld</span><span class="sxs-lookup"><span data-stu-id="93bbf-137">Field</span></span>|<span data-ttu-id="93bbf-138">Description</span><span class="sxs-lookup"><span data-stu-id="93bbf-138">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="93bbf-139">**Schemacode XML**</span><span class="sxs-lookup"><span data-stu-id="93bbf-139">**XML Schema Code**</span></span>|<span data-ttu-id="93bbf-140">Geef het XML-schemabestand op dat u hebt geladen in stap 5 in het gedeelte "Een XML-schemabestand laden".</span><span class="sxs-lookup"><span data-stu-id="93bbf-140">Specify the XML schema file that you loaded in step 5 in the “To load an XML schema file” section.</span></span>|  
    |<span data-ttu-id="93bbf-141">**Nieuw XMLport-nummer**</span><span class="sxs-lookup"><span data-stu-id="93bbf-141">**New XMLport No.**</span></span>|<span data-ttu-id="93bbf-142">Geef het nummer op van de XMLport die is gemaakt op basis van dit XML-schema wanneer u de actie **XMLPort genereren** kiest.</span><span class="sxs-lookup"><span data-stu-id="93bbf-142">Specify the number of the XMLport that is created from this XML schema when you choose the **Generate XMLport** action.</span></span>|  

     <span data-ttu-id="93bbf-143">De regels worden nu gevuld met knooppunten die alle onderdelen in het XML-schema vertegenwoordigen.</span><span class="sxs-lookup"><span data-stu-id="93bbf-143">The lines are now filled with nodes representing all elements in the XML schema.</span></span> <span data-ttu-id="93bbf-144">Knooppunten voor elementen die verplicht zijn volgens het XML-schema, worden standaard geselecteerd.</span><span class="sxs-lookup"><span data-stu-id="93bbf-144">Nodes for elements that are mandatory according to the XML schema are selected by default.</span></span>  

3.  <span data-ttu-id="93bbf-145">Vouw op de eerste regel in de kolom **Knooppuntnaam** het knooppunt **Document** uit en vouw vervolgens geleidelijk onderliggende knooppunten uit die u wilt controleren.</span><span class="sxs-lookup"><span data-stu-id="93bbf-145">On the first line, in the **Node Name** column, expand the **Document** node, and then gradually expand underlying nodes that you want to review.</span></span>  

     <span data-ttu-id="93bbf-146">U kunt ook met de rechtermuisknop op een knooppunt klikken en **Alles uitvouwen** kiezen.</span><span class="sxs-lookup"><span data-stu-id="93bbf-146">Alternatively, right-click on a node and then choose **Expand All**.</span></span>  

4.  <span data-ttu-id="93bbf-147">Kies op het tabblad **Start** in de groep **Weergeven** een van de volgende acties om te wijzigen welke knooppunten worden weergegeven.</span><span class="sxs-lookup"><span data-stu-id="93bbf-147">On the **Home** tab, in the **View** group, choose either of the following actions to change which nodes are displayed.</span></span>  

    |<span data-ttu-id="93bbf-148">**Actie**</span><span class="sxs-lookup"><span data-stu-id="93bbf-148">**Action**</span></span>|<span data-ttu-id="93bbf-149">Description</span><span class="sxs-lookup"><span data-stu-id="93bbf-149">Description</span></span>|  
    |----------------|---------------------------------------|  
    |<span data-ttu-id="93bbf-150">**Alles weergeven**</span><span class="sxs-lookup"><span data-stu-id="93bbf-150">**Show All**</span></span>|<span data-ttu-id="93bbf-151">Alle knooppunten worden weergegeven.</span><span class="sxs-lookup"><span data-stu-id="93bbf-151">All nodes are shown.</span></span>|  
    |<span data-ttu-id="93bbf-152">**Niet-verplicht verbergen**</span><span class="sxs-lookup"><span data-stu-id="93bbf-152">**Hide Non-Mandatory**</span></span>|<span data-ttu-id="93bbf-153">Alleen knooppunten die elementen vertegenwoordigen die vereist zijn volgens het XML-schema, worden weergegeven.</span><span class="sxs-lookup"><span data-stu-id="93bbf-153">Only nodes representing elements that are required according to the XML schema are shown.</span></span> <span data-ttu-id="93bbf-154">Deze knooppunten worden doorgaans aangegeven met een **1** in het veld **MinOcurrs**.</span><span class="sxs-lookup"><span data-stu-id="93bbf-154">These nodes are typically indicated by a **1** in the **MinOccurs** field.</span></span><br /><br /> <span data-ttu-id="93bbf-155">Kies **Alles weergeven** om de weergave om te keren.</span><span class="sxs-lookup"><span data-stu-id="93bbf-155">Choose **Show All** to reverse the view.</span></span>|  
    |<span data-ttu-id="93bbf-156">**Niet-geselecteerd verbergen**</span><span class="sxs-lookup"><span data-stu-id="93bbf-156">**Hide Non-Selected**</span></span>|<span data-ttu-id="93bbf-157">Alleen knooppunten waarbij het selectievakje **Geselecteerd** is ingeschakeld, worden weergegeven.</span><span class="sxs-lookup"><span data-stu-id="93bbf-157">Only nodes where the **Selected** check box is selected are shown.</span></span><br /><br /> <span data-ttu-id="93bbf-158">Kies **Alles weergeven** om de weergave om te keren.</span><span class="sxs-lookup"><span data-stu-id="93bbf-158">Choose **Show All** to reverse the view.</span></span>|  

5.  <span data-ttu-id="93bbf-159">Kies op het tabblad **Home** in de groep **Beheren** de optie **Bewerken**.</span><span class="sxs-lookup"><span data-stu-id="93bbf-159">On the **Home** tab, in the **Manage** group, choose **Edit**.</span></span>  

6.  <span data-ttu-id="93bbf-160">Geef met het selectievakje **Geselecteerd** voor elk knooppunt aan of u wilt dat het element wordt ondersteund in de definitie voor gegevensuitwisseling voor het gerelateerde SEPA-bankbestand.</span><span class="sxs-lookup"><span data-stu-id="93bbf-160">In the **Selected** check box, specify for each node if you want the element to be supported in the data exchange definition for the related SEPA bank file.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="93bbf-161">Wanneer u een verplicht onderliggend knooppunt selecteert, worden alle bovenliggende knooppunten ook geselecteerd.</span><span class="sxs-lookup"><span data-stu-id="93bbf-161">When you select a mandatory child node, all parent nodes above it are also selected.</span></span>  

7.  <span data-ttu-id="93bbf-162">Kies de actie **Alle verplichte elementen selecteren** om alle knooppunten opnieuw te selecteren die elementen voorstellen die verplicht zijn volgens het XML-schema.</span><span class="sxs-lookup"><span data-stu-id="93bbf-162">Choose the **Select All Mandatory Elements** action to reselect all nodes that represent elements that are mandatory according to the XML schema.</span></span>  

8.  <span data-ttu-id="93bbf-163">Kies de actie **Alles deselecteren** om alle selecties te wissen.</span><span class="sxs-lookup"><span data-stu-id="93bbf-163">Choose the **Deselect All** action to clear all selections.</span></span>  

     <span data-ttu-id="93bbf-164">Het veld **Keuze** geeft aan of het knooppunt twee of meer knooppunten op hetzelfde niveau heeft die functioneren als opties.</span><span class="sxs-lookup"><span data-stu-id="93bbf-164">The **Choice** field specifies that the node has two or more sibling nodes that function as options.</span></span>  

### <a name="to-generate-a-data-exchange-definition-that-is-based-on-an-xml-schema"></a><span data-ttu-id="93bbf-165">De definitie van een gegevensuitwisseling genereren die is gebaseerd op een XML-schema</span><span class="sxs-lookup"><span data-stu-id="93bbf-165">To generate a data exchange definition that is based on an XML schema</span></span>  

1.  <span data-ttu-id="93bbf-166">In het vak **Zoeken** voert u **XML-schema's** in en vervolgens kiest u de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="93bbf-166">In the **Search** box, enter  **XML Schemas**, and then choose the related link.</span></span>  

2.  <span data-ttu-id="93bbf-167">Selecteer het betreffende XML-schema en kies op het tabblad **Start** in de groep **Verwerken** de optie **XML-schema-viewer openen**.</span><span class="sxs-lookup"><span data-stu-id="93bbf-167">Select the relevant XML schema, and then on the on the **Home** tab, in the **Process** group, choose **Open XML Schema Viewer**.</span></span>  

3.  <span data-ttu-id="93bbf-168">Zorg dat de relevante knooppunten zijn geselecteerd.</span><span class="sxs-lookup"><span data-stu-id="93bbf-168">Make sure the relevant nodes are selected.</span></span> <span data-ttu-id="93bbf-169">Zie voor meer informatie het gedeelte "Knooppunten selecteren of wissen in een XML-schema".</span><span class="sxs-lookup"><span data-stu-id="93bbf-169">For more information, see the “To select or clear nodes in an XML schema” section.</span></span>  

4.  <span data-ttu-id="93bbf-170">Kies in het venster **XML-schemaviewer** op het tabblad **Start** in de groep **Verwerken** de optie **Definities van gegevensuitwisseling genereren**.</span><span class="sxs-lookup"><span data-stu-id="93bbf-170">In the **XML Schema Viewer** window, on the **Home** tab, in the **Process** group, choose **Generate Data Exchange Definition**.</span></span>  

 <span data-ttu-id="93bbf-171">In het venster **Uitwisselingsdefinitie van boeking** wordt een definitie voor gegevensuitwisseling gemaakt die u kunt invullen om op te geven welke elementen in het bestand moeten worden toegewezen aan welke velden in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="93bbf-171">A data exchange definition is created in the **Posting Exchange Definition** window, which you can complete by specifying which elements in the file map to which fields in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="93bbf-172">Zie [Procedure: Definities voor gegevensuitwisseling instellen](across-how-to-set-up-data-exchange-definitions.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="93bbf-172">For more information, see [How to: Set Up Data Exchange Definitions](across-how-to-set-up-data-exchange-definitions.md).</span></span>  

> [!NOTE]  
>  <span data-ttu-id="93bbf-173">U kunt ook de functie **Bestandstructuur ophalen** in het venster **Uitwisselingsdefinitie van boeking** gebruiken. Deze maakt gebruik van de functionaliteit van het venster **XML-schemaviewer** om het sneltabblad **Kolomdefinities** vooraf te vullen.</span><span class="sxs-lookup"><span data-stu-id="93bbf-173">You can also use the **Get File Structure** function from the **Posting Exchange Definition** window, which uses the functionality of the **XML Schema Viewer** window to prefill the **Column Definitions** TastTab.</span></span>  

### <a name="to-generate-an-xmlport-that-is-based-on-an-xml-schema"></a><span data-ttu-id="93bbf-174">Een XMLport genereren dat is gebaseerd op een XML-schema</span><span class="sxs-lookup"><span data-stu-id="93bbf-174">To generate an XMLport that is based on an XML schema</span></span>  

1.  <span data-ttu-id="93bbf-175">In het vak **Zoeken** voert u **XML-schema's** in en vervolgens kiest u de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="93bbf-175">In the **Search** box, enter  **XML Schemas**, and then choose the related link.</span></span>  

2.  <span data-ttu-id="93bbf-176">Selecteer het betreffende XML-schema en kies op het tabblad **Start** in de groep **Verwerken** de optie **XML-schemaviewer openen**.</span><span class="sxs-lookup"><span data-stu-id="93bbf-176">Select the relevant XML schema, and then on the on the **Home** tab, in the **Process** group, choose **Open XML Schema Viewer**.</span></span>  

3.  <span data-ttu-id="93bbf-177">Geef in het veld **Nieuw XMLport-nummer**</span><span class="sxs-lookup"><span data-stu-id="93bbf-177">In the **New XMLport No.**</span></span> <span data-ttu-id="93bbf-178">het nummer op dat het nieuwe XMLport-object krijgt wanneer het wordt gegenereerd.</span><span class="sxs-lookup"><span data-stu-id="93bbf-178">field, specify the number that the new XMLport object will be given when it is generated.</span></span>  

4.  <span data-ttu-id="93bbf-179">Zorg dat de relevante knooppunten zijn geselecteerd.</span><span class="sxs-lookup"><span data-stu-id="93bbf-179">Make sure the relevant nodes are selected.</span></span> <span data-ttu-id="93bbf-180">Zie voor meer informatie het gedeelte "Knooppunten selecteren of wissen in een XML-schema".</span><span class="sxs-lookup"><span data-stu-id="93bbf-180">For more information, see the “To select or clear nodes in an XML schema” section.</span></span>  

5.  <span data-ttu-id="93bbf-181">Kies op het tabblad **Start** in de groep **Verwerken** de optie **XMLport genereren** en sla het object als een .txt-bestand op in een geschikte vestiging.</span><span class="sxs-lookup"><span data-stu-id="93bbf-181">On the **Home** tab, in the **Process** group, choose **Generate XMLport**, and then save the object as a .txt file in an appropriate location.</span></span>  

6. <span data-ttu-id="93bbf-182">Importeer de nieuwe XMLport in de [!INCLUDE[d365fin](includes/d365fin_md.md)]-ontwikkelingsomgeving en compileer deze.</span><span class="sxs-lookup"><span data-stu-id="93bbf-182">Import the new XMLport into the [!INCLUDE[d365fin](includes/d365fin_md.md)] development environment and compile it.</span></span>

## <a name="see-also"></a><span data-ttu-id="93bbf-183">Zie ook</span><span class="sxs-lookup"><span data-stu-id="93bbf-183">See Also</span></span>  
<span data-ttu-id="93bbf-184">[Procedure: Definities voor gegevensuitwisseling instellen](across-how-to-set-up-data-exchange-definitions.md) </span><span class="sxs-lookup"><span data-stu-id="93bbf-184">[How to: Set Up Data Exchange Definitions](across-how-to-set-up-data-exchange-definitions.md) </span></span>  
<span data-ttu-id="93bbf-185">[Procedure: Betalingen naar een bankbestand exporteren](payables-how-export-payments-bank-file.md) </span><span class="sxs-lookup"><span data-stu-id="93bbf-185">[How to: Export Payments to a Bank File](payables-how-export-payments-bank-file.md) </span></span>  
<span data-ttu-id="93bbf-186">[Betalingen verzamelen via automatische incasso van SEPA](finance-collect-payments-with-sepa-direct-debit.md) </span><span class="sxs-lookup"><span data-stu-id="93bbf-186">[Collecting Payments with SEPA Direct Debit](finance-collect-payments-with-sepa-direct-debit.md) </span></span>  
[<span data-ttu-id="93bbf-187">Over het kader voor gegevensuitwisseling</span><span class="sxs-lookup"><span data-stu-id="93bbf-187">About the Data Exchange Framework</span></span>](across-about-the-data-exchange-framework.md)

