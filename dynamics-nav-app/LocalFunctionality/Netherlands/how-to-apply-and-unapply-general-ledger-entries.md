---
title: Grootboekposten vereffenen en de vereffening ervan ongedaan maken
description: Door tijdelijke grootboekposten te vereffenen kunnen bedrijven werken met tijdelijke rekeningen en transferrekeningen in het grootboek. Tijdelijke en transferrekeningen worden gebruikt om tijdelijke posten op te slaan die op verdere verwerking in het grootboek wachten.
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
ms.openlocfilehash: d22556c7fa33cf03eb6a1573378117af68979c4f
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-apply-and-unapply-general-ledger-entries"></a><span data-ttu-id="56374-104">Procedure: Grootboekposten vereffenen en de vereffening ervan ongedaan maken</span><span class="sxs-lookup"><span data-stu-id="56374-104">How to: Apply and Unapply General Ledger Entries</span></span>
<span data-ttu-id="56374-105">Door tijdelijke grootboekposten te vereffenen kunnen bedrijven werken met tijdelijke rekeningen en transferrekeningen in het grootboek.</span><span class="sxs-lookup"><span data-stu-id="56374-105">Applying temporary general ledger entries allows companies to work with temporary and transfer accounts in the general ledger.</span></span> <span data-ttu-id="56374-106">Tijdelijke en transferrekeningen worden gebruikt om tijdelijke posten op te slaan die op verdere verwerking in het grootboek wachten.</span><span class="sxs-lookup"><span data-stu-id="56374-106">Temporary and transfer accounts are used to store temporary ledger entries that are waiting for further processing into the general ledger.</span></span>  
  
 <span data-ttu-id="56374-107">U kunt tijdelijke rekeningen gebruiken voor:</span><span class="sxs-lookup"><span data-stu-id="56374-107">You can use temporary accounts for:</span></span>  
  
-   <span data-ttu-id="56374-108">Geldtransfers van de ene naar de andere bankrekening.</span><span class="sxs-lookup"><span data-stu-id="56374-108">Money transfers from one bank account to another.</span></span>  
  
-   <span data-ttu-id="56374-109">Financiële transactietransfers van het ene systeem naar het andere, waarbij een deel van de gegevens tijdelijk op het oorspronkelijke systeem staat.</span><span class="sxs-lookup"><span data-stu-id="56374-109">Financial transaction transfers from one system to another in which part of the information temporarily resides on the original system.</span></span>  
  
-   <span data-ttu-id="56374-110">Transacties waarvoor u een verkoopfactuur hebt verzonden naar een klant maar nog niet de bijbehorende inkoopfactuur van de leverancier hebt ontvangen.</span><span class="sxs-lookup"><span data-stu-id="56374-110">Transactions for which you have issued a sales invoice to a customer but have not yet received the corresponding purchase invoice from the vendor.</span></span>  
  
 <span data-ttu-id="56374-111">Nadat de posten zijn verwerkt, kunt u de functie voor postenvereffening gebruiken om de geboekte posten en het boekingsrekeningsoort bij te werken.</span><span class="sxs-lookup"><span data-stu-id="56374-111">When the ledger entries have been processed, you can use the apply entries function to update the posted ledger entries and the posting account type.</span></span>  
  
 <span data-ttu-id="56374-112">U kunt de vereffening van de vereffende grootboekposten ongedaan maken en vervolgens de gesloten posten openen om wijzigingen aan te brengen.</span><span class="sxs-lookup"><span data-stu-id="56374-112">You can unapply the applied general ledger entries and then open the closed entries to make changes.</span></span>  
  
### <a name="to-apply-general-ledger-entries"></a><span data-ttu-id="56374-113">Grootboekposten vereffenen</span><span class="sxs-lookup"><span data-stu-id="56374-113">To apply general ledger entries</span></span>  
  
1.  <span data-ttu-id="56374-114">Voer in het tekstvak **Zoeken** **Grootboekjournalen** in en kies vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="56374-114">In the **Search**  box, enter **G/L Registers**, and then choose the related link.</span></span>  
  
2.  <span data-ttu-id="56374-115">Selecteer een grootboekjournaal en kies op het tabblad **Start** in de groep **Verwerken** de optie **Grootboek**.</span><span class="sxs-lookup"><span data-stu-id="56374-115">Select a general ledger register, and then, on the **Home** tab, in the **Process** group, choose **General Ledger**.</span></span>  
  
3.  <span data-ttu-id="56374-116">Kies in het venster **Grootboekposten** op het tabblad **Start** in de groep **Functies** de optie **Posten vereffenen**.</span><span class="sxs-lookup"><span data-stu-id="56374-116">In the **General Ledger Entries** window, on the **Home** tab, in the **Functions** group, choose **Apply Entries**.</span></span>  
  
     <span data-ttu-id="56374-117">Alle openstaande posten voor de grootboekrekening worden weergegeven in het venster **Grootboekposten vereffenen**.</span><span class="sxs-lookup"><span data-stu-id="56374-117">All open ledger entries for the general ledger account are displayed in the **Apply General Ledger Entries** window.</span></span>  
  
    > [!NOTE]  
    >  <span data-ttu-id="56374-118">Standaard wordt het veld **Posten opnemen** ingesteld op **Open**.</span><span class="sxs-lookup"><span data-stu-id="56374-118">By default, the **Include Entries** field is set to **Open**.</span></span> <span data-ttu-id="56374-119">U kunt de waarde van het veld **Posten opnemen** wijzigen in **Alle** of **Afgesloten**.</span><span class="sxs-lookup"><span data-stu-id="56374-119">You can change the value of the **Include Entries** field to **All** or **Closed**.</span></span> <span data-ttu-id="56374-120">U kunt alleen grootboekposten vereffenen die **open** zijn.</span><span class="sxs-lookup"><span data-stu-id="56374-120">You can only apply general ledger entries that are **Open**.</span></span>  
  
4.  <span data-ttu-id="56374-121">Selecteer de relevante grootboekpost en kies vervolgens op het tabblad **Navigeren** in de groep **Toepassing** de optie **Vereffenings-id instellen**.</span><span class="sxs-lookup"><span data-stu-id="56374-121">Select the relevant general ledger entry, and then, on the **Navigate** tab, in the **Application** group, choose **Set Applies-to ID**.</span></span>  
  
     <span data-ttu-id="56374-122">Het veld **Vereffenings-id** wordt bijgewerkt met de gebruikers-id.</span><span class="sxs-lookup"><span data-stu-id="56374-122">The **Applies-to ID** field is updated with the user ID.</span></span> <span data-ttu-id="56374-123">Het restbedrag wordt weergegeven in het veld **Saldo** in het venster **Grootboekposten vereffenen**.</span><span class="sxs-lookup"><span data-stu-id="56374-123">The remaining amount is displayed in the **Balance** field in the **Apply General Ledger Entries** window.</span></span>  
  
5.  <span data-ttu-id="56374-124">Klik op het tabblad **Navigeren** in de groep **Vereffening** op **Vereffening boeken**.</span><span class="sxs-lookup"><span data-stu-id="56374-124">On the **Navigate** tab, in the **Application** group, choose **Post Application**.</span></span>  
  
     <span data-ttu-id="56374-125">U kunt de vereffening boeken zelfs wanneer het saldobedrag gelijk is aan 0.</span><span class="sxs-lookup"><span data-stu-id="56374-125">You can post the application even if the balance amount is equal to 0.</span></span> <span data-ttu-id="56374-126">Wanneer wordt geboekt, wordt het veld **Restbedrag** als volgt beïnvloed:</span><span class="sxs-lookup"><span data-stu-id="56374-126">When posted, the **Remaining Amount** field is affected as follows:</span></span>  
  
    -   <span data-ttu-id="56374-127">Als het veld **Saldo** gelijk is aan 0, wordt het veld **Restbedrag** bij alle grootboekposten op 0 gezet.</span><span class="sxs-lookup"><span data-stu-id="56374-127">If the **Balance** is equal to 0, then the **Remaining Amount** field on all ledger entries is set to 0.</span></span>  
  
    -   <span data-ttu-id="56374-128">Als het veld **Saldo** niet gelijk is aan 0, wordt het bedrag in het veld **Saldo** overgebracht naar het veld **Restbedrag** van de grootboekpost die was geselecteerd toe u de vereffening boekte.</span><span class="sxs-lookup"><span data-stu-id="56374-128">If the **Balance** is not equal to 0, then the amount in the **Balance** field is transferred to the **Remaining Amount** field for the general ledger entry that was selected when you posted the application.</span></span>  
  
    -   <span data-ttu-id="56374-129">Voor alle overige grootboekposten wordt het veld **Restbedrag** op 0 gezet en worden de velden **Open**, **Afgesloten door volgnr.**, **Afgesloten met bedrag** en **Afgesloten op** bijgewerkt.</span><span class="sxs-lookup"><span data-stu-id="56374-129">For all other general ledger entries, the **Remaining Amount** field is set to 0 and the **Open**, **Closed by Entry No.**, **Closed by Amount**, and **Closed at Date** fields are updated.</span></span>  
  
    > [!NOTE]  
    >  <span data-ttu-id="56374-130">Wanneer wordt geboekt, worden de grootboekposten die het veld **Vereffenings-id** bijwerken, verwijderd.</span><span class="sxs-lookup"><span data-stu-id="56374-130">When posted, the general ledger entries which update the **Applies-to ID** field are deleted.</span></span>  
  
6.  <span data-ttu-id="56374-131">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="56374-131">Choose the **OK** button.</span></span>  
  
### <a name="to-view-the-applied-general-ledger-entries"></a><span data-ttu-id="56374-132">De vereffende grootboekposten weergeven</span><span class="sxs-lookup"><span data-stu-id="56374-132">To view the applied general ledger entries</span></span>  
  
1.  <span data-ttu-id="56374-133">Voer in het tekstvak **Zoeken** **Grootboekjournalen** in en kies vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="56374-133">In the **Search**  box, enter **G/L Registers**, and then choose the related link.</span></span>  
  
2.  <span data-ttu-id="56374-134">Selecteer een grootboekjournaal en kies op het tabblad **Start** in de groep **Verwerken** de optie **Grootboek**.</span><span class="sxs-lookup"><span data-stu-id="56374-134">Select a general ledger register, and then, on the **Home** tab, in the **Process** group, choose **General Ledger**.</span></span>  
  
3.  <span data-ttu-id="56374-135">Selecteer de relevante grootboekpost en kies vervolgens op het tabblad **Navigeren** in de groep **Toepassing** de optie **Vereffende posten**.</span><span class="sxs-lookup"><span data-stu-id="56374-135">Select the relevant general ledger entry, and then, on the **Navigate** tab, in the **Application** group, choose **Applied Entries**.</span></span>  
  
     <span data-ttu-id="56374-136">U kunt alle vereffende grootboekposten weergeven.</span><span class="sxs-lookup"><span data-stu-id="56374-136">You can view all the applied general ledger entries.</span></span>  
  
4.  <span data-ttu-id="56374-137">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="56374-137">Choose the **OK** button.</span></span>  
  
### <a name="to-unapply-general-ledger-entries"></a><span data-ttu-id="56374-138">De vereffening van grootboekposten ongedaan maken</span><span class="sxs-lookup"><span data-stu-id="56374-138">To unapply general ledger entries</span></span>  
  
1.  <span data-ttu-id="56374-139">Voer in het tekstvak **Zoeken** **Grootboekjournalen** in en kies vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="56374-139">In the **Search**  box, enter **G/L Registers**, and then choose the related link.</span></span>  
  
2.  <span data-ttu-id="56374-140">Selecteer een grootboekjournaal en kies op het tabblad **Start** in de groep **Verwerken** de optie **Grootboek**.</span><span class="sxs-lookup"><span data-stu-id="56374-140">Select a general ledger register, and then, on the **Home** tab, in the **Process** group, choose **General Ledger**.</span></span>  
  
3.  <span data-ttu-id="56374-141">Selecteer de grootboekpost waarvan u de vereffening ongedaan wilt maken en kies vervolgens op het tabblad **Navigeren** in de groep **Toepassing** de optie **Vereffening ongedaan maken**.</span><span class="sxs-lookup"><span data-stu-id="56374-141">Select the general ledger entry that you want to unapply, and then, on the **Navigate** tab, in the **Application** group, choose **Undo Application**.</span></span>  
  
     <span data-ttu-id="56374-142">De vereffening van de vereffende grootboekposten wordt ongedaan gemaakt.</span><span class="sxs-lookup"><span data-stu-id="56374-142">The applied general ledger entries are unapplied.</span></span>  
  
    > [!NOTE]  
    >  <span data-ttu-id="56374-143">Als een post is vereffend met meer dan één vereffeningspost, moet u de vereffening van de laatste vereffeningspost het eerst ongedaan maken.</span><span class="sxs-lookup"><span data-stu-id="56374-143">If an entry is applied to more than one application entry, you must unapply the latest application entry first.</span></span> <span data-ttu-id="56374-144">Standaard wordt de laatste post weergegeven.</span><span class="sxs-lookup"><span data-stu-id="56374-144">By default, the latest entry is displayed.</span></span>  
  
4.  <span data-ttu-id="56374-145">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="56374-145">Choose the **OK** button.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="56374-146">Zie ook</span><span class="sxs-lookup"><span data-stu-id="56374-146">See Also</span></span>  
 <span data-ttu-id="56374-147">Grootboekrekening</span><span class="sxs-lookup"><span data-stu-id="56374-147">G/L Account</span></span>   
 <span data-ttu-id="56374-148">Grootboekpost</span><span class="sxs-lookup"><span data-stu-id="56374-148">G/L Entry</span></span>   
 <span data-ttu-id="56374-149">Grootboekposten</span><span class="sxs-lookup"><span data-stu-id="56374-149">General Ledger Entries</span></span>
