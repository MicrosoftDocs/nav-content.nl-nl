---
title: Gebruikersactiviteit bijhouden in een wijzigingslogbestand
Description: U kunt een gebruikerslogboek activeren zodat u een historie hebt van eventuele wijzigingen in gegevens in getraceerde tabellen.
documentationcenter: 
author: edupont04
ms.prod: dynamics-nav-2017
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: user log, user activity, tracking
ms.date: 06/02/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 74d70c9929cfa29909281b964488319be7a9f127
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="logging-changes-in-dynamics-nav"></a><span data-ttu-id="aa718-103">Wijzigingen registreren in Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="aa718-103">Logging Changes in Dynamics NAV</span></span>
<span data-ttu-id="aa718-104">U kunt het wijzigingslogbestand in [!INCLUDE[d365fin](includes/d365fin_md.md)] inschakelen, zodat u een overzicht van activiteiten hebt.</span><span class="sxs-lookup"><span data-stu-id="aa718-104">You can enable the change log in [!INCLUDE[d365fin](includes/d365fin_md.md)] so you have a history of activities.</span></span> <span data-ttu-id="aa718-105">Het logboek is gebaseerd op wijzigingen die worden aangebracht in gegevens in de tabellen die u bijhoudt. In het wijzigingslogbestand worden posten chronologisch geordend en worden wijzigingen weergeven die worden aangebracht in de velden in de opgegeven tabellen.</span><span class="sxs-lookup"><span data-stu-id="aa718-105">The log is based on changes that are made to data in the tables that you track. In the change log, entries are chronologically ordered and show changes that are made to the fields on the specified tables.</span></span> <span data-ttu-id="aa718-106">In het wijzigingslogbestand verzamelt alle wijzigingen die in de tabel worden aangebracht.</span><span class="sxs-lookup"><span data-stu-id="aa718-106">The change log collects all changes that are made to the table.</span></span>  

## <a name="working-with-the-change-log"></a><span data-ttu-id="aa718-107">Werken met het wijzigingslogbestand</span><span class="sxs-lookup"><span data-stu-id="aa718-107">Working with the change log</span></span>
<span data-ttu-id="aa718-108">Een vaak voorkomend probleem in veel financiële systemen is het lokaliseren van de oorzaak van fouten en wijzigingen in gegevens.</span><span class="sxs-lookup"><span data-stu-id="aa718-108">A common problem in many financial systems is to locate the origin of errors and changes in data.</span></span> <span data-ttu-id="aa718-109">Het probleem kan variëren van een foutief telefoonnummer van een klant tot een foutieve boeking naar het grootboek.</span><span class="sxs-lookup"><span data-stu-id="aa718-109">It could be anything from an incorrect customer telephone number to an incorrect posting to the general ledger.</span></span> <span data-ttu-id="aa718-110">Met het wijzigingslogbestand kunt u alle directe wijzigingen bijhouden die een gebruiker aanbrengt in de databasegegevens.</span><span class="sxs-lookup"><span data-stu-id="aa718-110">The change log lets you track all direct modifications a user makes to data in the database.</span></span> <span data-ttu-id="aa718-111">U moet elke tabel en elk veld opgeven dat u door het systeem wilt laten registreren. Vervolgens moet u het wijzigingslogbestand instellen.</span><span class="sxs-lookup"><span data-stu-id="aa718-111">You must specify each table and field that you want the system to log, and then you must activate the change log.</span></span>  

<span data-ttu-id="aa718-112">U activeert en deactiveert het wijzigingslogbestand in het venster **Wijzigingslogbestandinstellingen**.</span><span class="sxs-lookup"><span data-stu-id="aa718-112">You activate and deactivate the change log in the **Change Log Setup** window.</span></span> <span data-ttu-id="aa718-113">Als u het wijzigingslogbestand activeert of deactiveert, wordt deze activiteit geregistreerd, zodat u altijd kunt zien welke gebruiker het wijzigingslogbestand heeft gedeactiveerd of opnieuw heeft geactiveerd.</span><span class="sxs-lookup"><span data-stu-id="aa718-113">When you activate or deactivate the change log, this activity is logged, so you can always see which user deactivated or reactivated the change log.</span></span> <span data-ttu-id="aa718-114">Dit kan niet worden uitgeschakeld.</span><span class="sxs-lookup"><span data-stu-id="aa718-114">This cannot be turned off.</span></span>  

<span data-ttu-id="aa718-115">In het venster **Wijzigingslogbestandinstellingen** kunt u als u de actie **Tabellen** kiest, opgeven voor welke tabellen u wijzigingen wilt bijhouden en welke wijzigingen moeten worden bijgehouden. [!INCLUDE[d365fin](includes/d365fin_md.md)] houdt ook een aantal systeemtabellen bij.</span><span class="sxs-lookup"><span data-stu-id="aa718-115">In the **Change Log Setup** window, if you choose the **Tables** action, you can specify which tables you want to track changes for, and which changes to track. [!INCLUDE[d365fin](includes/d365fin_md.md)] also tracks a number of system tables.</span></span>

<span data-ttu-id="aa718-116">Nadat u het wijzigingslogbestand hebt ingesteld, hebt geactiveerd en gegevens hebt gewijzigd, kunt u de wijzigingen weergeven en filteren in het venster **Wijzigingslogposten**.</span><span class="sxs-lookup"><span data-stu-id="aa718-116">After you have set up the change log, activated it, and made a change to data, you can view and filter the changes in the **Change Log Entries** window.</span></span> <span data-ttu-id="aa718-117">Als u posten wilt verwijderen, kunt u dat doen in het venster **Wijzigingslogposten verwijderen**, waar u filters kunt instellen op basis van datums en tijd.</span><span class="sxs-lookup"><span data-stu-id="aa718-117">If you want to delete entries, you can do that in the **Delete Change Log Entries** window, where you can set filters based on dates and time.</span></span>  

## <a name="see-also"></a><span data-ttu-id="aa718-118">Zie ook</span><span class="sxs-lookup"><span data-stu-id="aa718-118">See Also</span></span>
[<span data-ttu-id="aa718-119">Basisinstellingen wijzigen</span><span class="sxs-lookup"><span data-stu-id="aa718-119">Changing Basic Settings</span></span>](ui-change-basic-settings.md)  
[<span data-ttu-id="aa718-120">Sorteren</span><span class="sxs-lookup"><span data-stu-id="aa718-120">Sorting</span></span>](ui-sorting.md)  
[<span data-ttu-id="aa718-121">Zoeken naar pagina of rapport gebruiken</span><span class="sxs-lookup"><span data-stu-id="aa718-121">Using Search for Page or Report</span></span>](ui-search.md)  
<span data-ttu-id="aa718-122">[Procedure: Gebruikers en machtigingen beheren](ui-how-users-permissions.md)  </span><span class="sxs-lookup"><span data-stu-id="aa718-122">[How to: Manage Users and Permissions](ui-how-users-permissions.md)  </span></span>  
<span data-ttu-id="aa718-123">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="aa718-123">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

