---
title: Begrijpen hoe u inkoopdocumenten boekt
description: Leren over de verschillende boekingsfuncties om inkoopdocumenten te boeken.
documentationcenter: 
author: SusanneWindfeldPedersen
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 05/12/2017
ms.author: solsen
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 9f9320495accdd08700b67e68edb1d5692990179
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="posting-purchases"></a><span data-ttu-id="e1e38-103">Inkopen boeken</span><span class="sxs-lookup"><span data-stu-id="e1e38-103">Posting Purchases</span></span>
<span data-ttu-id="e1e38-104">In de **Boekingsgroep** op een inkoopdocument kunt u kiezen uit de volgende boekingsfuncties:</span><span class="sxs-lookup"><span data-stu-id="e1e38-104">In the **Posting group** on a purchase document, you can choose between the following posting functions:</span></span>

* <span data-ttu-id="e1e38-105">**Boeken**</span><span class="sxs-lookup"><span data-stu-id="e1e38-105">**Post**</span></span>
* <span data-ttu-id="e1e38-106">**Voorbeeld van boeking weergeven**</span><span class="sxs-lookup"><span data-stu-id="e1e38-106">**Preview Posting**</span></span>
* <span data-ttu-id="e1e38-107">**Boeken en afdrukken**</span><span class="sxs-lookup"><span data-stu-id="e1e38-107">**Post and Print**</span></span>
* <span data-ttu-id="e1e38-108">**Testrapport**</span><span class="sxs-lookup"><span data-stu-id="e1e38-108">**Test Report**</span></span>
* <span data-ttu-id="e1e38-109">**Batchboeken**</span><span class="sxs-lookup"><span data-stu-id="e1e38-109">**Post Batch**</span></span>

<span data-ttu-id="e1e38-110">Wanneer u alle regels hebt ingevuld en alle informatie hebt ingevoerd op de inkooporder, kunt u de order boeken. Dit houdt in dat u een ontvangst en een factuur maakt.</span><span class="sxs-lookup"><span data-stu-id="e1e38-110">When you have completed all the lines and entered all the information on the purchase order, you can post it, that is, create a receipt and an invoice.</span></span>

<span data-ttu-id="e1e38-111">Wanneer een inkooporder wordt geboekt, worden de rekening van de leverancier, het grootboek en de artikelposten bijgewerkt.</span><span class="sxs-lookup"><span data-stu-id="e1e38-111">When a purchase order is posted, the vendor's account, the general ledger, and the item ledger entries are updated.</span></span>

<span data-ttu-id="e1e38-112">Voor elke inkooporder wordt een inkooppost gemaakt in de tabel **Grootboekpost**.</span><span class="sxs-lookup"><span data-stu-id="e1e38-112">For each purchase order, a purchase entry is created in the **G/L Entry** table.</span></span> <span data-ttu-id="e1e38-113">Ook wordt een post in de leveranciersrekening in de tabel **Leverancierspost** gemaakt en wordt er een grootboekpost in de betreffende schuldenrekening gemaakt.</span><span class="sxs-lookup"><span data-stu-id="e1e38-113">An entry is also created in the vendor's account in the **Vendor Ledger Entry** table and a G/L entry is created in the relevant payables account.</span></span> <span data-ttu-id="e1e38-114">Bovendien kan het boeken van de order resulteren in een btw-post en een grootboekpost voor de totale korting.</span><span class="sxs-lookup"><span data-stu-id="e1e38-114">In addition, posting the order may result in a VAT entry and a G/L entry for the discount amount.</span></span> <span data-ttu-id="e1e38-115">Of er een post voor de korting wordt geboekt, wordt bepaald door de inhoud van het veld **Korting boeken** in het venster **Inkoopinstellingen**.</span><span class="sxs-lookup"><span data-stu-id="e1e38-115">Whether an entry for the discount is posted depends on the contents of the **Discount Posting** field in the **Purchases & Payables Setup** window.</span></span>

<span data-ttu-id="e1e38-116">Voor elke inkooporderregel wordt een artikelpost gemaakt in de tabel **Artikelpost** (als op de inkoopregels artikelnummers staan) of een grootboekpost in de tabel **Grootboekpost** (als op de inkoopregels een grootboekrekening staat).</span><span class="sxs-lookup"><span data-stu-id="e1e38-116">For each purchase order line, an item ledger entry will be created in the **Item Ledger Entry** table (if the purchase lines contain item numbers) or a G/L entry will be created in the **G/L Entry** table (if the purchase lines contain a G/L account).</span></span> <span data-ttu-id="e1e38-117">Daarnaast worden inkooporders altijd vastgelegd in de tabellen **Inkoopontvangst** en **Inkoopfactuur**.</span><span class="sxs-lookup"><span data-stu-id="e1e38-117">In addition, purchase orders are always recorded in the **Purch. Recpt. Header** and **Purch. Inv. Header** tables.</span></span>

<span data-ttu-id="e1e38-118">Voordat u gaat boeken, kunt u een controlelijst afdrukken met alle informatie uit de inkooporder en eventuele fouten die erin voorkomen.</span><span class="sxs-lookup"><span data-stu-id="e1e38-118">Before you start to post, you can print a test report that contains all the information in the purchase order and indicates any errors there.</span></span> <span data-ttu-id="e1e38-119">Kies **Boeken** en vervolgens **Testrapport** als u het rapport wilt afdrukken.</span><span class="sxs-lookup"><span data-stu-id="e1e38-119">To print the report, choose **Posting**, and then choose **Test Report**.</span></span>

> [!IMPORTANT]  
>   <span data-ttu-id="e1e38-120">Tijdens het boeken van een order kunt u zowel een ontvangst als een factuur maken.</span><span class="sxs-lookup"><span data-stu-id="e1e38-120">When you post an order, you can create both a receipt and an invoice.</span></span> <span data-ttu-id="e1e38-121">Deze kunt u tegelijkertijd, maar ook onafhankelijk van elkaar maken.</span><span class="sxs-lookup"><span data-stu-id="e1e38-121">These can be done simultaneously or independently.</span></span> <span data-ttu-id="e1e38-122">U kunt ook een gedeeltelijke ontvangst en een gedeeltelijke factuur maken door de velden **Te ontvangen aantal** en **Te factureren aantal** op de afzonderlijke inkooporderregels in te vullen voordat u de boeking uitvoert.</span><span class="sxs-lookup"><span data-stu-id="e1e38-122">You can also create a partial receipt and a partial invoice by completing the **Qty. to Receive** and **Qty. to Invoice** fields on the individual purchase order lines before you post.</span></span> <span data-ttu-id="e1e38-123">U kunt geen factuur maken voor iets dat niet is ontvangen.</span><span class="sxs-lookup"><span data-stu-id="e1e38-123">Note that you cannot create an invoice for something that has not been received.</span></span> <span data-ttu-id="e1e38-124">Dit betekent dat u pas kunt factureren als er een ontvangst is vastgelegd, of u moet tegelijkertijd ontvangen en factureren.</span><span class="sxs-lookup"><span data-stu-id="e1e38-124">That is, before you can invoice, you must have recorded a receipt, or you must choose to receive and invoice at the same time.</span></span>

<span data-ttu-id="e1e38-125">U kunt de optie Boeken of Boeken en afdrukken kiezen.</span><span class="sxs-lookup"><span data-stu-id="e1e38-125">You can either post, or post and print.</span></span> <span data-ttu-id="e1e38-126">Als u ervoor kiest om te boeken en af te drukken, wordt een lijst afgedrukt nadat de order is geboekt.</span><span class="sxs-lookup"><span data-stu-id="e1e38-126">If you choose to post and print, a report is printed when the order is posted.</span></span> <span data-ttu-id="e1e38-127">U kunt ook de functie **Batchboeken** kiezen, waarmee u verschillende orders tegelijkertijd kunt boeken.</span><span class="sxs-lookup"><span data-stu-id="e1e38-127">You can also choose the **Post Batch** function, which lets you post several orders at the same time.</span></span>

<span data-ttu-id="e1e38-128">Na de boeking worden de geboekte inkoopregels verwijderd uit de order.</span><span class="sxs-lookup"><span data-stu-id="e1e38-128">When the posting is completed, the posted purchase lines are removed from the order.</span></span> <span data-ttu-id="e1e38-129">Er verschijnt een bericht als de boeking is voltooid.</span><span class="sxs-lookup"><span data-stu-id="e1e38-129">A message tells you when the posting is completed.</span></span> <span data-ttu-id="e1e38-130">Hierna kunt u de geboekte posten bekijken in de verschillende vensters die geboekte posten bevatten, zoals de vensters **Leveranciersposten**, **Grootboekposten**, **Artikelposten**, **Geboekte inkoopontvangsten** en **Geboekte inkoopfacturen**.</span><span class="sxs-lookup"><span data-stu-id="e1e38-130">After this, you will be able to see the posted entries in the various windows that contain posted entries, such as the **Vendor Ledger Entries**, **G/L Entries**, **Item Ledger Entries**, **Purchase Receipts**, and **Posted Purchase Invoices** windows.</span></span>

## <a name="see-also"></a><span data-ttu-id="e1e38-131">Zie ook</span><span class="sxs-lookup"><span data-stu-id="e1e38-131">See Also</span></span>
[<span data-ttu-id="e1e38-132">Inkoop</span><span class="sxs-lookup"><span data-stu-id="e1e38-132">Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="e1e38-133">Documenten en dagboeken boeken</span><span class="sxs-lookup"><span data-stu-id="e1e38-133">Post Documents and Journals</span></span>](ui-post-documents-journals.md)  
<span data-ttu-id="e1e38-134">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="e1e38-134">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>


