---
title: Responsberichten van de belastingdienst verwerken
description: Als u een elektronische btw- of ICP-aangifte verzendt naar de belastingdienst, wordt de aangifte verwerkt en wordt u in reactie een bericht gestuurd.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 3698f57c9ba835d36356da85adcf7658059ea99a
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-process-response-messages-from-tax-authorities"></a><span data-ttu-id="90f34-103">Procedure: Responsberichten van de belastingdienst verwerken</span><span class="sxs-lookup"><span data-stu-id="90f34-103">How to: Process Response Messages from Tax Authorities</span></span>
<span data-ttu-id="90f34-104">Als u een elektronische btw- of ICP-aangifte verzendt naar de belastingdienst, wordt de aangifte verwerkt en wordt u in reactie een bericht gestuurd.</span><span class="sxs-lookup"><span data-stu-id="90f34-104">When you submit a VAT or ICP declaration to the tax authorities electronically, they will process the declaration and send you a message in response.</span></span>  
  
 <span data-ttu-id="90f34-105">U kunt de respons in [!INCLUDE[navnow](../../includes/navnow_md.md)] importeren met de batchverwerking **Responsberichten ontvangen**.</span><span class="sxs-lookup"><span data-stu-id="90f34-105">You can import the response into [!INCLUDE[navnow](../../includes/navnow_md.md)] by using the **Receive Response Messages** batch job.</span></span> <span data-ttu-id="90f34-106">Het responsbericht bevat de status van de aangifte.</span><span class="sxs-lookup"><span data-stu-id="90f34-106">The response message will contain the status of the declaration.</span></span>  
  
### <a name="to-import-messages-from-the-tax-authorities-server"></a><span data-ttu-id="90f34-107">Berichten importeren van de server van de belastingdienst</span><span class="sxs-lookup"><span data-stu-id="90f34-107">To import messages from the tax authorities' server</span></span>  
  
1.  <span data-ttu-id="90f34-108">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Responsberichten elektronische aangiften** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="90f34-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Elec. Tax Decl. Response Msgs.**, and then choose the related link.</span></span>  
  
2.  <span data-ttu-id="90f34-109">Kies op het tabblad **Start** in de groep **Verwerken** de optie **Responsberichten ontvangen**.</span><span class="sxs-lookup"><span data-stu-id="90f34-109">On the **Home** tab, in the **Process** group, choose **Receive Response Messages**.</span></span>  
  
3.  <span data-ttu-id="90f34-110">Vul op het sneltabblad **Opties** de velden in, zoals in de volgende tabel is beschreven.</span><span class="sxs-lookup"><span data-stu-id="90f34-110">On the **Options** FastTab, fill in the fields as described in the following table.</span></span>  
  
    |<span data-ttu-id="90f34-111">Veld</span><span class="sxs-lookup"><span data-stu-id="90f34-111">Field</span></span>|<span data-ttu-id="90f34-112">Description</span><span class="sxs-lookup"><span data-stu-id="90f34-112">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="90f34-113">**Wachtwoord versleuteling CA-certificaat**</span><span class="sxs-lookup"><span data-stu-id="90f34-113">**CA Certificate Encryption Password**</span></span>|<span data-ttu-id="90f34-114">Het wachtwoord dat is gebruikt wordt om de CA-certificaten te versleutelen.</span><span class="sxs-lookup"><span data-stu-id="90f34-114">The password that was used to encrypt the Certificate Authorities' certificates.</span></span>|  
    |<span data-ttu-id="90f34-115">**Wachtwoord gebruikerscertificaat**</span><span class="sxs-lookup"><span data-stu-id="90f34-115">**User Certificate Password**</span></span>|<span data-ttu-id="90f34-116">Het wachtwoord dat gebruikt wordt om de gebruikerscertificaten te versleutelen.</span><span class="sxs-lookup"><span data-stu-id="90f34-116">The password that is used to encrypt the user certificates.</span></span>|  
  
4.  <span data-ttu-id="90f34-117">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="90f34-117">Choose the **OK** button.</span></span>  
  
### <a name="to-process-the-response-messages-from-the-tax-authorities"></a><span data-ttu-id="90f34-118">Responsberichten van de belastingdienst verwerken</span><span class="sxs-lookup"><span data-stu-id="90f34-118">To process the response messages from the tax authorities</span></span>  
  
1.  <span data-ttu-id="90f34-119">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Responsberichten elektronische aangiften** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="90f34-119">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Elec. Tax Decl. Response Msgs.**, and then choose the related link.</span></span>  
  
2.  <span data-ttu-id="90f34-120">Kies op het tabblad **Start** in de groep **Verwerken** de optie **Responsberichten verwerken**.</span><span class="sxs-lookup"><span data-stu-id="90f34-120">On the **Home** tab, in the **Process** group, choose **Process Response Messages**.</span></span>  
  
3.  <span data-ttu-id="90f34-121">Selecteer in het venster **Batchverwerking Responsberichten verwerken** op het sneltabblad **Elek. aangifteresponsbericht** de juiste filters.</span><span class="sxs-lookup"><span data-stu-id="90f34-121">In the **Process Response Messages Batch Job** window, on the **Elec. Tax Decl. Response Msg**. FastTab, select the appropriate filters.</span></span>  
  
4.  <span data-ttu-id="90f34-122">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="90f34-122">Choose the **OK** button.</span></span>  
  
     <span data-ttu-id="90f34-123">De verwerkte gegevens over het responsbericht wordt weergegeven in het **Responsberichten elektronische aangiften**</span><span class="sxs-lookup"><span data-stu-id="90f34-123">The processed information about the response message is displayed in the **Elec. Tax Decl. Response Msgs.**.</span></span> <span data-ttu-id="90f34-124">in.</span><span class="sxs-lookup"><span data-stu-id="90f34-124">window.</span></span>  
  
5.  <span data-ttu-id="90f34-125">Als u een bericht of bijlage wilt verwerken, kiest u op het tabblad **Acties** in de groep **Functies** **Responsbericht exporteren** of **Responsbijlage exporteren**.</span><span class="sxs-lookup"><span data-stu-id="90f34-125">To export a message or attachment, on the **Actions** tab, in the **Functions** group, choose **Export Response Message** or **Export Response Attachment**.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="90f34-126">Zie ook</span><span class="sxs-lookup"><span data-stu-id="90f34-126">See Also</span></span>  
 <span data-ttu-id="90f34-127">[Elektronische btw- en ICP-aangiften](electronic-vat-and-icp-declarations.md) </span><span class="sxs-lookup"><span data-stu-id="90f34-127">[Electronic VAT and ICP Declarations](electronic-vat-and-icp-declarations.md) </span></span>  
 <span data-ttu-id="90f34-128">[Procedure: Btw-categorieën instellen:](how-to-set-up-vat-categories.md) </span><span class="sxs-lookup"><span data-stu-id="90f34-128">[How to: Set Up VAT Categories](how-to-set-up-vat-categories.md) </span></span>  
 <span data-ttu-id="90f34-129">[Procedure: Elektronische btw- en ICP-aangiften maken](how-to-create-electronic-vat-and-icp-declarations.md) </span><span class="sxs-lookup"><span data-stu-id="90f34-129">[How to: Create Electronic VAT and ICP Declarations](how-to-create-electronic-vat-and-icp-declarations.md) </span></span>  
 <span data-ttu-id="90f34-130">Tabel Elek. aangiftekop</span><span class="sxs-lookup"><span data-stu-id="90f34-130">Elec. Tax Declaration Header Table</span></span>   
 <span data-ttu-id="90f34-131">Tabel Elek. aangifteresponsbericht</span><span class="sxs-lookup"><span data-stu-id="90f34-131">Elec. Tax Decl. Response Msg. Table</span></span>   
 <span data-ttu-id="90f34-132">Batchverwerking Responsberichten ontvangen</span><span class="sxs-lookup"><span data-stu-id="90f34-132">Receive Response Messages Batch Job</span></span>   
 <span data-ttu-id="90f34-133">Batchverwerking Responsberichten verwerken</span><span class="sxs-lookup"><span data-stu-id="90f34-133">Process Response Messages Batch Job</span></span>
