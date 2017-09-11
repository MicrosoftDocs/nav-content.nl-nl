---
title: 'Procedure: Klantbetalingen inschakelen via PayPal'
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: 15f30a03c3e7ccc865ef527a707794c2c6428b2f
ms.contentlocale: nl-nl
ms.lasthandoff: 09/11/2017

---

# <a name="how-to-enable-customer-payments-through-paypal"></a><span data-ttu-id="5139a-102">Procedure: Klantbetalingen inschakelen via PayPal#</span><span class="sxs-lookup"><span data-stu-id="5139a-102">How to: Enable Customer Payments Through PayPal#</span></span>
<span data-ttu-id="5139a-103">Als alternatief voor het innen van betalingen door middel van bankoverschrijving of creditcards kunt u klanten aanbieden met hun PayPal-rekening te betalen.</span><span class="sxs-lookup"><span data-stu-id="5139a-103">As an alternative to collecting payments through bank transfer or credit cards, you can offer your customers to pay you through their PayPal account.</span></span>

<span data-ttu-id="5139a-104">Wanneer een klant de PayPal-koppeling op een verkoopfactuur of een verkooporderdocument kiest, wordt de servicepagina van hun PayPal-rekening geopend waarin de betalingsdetails voor de verkoop worden weergegeven.</span><span class="sxs-lookup"><span data-stu-id="5139a-104">When a customer chooses the PayPal link on a sales invoice or sales order document, the service page for their PayPal account appears showing the payment details for the sale.</span></span> <span data-ttu-id="5139a-105">De klant kan de factuur vervolgens als elke andere PayPal-betaling betalen.</span><span class="sxs-lookup"><span data-stu-id="5139a-105">The customer can then pay the invoice as any other PayPal payment.</span></span>

<span data-ttu-id="5139a-106">Als u klantbetalingen via PayPal wilt inschakelen, moet u het volgende doen:</span><span class="sxs-lookup"><span data-stu-id="5139a-106">To enable customer payments through PayPal, you must do the following:</span></span>

1. <span data-ttu-id="5139a-107">Stel PayPal-betalingsstandaard als een betalingsservice in het venster **Betalingsservices** in.</span><span class="sxs-lookup"><span data-stu-id="5139a-107">Set up PayPal Payments Standard as a payment service in the **Payments Services** window.</span></span>
2. <span data-ttu-id="5139a-108">Selecteer PayPal-betalingsstandaard in het veld **Betalingsservice** in het desbetreffende verkoopdocument.</span><span class="sxs-lookup"><span data-stu-id="5139a-108">Select PayPal Payments Standard in the **Payment Service** field on the sales document in question.</span></span>

<span data-ttu-id="5139a-109">De PayPal-betalingsstandaardservice wordt geïnstalleerd als een extensie voor Dynamics NAV en kan worden ingeschakeld.</span><span class="sxs-lookup"><span data-stu-id="5139a-109">The PayPal Payments Standard service is installed as an extension to Dynamics NAV and ready to enabled.</span></span> <span data-ttu-id="5139a-110">Zie [Dynamics NAV aanpassen met extensies ](ui-extensions.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="5139a-110">For more information, see [Customizing Dynamics NAV Using Extensions ](ui-extensions.md).</span></span>

## <a name="to-enable-the-paypal-payments-standard-service"></a><span data-ttu-id="5139a-111">De PayPal-betalingsstandaardservice inschakelen</span><span class="sxs-lookup"><span data-stu-id="5139a-111">To enable the PayPal Payments Standard service</span></span>
1. <span data-ttu-id="5139a-112">Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, kies **Betalingsservices** en kies vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="5139a-112">In the top right corner, choose the **Search for Page or Report** icon, **Payment Services**, and then choose the related link.</span></span>  
2. <span data-ttu-id="5139a-113">Kies in het venster **Betalingsservices** de actie **Nieuw**.</span><span class="sxs-lookup"><span data-stu-id="5139a-113">In the **Payment Services** window, choose the **New** action.</span></span>
3. <span data-ttu-id="5139a-114">Selecteer **PayPal-standaard** en sluit vervolgens het venster.</span><span class="sxs-lookup"><span data-stu-id="5139a-114">Select **PayPal Standard**, and then close the window.</span></span>
4. <span data-ttu-id="5139a-115">Kies in het venster **Betalingsservices** de actie **Instellen**.</span><span class="sxs-lookup"><span data-stu-id="5139a-115">In the **Payment Services** window, choose the **Setup** action.</span></span>
5. <span data-ttu-id="5139a-116">Vul indien nodig de velden in.</span><span class="sxs-lookup"><span data-stu-id="5139a-116">Fill in the fields as necessary.</span></span> <span data-ttu-id="5139a-117">Kies een veld om een korte omschrijving van het veld of een koppeling naar meer informatie te lezen.</span><span class="sxs-lookup"><span data-stu-id="5139a-117">Choose a field to read a short description of the field or link to more information.</span></span>

    <span data-ttu-id="5139a-118">**Opmerking**: schakel het selectievakje **Altijd opnemen in documenten** in als de hyperlink voor de PayPal-betalingsservice altijd zichtbaar moet zijn in verkoopdocumenten waarin de betaling via PayPal wordt ingeschakeld.</span><span class="sxs-lookup"><span data-stu-id="5139a-118">**Note**: Select the **Always Include on Documents** check box if the hyperlink for the PayPal payment service should always be visible on sales documents where payment through PayPal is enabled.</span></span>

6. <span data-ttu-id="5139a-119">Sluit het venster.</span><span class="sxs-lookup"><span data-stu-id="5139a-119">Close the window.</span></span>

## <a name="to-select-paypal-payments-standard-on-a-sales-invoice"></a><span data-ttu-id="5139a-120">PayPal-betalingsstandaard op een verkoopfactuur selecteren</span><span class="sxs-lookup"><span data-stu-id="5139a-120">To select PayPal Payments Standard on a sales invoice</span></span>
1. <span data-ttu-id="5139a-121">Kies op de startpagina **Verkoopfacturen**.</span><span class="sxs-lookup"><span data-stu-id="5139a-121">On the Home page, choose **Sales Invoices**.</span></span>
2. <span data-ttu-id="5139a-122">Open de verkoopfactuur waarvoor u PayPal-betalingen u wilt inschakelen.</span><span class="sxs-lookup"><span data-stu-id="5139a-122">Open the sales invoice that you want to enable PayPal payments for.</span></span>
3. <span data-ttu-id="5139a-123">Kies in het veld **Betalingsservice** een PayPal-betalingsstandaard.</span><span class="sxs-lookup"><span data-stu-id="5139a-123">In the **Payment Service** field, choose PayPal Payments Standard.</span></span>

<span data-ttu-id="5139a-124">**Opmerking**: het veld **Betalingsservice** is alleen zichtbaar als de PayPal-betalingsstandaardservice wordt ingeschakeld.</span><span class="sxs-lookup"><span data-stu-id="5139a-124">**Note**: The **Payment Service** field is only visible if the PayPal Payments Standard service is enabled.</span></span>   

## <a name="see-also"></a><span data-ttu-id="5139a-125">Zie ook</span><span class="sxs-lookup"><span data-stu-id="5139a-125">See Also</span></span>  
[<span data-ttu-id="5139a-126">Verkopen instellen</span><span class="sxs-lookup"><span data-stu-id="5139a-126">Set Up Sales</span></span>](sales-setup-sales.md)  
[<span data-ttu-id="5139a-127">Verkoop beheren</span><span class="sxs-lookup"><span data-stu-id="5139a-127">Manage Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="5139a-128">Dynamics NAV aanpassen met extensies</span><span class="sxs-lookup"><span data-stu-id="5139a-128">Customizing Dynamics NAV Using Extensions</span></span>](ui-extensions.md)

