---
title: Dynamics NAV aanpassen met extensies
author: edupont04
ms.custom: na
ms.date: 09/23/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: cc832772a255c7c801a7b956c74da827caca3765
ms.contentlocale: nl-nl
ms.lasthandoff: 09/11/2017

---

# <a name="customizing-dynamics-nav-using-extensions"></a><span data-ttu-id="2b64b-102">Dynamics NAV aanpassen met extensies</span><span class="sxs-lookup"><span data-stu-id="2b64b-102">Customizing Dynamics NAV Using Extensions</span></span>
<span data-ttu-id="2b64b-103">U kunt Dynamics NAV wijzigen door extensies te installeren die bijvoorbeeld functionaliteit toevoegen, gedrag wijzigen of u toegang verlenen tot nieuwe online services.</span><span class="sxs-lookup"><span data-stu-id="2b64b-103">You can change Dynamics NAV by installing extensions that add functionality, change behavior, or give you access to new online services, for example.</span></span>
<span data-ttu-id="2b64b-104">Wanneer u Dynamics NAV voor het eerst start, zijn bepaalde extensies al voor u geïnstalleerd.</span><span class="sxs-lookup"><span data-stu-id="2b64b-104">When you first launch Dynamics NAV, some extensions are already installed for you.</span></span> <span data-ttu-id="2b64b-105">In de loop van de tijd kunnen meer extensies beschikbaar voor u worden gemaakt en u kunt dan zelf bepalen of u de extensie wilt gebruiken of niet.</span><span class="sxs-lookup"><span data-stu-id="2b64b-105">Over time, more extensions can be made available to you, and you can then choose if you want to use the extension or not.</span></span>

<span data-ttu-id="2b64b-106">Zo verschaft Microsoft een extensie die integratie met PayPal Payments Standard biedt.</span><span class="sxs-lookup"><span data-stu-id="2b64b-106">For example, Microsoft provides an extension that provides integration with PayPal Payments Standard.</span></span> <span data-ttu-id="2b64b-107">Deze extensie is standaard geïnstalleerd.</span><span class="sxs-lookup"><span data-stu-id="2b64b-107">This extension is installed by default.</span></span>
<span data-ttu-id="2b64b-108">Maar als er een andere extensie beschikbaar komt die integratie met een andere betalingsservice biedt, kunt u de nieuwe extensie installeren en vervolgens bepalen welke van de services moeten worden gebruikt.</span><span class="sxs-lookup"><span data-stu-id="2b64b-108">But if another extension is made available that offers integration with another payment service, you can install the new extension and then choose which of the two services to use.</span></span>  

<span data-ttu-id="2b64b-109">U beheert de extensies in het venster **Extensiebeheer**.</span><span class="sxs-lookup"><span data-stu-id="2b64b-109">You manage the extensions in the **Extension Management** window.</span></span> <span data-ttu-id="2b64b-110">U kunt tot dit venster toegang krijgen via de startpagina.</span><span class="sxs-lookup"><span data-stu-id="2b64b-110">You can access this window from Home.</span></span> <span data-ttu-id="2b64b-111">U kunt ook in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport** kiezen, **Extensie** invoeren en vervolgens de gerelateerde koppeling kiezen.</span><span class="sxs-lookup"><span data-stu-id="2b64b-111">Alternatively, choose the **Search for Page or Report** icon in the top right corner, enter **Extension**, and then choose the related link.</span></span>   

## <a name="installing-an-extension"></a><span data-ttu-id="2b64b-112">Een extensie installeren</span><span class="sxs-lookup"><span data-stu-id="2b64b-112">Installing an Extension</span></span>
<span data-ttu-id="2b64b-113">Als nieuwe extensies beschikbaar voor u worden gemaakt omdat ze naar uw server zijn gepubliceerd, worden ze weergegeven in het venster **Extensiebeheer**.</span><span class="sxs-lookup"><span data-stu-id="2b64b-113">If new extensions are made available to you because they have been published to your server, they will be shown in the **Extension Management** window.</span></span> <span data-ttu-id="2b64b-114">Van hieruit kunt u extensies installeren en verwijderen.</span><span class="sxs-lookup"><span data-stu-id="2b64b-114">From here, you can choose to install and uninstall extensions.</span></span>  

<span data-ttu-id="2b64b-115">Als u een extensie kiest, kunt u lezen over wat de extensie doet en kunt u Help opvragen voor de extensie voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="2b64b-115">If you choose an extension, you can read about what the extension does, and you can access Help for the extension to learn more.</span></span> <span data-ttu-id="2b64b-116">Wanneer u een extensie wilt verkrijgen, moet u akkoord gaan met de gebruiksvoorwaarden.</span><span class="sxs-lookup"><span data-stu-id="2b64b-116">When you choose to get an extension, you must agree to the terms of use.</span></span>  

<span data-ttu-id="2b64b-117">Wanneer u een extensie installeert, moet u deze mogelijk instellen. Zo moet u wellicht een rekening opgeven met de extensie **PayPal Payments Standard voor Dynamics NAV**.</span><span class="sxs-lookup"><span data-stu-id="2b64b-117">When you install an extension, you might have to set it up, such as specifying an account for use with the **PayPal Payments Standard for Dynamics NAV** extension.</span></span>
<span data-ttu-id="2b64b-118">Met andere extensies worden gewoonweg velden aan een bestaande pagina toegevoegd of wordt bijvoorbeeld een nieuwe pagina toegevoegd.</span><span class="sxs-lookup"><span data-stu-id="2b64b-118">Other extensions simply add fields to an existing page, or they add a new page, for example.</span></span>   

<span data-ttu-id="2b64b-119">Als u een extensie verwijdert en vervolgens van gedachten verandert, kunt u deze opnieuw installeren.</span><span class="sxs-lookup"><span data-stu-id="2b64b-119">If you uninstall an extension, and you then change your mind, you can install it again.</span></span> <span data-ttu-id="2b64b-120">Wanneer u een extensie verwijdert die u gebruikt, worden de gegevens bewaard zodat deze gegevens nog steeds beschikbaar zijn als u de extensie opnieuw installeert.</span><span class="sxs-lookup"><span data-stu-id="2b64b-120">When you uninstall an extension that you have been using, the data is preserved so that if you install the extension again, your data is still available.</span></span>  

<span data-ttu-id="2b64b-121">Microsoft biedt de volgende extensies:</span><span class="sxs-lookup"><span data-stu-id="2b64b-121">Microsoft provides the following extensions:</span></span>  
- [<span data-ttu-id="2b64b-122">PayPal Payments Standard</span><span class="sxs-lookup"><span data-stu-id="2b64b-122">PayPal Payments Standard</span></span>](ui-extensions-paypal-payments-standard.md)  
- [<span data-ttu-id="2b64b-123">Verkoop- en voorraadprognose</span><span class="sxs-lookup"><span data-stu-id="2b64b-123">Sales and Inventory Forecast</span></span>](ui-extensions-sales-forecast.md)  

<span data-ttu-id="2b64b-124">Andere extensies zijn ook standaard beschikbaar, afhankelijk van uw land/regio.</span><span class="sxs-lookup"><span data-stu-id="2b64b-124">Other extensions are also available by default, depending on your country/region.</span></span>

## <a name="see-also"></a><span data-ttu-id="2b64b-125">Zie ook</span><span class="sxs-lookup"><span data-stu-id="2b64b-125">See Also</span></span>  
[<span data-ttu-id="2b64b-126">Procedure: Klantbetalingen inschakelen via PayPal</span><span class="sxs-lookup"><span data-stu-id="2b64b-126">How to: Enable Customer Payment Through PayPal</span></span>](sales-how-enable-customer-payments-paypal.md)  
[<span data-ttu-id="2b64b-127">Welkom bij Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="2b64b-127">Welcome to Dynamics NAV</span></span>](across-get-started.md)  

