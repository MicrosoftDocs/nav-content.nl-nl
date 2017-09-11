---
title: Nummerreeksen maken
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 22b3bcf71c99e106527d6bfa35478045d29b9629
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="create-number-series"></a><span data-ttu-id="38dbf-102">Nummerreeksen maken</span><span class="sxs-lookup"><span data-stu-id="38dbf-102">Create Number Series</span></span>

<span data-ttu-id="38dbf-103">Voor elk bedrijf dat u instelt, moet u unieke id-codes toewijzen aan zaken als grootboekrekeningen, klanten- en leveranciersrekeningen, facturen en documenten.</span><span class="sxs-lookup"><span data-stu-id="38dbf-103">For each company that you set up, you need to assign unique identification codes to things such as general ledger accounts, customer and vendor accounts, invoices, and documents.</span></span> <span data-ttu-id="38dbf-104">De nummering is niet alleen belangrijk voor identificatie.</span><span class="sxs-lookup"><span data-stu-id="38dbf-104">Numbering is important not only for identification.</span></span> <span data-ttu-id="38dbf-105">Met een goed opgezet nummeringssysteem kan het bedrijf ook beter worden beheerd en geanalyseerd en kan het aantal fouten tijdens gegevensinvoer worden beperkt.</span><span class="sxs-lookup"><span data-stu-id="38dbf-105">A well-designed numbering system also makes the company more manageable and easy to analyze, and can reduce the number of errors that occur in data entry.</span></span>

<span data-ttu-id="38dbf-106">U kunt een volledig nummeringssysteem instellen met een onbeperkt aantal reeksen.</span><span class="sxs-lookup"><span data-stu-id="38dbf-106">You can set up a complete numbering system with an unlimited number of number series.</span></span> <span data-ttu-id="38dbf-107">U kunt nummerreeksen gebruiken voor alle soorten documenten en dagboeken alsmede voor hoofdgegevens, zoals klanten, artikelen en verwerkingen.</span><span class="sxs-lookup"><span data-stu-id="38dbf-107">You can use number series for all types of documents and journals, as well as for master data such as customers, items, and jobs.</span></span>

<span data-ttu-id="38dbf-108">U kunt het gebruik van nummerreeksen combineren met handmatige nummering.</span><span class="sxs-lookup"><span data-stu-id="38dbf-108">You can combine the use of number series with manual numbering.</span></span>

<span data-ttu-id="38dbf-109">U maakt een nummeringssysteem door een of meer codes in te stellen voor elk soort hoofdgegevens of document.</span><span class="sxs-lookup"><span data-stu-id="38dbf-109">You create a numbering system by setting up one or more codes for each type of master data or document.</span></span> <span data-ttu-id="38dbf-110">U kunt bijvoorbeeld een code instellen voor het nummeren van klanten, een andere code voor het nummeren van verkoopfacturen en weer een andere code voor het nummeren van documenten in algemene dagboeken.</span><span class="sxs-lookup"><span data-stu-id="38dbf-110">For example, you can set up one code for numbering customers, another code for numbering sales invoices, and another code for numbering documents in general journals.</span></span>

<span data-ttu-id="38dbf-111">Nadat u een code hebt ingesteld, moet u minimaal één nummerreeksregel instellen.</span><span class="sxs-lookup"><span data-stu-id="38dbf-111">After you have set up a code, you set must set up at least one number series line.</span></span> <span data-ttu-id="38dbf-112">De nummerreeksregel bevat gegevens, zoals het eerste en laatste nummer in de reeks en de begindatum.</span><span class="sxs-lookup"><span data-stu-id="38dbf-112">The number series line contains information such as the first and last number in the series and the starting date.</span></span> <span data-ttu-id="38dbf-113">U kunt meer dan één nummerreeksregel per nummerreekscode invoeren, met een andere begindatum voor elke regel.</span><span class="sxs-lookup"><span data-stu-id="38dbf-113">You can set up more than one number series line per number series code, with a different starting date for each line.</span></span> <span data-ttu-id="38dbf-114">De reeks wordt opeenvolgend gebruikt, waarbij elke reeks wordt gestart op de betreffende begindatum.</span><span class="sxs-lookup"><span data-stu-id="38dbf-114">The series will be used consecutively, starting each series on the respective starting date.</span></span>

<span data-ttu-id="38dbf-115">Als u meer dan één nummerreekscode wilt gebruiken voor één soort hoofdgegevens (als u bijvoorbeeld verschillende nummerreeksen voor verschillende artikelcategorieën wilt gebruiken), kunt u relaties tussen nummerreeksen gebruiken.</span><span class="sxs-lookup"><span data-stu-id="38dbf-115">If you want to use more than one number series code for one type of master data - for example, if you want to use different number series for different categories of items - you can use number series relationships.</span></span>

<span data-ttu-id="38dbf-116">Naast de nummers die u handmatig of via het nummeringssysteem toewijst, worden aan alle transacties (posten) automatisch volgnummers toegewezen.</span><span class="sxs-lookup"><span data-stu-id="38dbf-116">In addition to the numbers that you assign manually or by use of the numbering system, all transactions (ledger entries) are automatically assigned consecutive numbers.</span></span> <span data-ttu-id="38dbf-117">Deze nummers vindt u in het veld **Postnr.**</span><span class="sxs-lookup"><span data-stu-id="38dbf-117">These numbers can be seen in the **Entry No.**</span></span> <span data-ttu-id="38dbf-118">in alle postvensters.</span><span class="sxs-lookup"><span data-stu-id="38dbf-118">field in all the ledger entry windows.</span></span> <span data-ttu-id="38dbf-119">U kunt deze nummers niet wijzigen of verwijderen.</span><span class="sxs-lookup"><span data-stu-id="38dbf-119">You cannot modify or delete these numbers.</span></span>

## <a name="to-create-relationships-between-number-series"></a><span data-ttu-id="38dbf-120">Relaties maken tussen nummerreeksen</span><span class="sxs-lookup"><span data-stu-id="38dbf-120">To create relationships between number series</span></span>
<span data-ttu-id="38dbf-121">Als u meerdere nummerreekscodes hebt ingesteld voor hetzelfde soort basisgegevens of transacties, kunt u relaties tussen de codes instellen.</span><span class="sxs-lookup"><span data-stu-id="38dbf-121">If you have set up more than one number series code for the same kind of basic information or transactions, you can create relationships between the codes.</span></span> <span data-ttu-id="38dbf-122">Met deze functie kunt u een code kiezen wanneer u een nummer gebruikt.</span><span class="sxs-lookup"><span data-stu-id="38dbf-122">This feature can assist you in deciding among the codes when you use a number.</span></span>

1. <span data-ttu-id="38dbf-123">Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Nr.-reeksen** in en kies vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="38dbf-123">In the top right corner, choose the **Search for Page or Report** icon, enter **No. Series**, and then choose the related link.</span></span>
2. <span data-ttu-id="38dbf-124">Selecteer de regel met de nummerreeks waarvoor u relaties wilt instellen en kies vervolgens **Relaties**.</span><span class="sxs-lookup"><span data-stu-id="38dbf-124">Select the line with the number series you want to create relationships for and then choose **Relationships**.</span></span>
3. <span data-ttu-id="38dbf-125">Geef in het veld **Reeks** de code op voor de nummerreeks die u wilt koppelen aan de reeks die u in stap 2 hebt geselecteerd.</span><span class="sxs-lookup"><span data-stu-id="38dbf-125">In the **Series Code** field, enter the code for the number series that you want to relate to the series you selected in step 2.</span></span>
4. <span data-ttu-id="38dbf-126">Voeg een regel toe voor elke code die u wilt koppelen aan de geselecteerde nummerreeksen.</span><span class="sxs-lookup"><span data-stu-id="38dbf-126">Add a line for each code that you want to relate to the selected number series.</span></span>
5. <span data-ttu-id="38dbf-127">Sluit het venster.</span><span class="sxs-lookup"><span data-stu-id="38dbf-127">Close the window.</span></span>

<span data-ttu-id="38dbf-128">Wanneer u nu iets instelt waarvoor u een nummer nodig hebt, kunt u de relaties gebruiken die u hebt ingesteld om te kiezen tussen de gekoppelde nummerreeksen.</span><span class="sxs-lookup"><span data-stu-id="38dbf-128">Now when you set up something that requires a number, you can use the relationships you created to select among the related number series.</span></span>

## <a name="see-also"></a><span data-ttu-id="38dbf-129">Zie ook</span><span class="sxs-lookup"><span data-stu-id="38dbf-129">See Also</span></span>
[<span data-ttu-id="38dbf-130">Werken met Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="38dbf-130">Work with Dynamics NAV</span></span>](ui-work-product.md)

