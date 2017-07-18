---
title: 'Procedure: Afschrijving van vaste activa instellen'
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 7efc50c673514498de0caa5b3a2dc4b32d4f7f5d
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-fixed-asset-depreciation"></a>Procedure: Afschrijving van vaste activa instellen
 U kunt diverse afschrijvingsmethoden gebruiken ter voorbereiding van financiële stukken en de aangifte van inkomstenbelasting. Veel grote ondernemingen gebruiken lineaire afschrijving voor hun jaarverslag omdat deze methode in het algemeen tot hogere netto-inkomsten leidt. Voor de inkomstenbelasting wordt vaker een versnelde afschrijvingsmethode gebruikt. Zie [Afschrijvingsmethoden](fa-depreciation-methods.md) voor meer informatie.

 Wanneer u de betreffende afschrijvingsboeken hebt ingesteld, moet u aan elk vast activum een of meer afschrijvingsboeken toewijzen. Naar een afschrijvingsboek dat aan een vast activum wordt toegewezen, wordt als een afschrijvingsboek voor vaste activa verwezen. Dienovereenkomstig wordt het venster voor toegewezen afschrijvingsboeken **Afschrijvingsboeken voor vaste activa** genoemd.

## <a name="to-create-a-depreciation-book"></a>Een afschrijvingsboek maken  
In een afschrijvingsboek voor vaste activa geeft u op hoe vaste activa worden afgeschreven. Het is mogelijk om meerdere afschrijvingsboeken in te stellen om diverse afschrijvingsmethoden toe te passen.  
1.  Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Afschrijvingsboeken** in en kies vervolgens de gerelateerde koppeling.
2. Kies in het venster **Lijst met afschrijvingsboeken** de actie **Nieuw**.
3. Vul in het venster **Afschrijvingsboek** indien nodig de velden in. Kies een veld om een korte omschrijving van het veld of een koppeling naar meer informatie te lezen.

    **Opmerking**: u kunt de transacties voor vaste activa registreren in het venster **Financieel dagboek voor vaste activa** of in het venster **Dagboek voor vaste activa**, afhankelijk van de vraag of de transacties zijn bedoeld voor financiële rapportage of intern beheer. Voer de volgende stap uit om te definiëren welk soort dagboek standaard wordt gebruikt voor de verschillende activiteiten voor vaste activa.
4. Schakel op het sneltabblad **Integratie** het selectievakje in voor elke activiteit voor vaste activa waarvan u transacties wilt boeken met het venster **Financieel dagboek voor vaste activa**.
5. Herhaal stap 2 t/m 4 voor elke afschrijvingsmethode of boekingsmethode die u aan vaste activa als afschrijvingsboek wilt toewijzen.

## <a name="to-assign-a-depreciation-book-to-a-fixed-asset"></a>Een afschrijvingsboek aan een vast activum toewijzen  
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Vaste activa** in en kies vervolgens de gerelateerde koppeling.
2. Selecteer het vaste activum waarvoor u een afschrijvingsboek voor vaste activa wilt instellen.
3. Vul op het sneltabblad **Afschrijvingsboek** indien nodig de velden in.
4. Als u meer dan één afschrijvingsboek aan het vaste activum moet toewijzen, kiest u de actie **Meer afschrijvingsboeken toevoegen**.
5. U kunt ook de actie **Afschrijvingsboeken** kiezen om een of meer afschrijvingsboeken voor vaste activa op te geven.

**Opmerking**: als u de handmatige afschrijvingsmethode gebruikt, moet u de afschrijving handmatig invullen in het financieel dagboek voor vaste activa. Uit de functie **Afschrijving berekenen** worden de vaste activa weggelaten die handmatig worden afgeschreven. U kunt deze methode gebruiken voor activa waarop niet wordt afgeschreven, zoals grond.

## <a name="to-assign-a-depreciation-book-to-multiple-fixed-assets-with-a-batch-job"></a>Een afschrijvingsboek aan meerdere vaste activa toewijzen met een batchverwerking
Als u een afschrijvingsboek wilt toewijzen aan meerdere vaste activa, kunt u de batchverwerking **Afschrijvingsboeken maken** gebruiken, zodat de benodigde afschrijvingsboeken voor vaste activa automatisch worden gemaakt in Dynamics NAV.  
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Vaste activa** in en kies vervolgens de gerelateerde koppeling.
2. Selecteer het vaste activum waaraan u een afschrijvingsboek wilt toewijzen en kies vervolgens de actie **Bewerken**.
3. In het venster **Afschrijvingsboek** kiest u de actie **VA-afschrijvingsboeken maken**.
4. In het venster **VA-afschrijvingsboeken maken** vult u het veld **Afschrijvingsboek** in.
5. Kies het veld **Kopiëren van VA-nr.** en selecteer vervolgens het nummer van het vaste activum dat u als basis wilt gebruiken voor het maken van nieuwe afschrijvingsboeken voor vaste activa.

    Als u dit veld invult, bevatten de afschrijvingsvelden in de nieuwe afschrijvingsboeken voor vaste activa dezelfde gegevens als de overeenkomstige velden in het afschrijvingsboek voor vaste activa waaruit u kopieert. Laat het veld leeg als u nieuwe VA-afschrijvingsboeken met lege afschrijvingsvelden wilt maken.  
6. Op het sneltabblad **Vast activum** kunt u met behulp van een filter aangeven voor welke activa u de afschrijvingsboeken voor vaste activa wilt maken.
7. Kies de knop **Ok**.

## <a name="to-set-up-depreciation-posting-types"></a>Boekingssoorten voor afschrijving instellen  
Voor elk afschrijvingsboek moet u instellen hoe diverse boekingssoorten in Dynamics NAV moeten worden verwerkt. Bijvoorbeeld, of de boeking debet of credit moet zijn, en of het boekingssoort moet worden opgenomen in de afschrijvingsbasis.  
1.  Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Afschrijvingsboeken** in en kies vervolgens de gerelateerde koppeling.  
2. Selecteer het afschrijvingsboek dat u wilt instellen en kies vervolgens de actie **VA-boekingssoortinstellingen**.
3. Vul indien nodig de velden in het venster **VA-boekingssoortinstellingen** in.

**OPMERKING**: in het venster **VA-boekingssoortinstellingen** kunt u geen regels wissen of invoegen. U kunt alleen de bestaande regels wijzigen.

Het wordt aangeraden om de instellingen van afschrijvingsboeken waarvoor al posten zijn geboekt niet te wijzigen. De wijzigingen gelden namelijk niet voor reeds geboekte posten, waardoor de statistische gegevens van het afschrijvingsboek onjuist worden.

## <a name="to-set-up-default-templates-and-batches-for-fixed-asset-depreciation"></a>Standaardsjablonen en batches instellen voor afschrijvingsboeken voor vaste activa  
Voor elk afschrijvingsboek definieert u een standaardinstelling van sjablonen en batches. U gebruikt deze standaardinstellingen in de volgende procedures:
- Regels dupliceren van het ene dagboek naar het andere.
- Maak dagboekregels met behulp van de batchverwerkingen **Afschrijving berekenen** of **Vast activum indexeren**.
- Aanschafkosten dupliceren in het verzekeringsdagboek.

1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Afschrijvingsboeken** in en kies vervolgens de gerelateerde koppeling.
2. Selecteer het afschrijvingsboek waarvoor u standaarddagboeken posten wilt definiëren en kies vervolgens de actie **VA-dagboekinstellingen**.
3. Als u voor elke gebruiker een standaardinstelling wilt gebruiken, kiest u het veld **Gebruikers-id** om een selectie te maken in het venster **Gebruikers**.
4. In de andere velden selecteert u de dagboeksjabloon of dagboekbatch die standaard moet worden gebruikt.

## <a name="see-also"></a>Zie ook
[Vaste activa instellen](fa-setup.md)  
[Vaste activa beheren](fa-manage.md)  
[Financiën](finance-setup.md)  
[Welkom bij Dynamics NAV](across-get-started.md)

