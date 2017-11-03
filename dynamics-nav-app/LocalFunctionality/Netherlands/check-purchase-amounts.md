---
title: Inkoopbedragen controleren
description: Voordat u een inkoopfactuur of creditnota boekt, wordt gecontroleerd of het 'bedrag incl. btw' en het 'btw-bedrag' die vermeld staan op het inkooporderdocument gelijk zijn aan het totaalbedrag van de ingevoegde inkoopregels.
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
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 2a4bd22a9778ad0d40b4090cb6db8416232cacd8
ms.contentlocale: nl-nl
ms.lasthandoff: 10/23/2017

---
# <a name="check-purchase-amounts"></a><span data-ttu-id="5e142-103">Inkoopbedragen controleren</span><span class="sxs-lookup"><span data-stu-id="5e142-103">Check Purchase Amounts</span></span>
<span data-ttu-id="5e142-104">Voordat u een inkoopfactuur of creditnota boekt, wordt gecontroleerd of het bedrag incl. btw en het btw-bedrag die vermeld staan op het inkooporderdocument, gelijk zijn aan het totaalbedrag van de ingevoegde inkoopregels.</span><span class="sxs-lookup"><span data-stu-id="5e142-104">Before posting a purchase invoice or credit memo, the program checks if the amount including VAT and the VAT amount stated on the purchase document is equal to the total amount of the inserted purchase lines.</span></span> <span data-ttu-id="5e142-105">Hiervoor moeten de velden **Documentbedrag incl. btw** en **Btw documentbedrag** ingevuld zijn in het venster **Inkoopfactuur** of **Inkoopcreditnota**.</span><span class="sxs-lookup"><span data-stu-id="5e142-105">To do this, the **Doc. Amount Incl. VAT** and **Doc. Amount VAT** fields must be filled in in the **Purchase Invoice** or **Purchase Credit Memo** window.</span></span>  

 <span data-ttu-id="5e142-106">Als er slechts één inkoopregel is of als alle regels vallen onder hetzelfde btw-percentage, wordt het juiste **Btw documentbedrag**-veld automatisch berekend wanneer u de inkoopregels en het veld **Documentbedrag incl. btw** hebt ingevoegd.</span><span class="sxs-lookup"><span data-stu-id="5e142-106">In case there is only one purchase line or in case all lines are subject to the same VAT %, the correct **Doc. Amount VAT Field** will be calculated automatically when you have inserted the purchase lines and the **Doc. Amount Incl. VAT Field**.</span></span> <span data-ttu-id="5e142-107">In het geval dat verschillende regels met verschillende btw-percentages bestaan, moet het veld **Documentbedrag incl. btw** handmatig worden gewijzigd.</span><span class="sxs-lookup"><span data-stu-id="5e142-107">In case several lines exist with different VAT percentages, the **Doc. Amount VAT Field** must be changed manually.</span></span>  

 <span data-ttu-id="5e142-108">De totaalbedragen van het inkoopdocument worden standaard gecontroleerd, maar u kunt dit uitschakelen door het selectievakje **Totaalbedragen documenten controleren** in het venster **Inkoopinstellingen** uit te schakelen.</span><span class="sxs-lookup"><span data-stu-id="5e142-108">Default the program will check the purchase document total amounts, but you can switch it off by deselecting the **Check Doc. Total Amounts** check box in the **Purchases & Payables Setup** window.</span></span>  

 <span data-ttu-id="5e142-109">Als u wilt weten waarom er een verschil is tussen de totaalbedragen van het document en de totaalbedragen van de ingevoegde inkoopregels, hebt u de mogelijkheid om het totaalbedrag, het totale basisbedrag, het totale btw-bedrag en het totaalbedrag inclusief btw van de ingevoegde inkoopregels te laten berekenen en deze onder aan het inkoopfactuur- of inkoopcreditnotavenster weer te geven.</span><span class="sxs-lookup"><span data-stu-id="5e142-109">To determine the reason of the difference between the document total amounts and the total amounts of the inserted purchase lines, you have the possibility to let the program calculate the total amount, total base amount, total VAT amount and total amount including VAT of the inserted purchase lines and show them at the bottom of the purchase invoice or purchase credit memo window.</span></span>  

 <span data-ttu-id="5e142-110">Deze totaalbedragen worden standaard niet weergegeven, maar u kunt dit inschakelen door het selectievakje **Totale op inkoopfactuur/CR-nota weergeven** in te schakelen</span><span class="sxs-lookup"><span data-stu-id="5e142-110">Default the program will not show these total amounts, but you can switch it on by selecting the **Show Totals on Purch. Inv.-CM.**</span></span> <span data-ttu-id="5e142-111">in het venster **Inkoopinstellingen**.</span><span class="sxs-lookup"><span data-stu-id="5e142-111">check box in the **Purchases & Payables Setup** window.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="5e142-112">Als u dit veld activeert, moeten de totalen van alle inkoopfacturen en creditnota's worden herberekend.</span><span class="sxs-lookup"><span data-stu-id="5e142-112">If you activate this field, totals on all purchase invoices and credit memos must be recalculated.</span></span> <span data-ttu-id="5e142-113">Dit kan een tijdrovend proces zijn, afhankelijk van het aantal documenten dat moet worden herberekend.</span><span class="sxs-lookup"><span data-stu-id="5e142-113">This can be a time-consuming process depending on the number of documents that must be recalculated.</span></span> <span data-ttu-id="5e142-114">U kunt dit veld niet activeren als er inkoopfacturen en/of creditnota's zijn zonder inkoopregels of als u inkoopfacturen en/of inkoopcreditnota's hebt waarbij geen aantal is opgegeven op de regels.</span><span class="sxs-lookup"><span data-stu-id="5e142-114">You can not activate this field in case purchase invoices and/or credit memos exist without any purchase lines or in case you have purchase invoices and/or purchase credit memos with no quantity specified on the lines.</span></span>  

## <a name="see-also"></a><span data-ttu-id="5e142-115">Zie ook</span><span class="sxs-lookup"><span data-stu-id="5e142-115">See Also</span></span>  
 [<span data-ttu-id="5e142-116">Procedure: Validatie van inkoopbedragen instellen</span><span class="sxs-lookup"><span data-stu-id="5e142-116">How to: Set Up Validation of Purchase Amounts</span></span>](how-to-set-up-validation-of-purchase-amounts.md)

