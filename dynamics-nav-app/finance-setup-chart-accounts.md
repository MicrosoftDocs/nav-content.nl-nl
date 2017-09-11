---
title: De rekeningschema's instellen of wijzigen
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: 2a2f1f2ec3ac5bdd935ec19c11d74e16bdee7686
ms.contentlocale: nl-nl
ms.lasthandoff: 09/11/2017

---

# <a name="set-up-or-change-the-chart-of-accounts"></a><span data-ttu-id="624d7-102">De rekeningschema's instellen of wijzigen</span><span class="sxs-lookup"><span data-stu-id="624d7-102">Set Up or Change the Chart of Accounts</span></span>
<span data-ttu-id="624d7-103">Het rekeningschema bevat de grootboekrekeningen die uw financiële gegevens bevatten.</span><span class="sxs-lookup"><span data-stu-id="624d7-103">The chart of accounts shows the ledger accounts that store your financial data.</span></span> <span data-ttu-id="624d7-104">Dynamics NAV bevat een standaardrekeningschema dat gereed is om uw bedrijf te ondersteunen.</span><span class="sxs-lookup"><span data-stu-id="624d7-104">Dynamics NAV includes a standard chart of accounts that is ready to support your business.</span></span>
<span data-ttu-id="624d7-105">Echter, kunt u de standaardrekeningen wijzigen en u kunt nieuwe rekeningen toevoegen.</span><span class="sxs-lookup"><span data-stu-id="624d7-105">However, you can change the default accounts, and you can add new accounts.</span></span>  

## <a name="adding-or-changing-accounts"></a><span data-ttu-id="624d7-106">Rekeningen toevoegen of wijzigen</span><span class="sxs-lookup"><span data-stu-id="624d7-106">Adding or Changing Accounts</span></span>
<span data-ttu-id="624d7-107">Vanuit het rekeningschema kunt u elke grootboekrekening openen en instellingen toevoegen of wijzigen.</span><span class="sxs-lookup"><span data-stu-id="624d7-107">From the chart of accounts, you can open each G/L account and add or change settings.</span></span>

<span data-ttu-id="624d7-108">**Opmerking**: u kunt een grootboekrekening verwijderen.</span><span class="sxs-lookup"><span data-stu-id="624d7-108">**Note**: You can delete a general ledger account.</span></span> <span data-ttu-id="624d7-109">Echter, voordat u deze verwijdert, moet het volgende waar zijn:</span><span class="sxs-lookup"><span data-stu-id="624d7-109">However, before you delete it, the following must be true:</span></span>  
- <span data-ttu-id="624d7-110">Het saldo op de rekening moet nul zijn.</span><span class="sxs-lookup"><span data-stu-id="624d7-110">The balance on the account must be zero.</span></span>  
- <span data-ttu-id="624d7-111">Het veld **Grootboekrek.-verwijdering toestaan voor** moet zijn ingesteld in het venster **Grootboekinstelling** en de rekening mag geen grootboekposten op of na die datum hebben.</span><span class="sxs-lookup"><span data-stu-id="624d7-111">The **Allow G/L Acc. Deletion Before** field must be set in the **General Ledger Setup** window, and the account must not have ledger entries on or after that date.</span></span>  
- <span data-ttu-id="624d7-112">Als het veld **Grootboekrek.-gebruik controleren** in het venster **Grootboekinstellingen** is geselecteerd, mag de rekening niet worden gebruikt in boekingsgroepen of boekingsinstellingen.</span><span class="sxs-lookup"><span data-stu-id="624d7-112">If the **Check G/L Account Usage** field in the **General Ledger Setup** window is selected, then the account must not be used in any posting groups or posting setup.</span></span>  

<span data-ttu-id="624d7-113">Dynamics NAV voorkomt dat u een grootboekrekening verwijdert die gegevens bevat die nodig zijn in het rekeningschema.</span><span class="sxs-lookup"><span data-stu-id="624d7-113">Dynamics NAV will prevent you from deleting a general ledger account that stores data that is needed in the chart of accounts.</span></span>  

##<a name="see-also"></a><span data-ttu-id="624d7-114">Zie ook</span><span class="sxs-lookup"><span data-stu-id="624d7-114">See Also</span></span>  
[<span data-ttu-id="624d7-115">Het grootboek en het rekeningschema</span><span class="sxs-lookup"><span data-stu-id="624d7-115">The General Ledger and the Chart of Accounts</span></span>](finance-setup-general-ledger.md)  
[<span data-ttu-id="624d7-116">Bankrekeningen beheren.</span><span class="sxs-lookup"><span data-stu-id="624d7-116">Manage Bank Accounts</span></span>](bank-manage-bank-accounts.md)  
[<span data-ttu-id="624d7-117">Dimensies</span><span class="sxs-lookup"><span data-stu-id="624d7-117">Dimensions</span></span>](finance-setup-dimensions.md)  
[<span data-ttu-id="624d7-118">Procedure: Met GIFI-codes werken in Canada</span><span class="sxs-lookup"><span data-stu-id="624d7-118">How to: Work With GIFI Codes in Canada</span></span>](ca-finance-setup-work-GiFI-codes.md)

