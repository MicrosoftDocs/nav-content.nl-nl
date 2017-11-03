---
title: Klantbetalingen via betalingsservices inschakelen
description: Maak het makkelijker voor klanten om facturen te betalen, door betalingsservices in te schakelen.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: online payment
ms.date: 07/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: f56df1759d375548b7415234c9b303a49e50687d
ms.contentlocale: nl-nl
ms.lasthandoff: 10/26/2017

---
# <a name="how-to-enable-customer-payments-through-payment-services"></a><span data-ttu-id="e2ddf-103">Procedure: Klantbetalingen via betalingsservices inschakelen</span><span class="sxs-lookup"><span data-stu-id="e2ddf-103">How to: Enable Customer Payments Through Payment Services</span></span>
<span data-ttu-id="e2ddf-104">Als alternatief voor het innen van betalingen door middel van bankoverschrijving of creditcards kunt u klanten laten betalen via hun account door middel van betalingsservices zoals PayPal en WorldPay.</span><span class="sxs-lookup"><span data-stu-id="e2ddf-104">As an alternative to collecting payments through bank transfer or credit cards, your customers can pay you through their account with payment services, such as PayPal and WorldPay.</span></span>  

<span data-ttu-id="e2ddf-105">Nadat u een betalingsservice hebt ingeschakeld in [!INCLUDE[d365fin](includes/d365fin_md.md)], wordt een koppeling naar de service beschikbaar op verkoopdocumenten die u per e-mail naar uw klanten verzendt.</span><span class="sxs-lookup"><span data-stu-id="e2ddf-105">After you enable a payment service in [!INCLUDE[d365fin](includes/d365fin_md.md)], a link to the service is available on sales documents that you send by email to your customers.</span></span> <span data-ttu-id="e2ddf-106">De klanten kunnen met de koppeling naar de betalingsservice gaan en de factuur betalen, rechtstreeks vanuit het verkoopdocument.</span><span class="sxs-lookup"><span data-stu-id="e2ddf-106">Customers can use the link to go to the payment service and pay the bill, directly from the sales document.</span></span> <span data-ttu-id="e2ddf-107">Als u de koppeling niet wilt opnemen, bijvoorbeeld wanneer een klant met contant geld betaalt, kunt u de betalingsservice uit de factuur verwijderen voordat u hem boekt.</span><span class="sxs-lookup"><span data-stu-id="e2ddf-107">If you don't want to include the link, for example, if a customer will pay with cash, you can remove the payment service from the invoice before posting.</span></span>  

<span data-ttu-id="e2ddf-108">De extensies PayPal Payments Standard en WorldPay Payments Standard zijn geïnstalleerd in [!INCLUDE[d365fin](includes/d365fin_md.md)] en u hoeft ze alleen maar in te schakelen.</span><span class="sxs-lookup"><span data-stu-id="e2ddf-108">The PayPal Payments Standard and WorldPay Payments Standard extensions are installed in [!INCLUDE[d365fin](includes/d365fin_md.md)], and are ready for you to enable.</span></span>  

## <a name="to-enable-a-payment-service-in-included365finincludesd365finmdmd"></a><span data-ttu-id="e2ddf-109">Een betalingsservice inschakelen in [!INCLUDE[d365fin](includes/d365fin_md.md)]</span><span class="sxs-lookup"><span data-stu-id="e2ddf-109">To enable a payment service in [!INCLUDE[d365fin](includes/d365fin_md.md)]</span></span>
1. <span data-ttu-id="e2ddf-110">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Betalingsservices** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="e2ddf-110">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Services**, and then choose the related link.</span></span>  
2. <span data-ttu-id="e2ddf-111">Kies in het venster **Betalingsservices** de actie **Nieuw**.</span><span class="sxs-lookup"><span data-stu-id="e2ddf-111">In the **Payment Services** window, choose the **New** action.</span></span>  
3. <span data-ttu-id="e2ddf-112">Selecteer de betalingsservice en sluit vervolgens het venster.</span><span class="sxs-lookup"><span data-stu-id="e2ddf-112">Select the payment service, and then close the window.</span></span>  
4. <span data-ttu-id="e2ddf-113">Kies in het venster **Betalingsservices** de actie **Instellen**.</span><span class="sxs-lookup"><span data-stu-id="e2ddf-113">In the **Payment Services** window, choose the **Setup** action.</span></span>  
5. <span data-ttu-id="e2ddf-114">Vul indien nodig de velden in.</span><span class="sxs-lookup"><span data-stu-id="e2ddf-114">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
6. <span data-ttu-id="e2ddf-115">Sluit het venster.</span><span class="sxs-lookup"><span data-stu-id="e2ddf-115">Close the window.</span></span>  

## <a name="to-select-a-payment-service-on-a-sales-invoice"></a><span data-ttu-id="e2ddf-116">Een betalingsservice selecteren op een verkoopfactuur</span><span class="sxs-lookup"><span data-stu-id="e2ddf-116">To select a payment service on a sales invoice</span></span>
1. <span data-ttu-id="e2ddf-117">Kies op de startpagina **Verkoopfacturen**.</span><span class="sxs-lookup"><span data-stu-id="e2ddf-117">On the Home page, choose **Sales Invoices**.</span></span>  
2. <span data-ttu-id="e2ddf-118">Open de verkoopfactuur die u wilt betalen door middel van de betalingsservice.</span><span class="sxs-lookup"><span data-stu-id="e2ddf-118">Open the sales invoice that you want to pay by using the payment service.</span></span>  
3. <span data-ttu-id="e2ddf-119">Kies in het veld **Betalingsservice** de gewenste betalingsservice.</span><span class="sxs-lookup"><span data-stu-id="e2ddf-119">In the **Payment Service** field, choose the payment service.</span></span>  

    > [!NOTE]  
>   <span data-ttu-id="e2ddf-120">Het veld **Betalingsservice** is alleen beschikbaar als u betalingsservices hebt ingeschakeld.</span><span class="sxs-lookup"><span data-stu-id="e2ddf-120">The **Payment Service** field is available only if you've enabled the payment service.</span></span>  

## <a name="see-also"></a><span data-ttu-id="e2ddf-121">Zie ook</span><span class="sxs-lookup"><span data-stu-id="e2ddf-121">See Also</span></span>  
[<span data-ttu-id="e2ddf-122">Verkopen instellen</span><span class="sxs-lookup"><span data-stu-id="e2ddf-122">Setting Up Sales</span></span>](sales-setup-sales.md)  
[<span data-ttu-id="e2ddf-123">Verkoop</span><span class="sxs-lookup"><span data-stu-id="e2ddf-123">Sales</span></span>](sales-manage-sales.md)  
<span data-ttu-id="e2ddf-124">[[!INCLUDE[d365fin](includes/d365fin_md.md)] aanpassen met behulp van extensies](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="e2ddf-124">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span></span>  
<span data-ttu-id="e2ddf-125">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="e2ddf-125">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

