---
title: Voorstellen maken
description: Voorstellen kunnen handmatig of automatisch worden gegenereerd op basis van leveranciers- of klantenposten.
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
ms.openlocfilehash: fe5374a9469b8d9c112e3bd99846e748d531b4c3
ms.contentlocale: nl-nl
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-create-proposals"></a>Procedure: Voorstellen maken
Voorstellen kunnen handmatig of automatisch worden gegenereerd op basis van leveranciers- of klantenposten.  

> [!IMPORTANT]  
>  Als u een voorstel maakt, moet u het veld **Rekeninghouder** in de vensters Bankrekening leverancier en Bankrekening klant gebruiken.  

> [!NOTE]  
>  U kunt op elk moment en op elk niveau, voorafgaand aan de verwerking van een voorstel, de transactiewijze en bankrekening wijzigen. Op het laagste niveau in de desbetreffende leveranciers- of klantenposten.  

## <a name="to-create-proposals-manually"></a>Handmatig voorstellen maken  

1.  Kies het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Telebankieren - bankoverzicht** in en kies de gerelateerde koppeling.  
2.  Selecteer de betreffende bankrekening en kies vervolgens de actie **Voorstel**.  
3.  U moet minimaal de velden **Rekeningsoort**, **Rekeningnr.**, **Transactiewijze**, **Bankrekeningnr.** en **Bedrag** invullen.  

4.  Als u de detailregels van het voorstel wilt bekijken of aanpassen, kiest u de actie **Detailinformatie**. Als u wilt terugkeren naar het voorstel, sluit u het venster **Voorsteldetailregel**.  

## <a name="to-create-proposals-automatically-from-sales"></a>Automatisch voorstellen maken op basis van verkoop  

1. Stel voor de klant die de factuur heeft verstuurd een kaart in met de juiste waarden voor de velden **Valutacode**, **Transactiewijze** en **Bankrekening**.  
2. Maak een verkoopfactuur of creditnota, vul de klant en relevante items in en boek de factuur.
3. Controleer of de velden **Valutacode**, **Transactiewijze** en **Bankrekening** van de factuur/creditnota de juiste waarden bevatten. Standaard worden deze gekopieerd vanuit de klantenkaart.  

4.  Kies het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Telebankieren - bankoverzicht** in en kies de gerelateerde koppeling.  
5.  Selecteer de betreffende bankrekening en kies vervolgens de actie **Voorstel**.  
6.  Kies de actie **Posten ophalen**.  

    U kunt de batchverwerking Voorstelposten ophalen gebruiken om voorstelregels te genereren op basis van relevante klantenposten.  

    > [!NOTE]  
    >  Alleen voor posten die een transactiewijze van het rekeningsoort **Klant** hebben en die aan de actieve bankrekening zijn gekoppeld, worden voorstelregels gemaakt.  

6.  Als u de detailregels van het voorstel wilt bekijken of aanpassen, kiest u de actie **Detailinformatie**. Als u wilt terugkeren naar het voorstel, sluit u het venster **Voorsteldetailregel**.  

## <a name="to-create-proposals-automatically-from-purchases"></a>Automatisch voorstellen maken op basis van inkoop  

1.  Stel voor de leverancier die de factuur heeft verstuurd een kaart in met de juiste waarden voor de velden **Valutacode**, **Transactiewijze** en **Bankrekening**.  
2.  Maak een inkoopfactuur of creditnota en voer de leverancier en relevante items in.
3. Boek de factuur.
4. Controleer of de velden **Valutacode**, **Transactiewijze** en **Bankrekening** van de factuur/creditnota de juiste waarden bevatten. Standaard worden deze gekopieerd vanuit de leverancierskaart.  
5.  Kies het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Telebankieren - bankoverzicht** in en kies de gerelateerde koppeling.  
6.  Selecteer de betreffende bankrekening en kies vervolgens de actie **Voorstel**.  
7.  Kies de actie **Posten ophalen**.  

    U kunt de batchverwerking Voorstelposten ophalen gebruiken om voorstelregels te genereren op basis van relevante leveranciersposten.  

    > [!NOTE]  
    >  Alleen voor posten die een transactiewijze van het rekeningsoort **Leverancier** hebben en die aan de actieve bankrekening zijn gekoppeld, worden voorstelregels gemaakt.  

6.  Als u de detailregels van het voorstel wilt bekijken of aanpassen, kiest u de actie **Detailinformatie**. Als u wilt terugkeren naar het voorstel, sluit u het venster **Voorsteldetailregel**.  

## <a name="see-also"></a>Zie ook  
 [Procedure: Nieuwe klanten registreren](../../sales-how-register-new-customers.md)   
 [Procedure: Verkoopbewerkingen](../../sales-how-invoice-sales.md)   
 [Procedure: Inkopen vastleggen](../../purchasing-how-record-purchases.md)   
 [Procedure: Betalingsrun maken en exporteren](how-to-create-and-export-payment-history.md)

