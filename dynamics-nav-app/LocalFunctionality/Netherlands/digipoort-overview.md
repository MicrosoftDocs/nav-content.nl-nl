---
title: Overzicht van Digipoort
description: In Nederland gebruikt u Digipoort om periodieke elektronische aangiften te maken voor btw-aangiften en ICP-rapporten in EU-verkooplijstverzendingen. Digipoort is het elektronische postkantoor dat door de Nederlandse overheid voor bedrijven wordt geboden. Het bevat de gemeenschappelijke infrastructuur voor de communicatie van gegevens tussen bedrijven en de overheid, inclusief btw-aangiftes. De rapporten hebben de XBRL-indeling.
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
ms.openlocfilehash: 671933c4d4a9404a5d9198f501a871ac8ec4893a
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="digipoort-overview"></a><span data-ttu-id="7b356-106">Overzicht van Digipoort</span><span class="sxs-lookup"><span data-stu-id="7b356-106">Digipoort Overview</span></span>
<span data-ttu-id="7b356-107">In Nederland gebruikt u Digipoort om periodieke elektronische aangiften te maken voor btw-aangiften en ICP-rapporten in EU-verkooplijstverzendingen.</span><span class="sxs-lookup"><span data-stu-id="7b356-107">In the Netherlands, you use Digipoort to make periodic electronic filings for VAT declarations and ICP reports in EU sales list submissions.</span></span> <span data-ttu-id="7b356-108">Digipoort is het elektronische postkantoor dat door de Nederlandse overheid voor bedrijven wordt geboden.</span><span class="sxs-lookup"><span data-stu-id="7b356-108">Digipoort is the electronic post office provided by the Dutch government for companies.</span></span> <span data-ttu-id="7b356-109">Het bevat de gemeenschappelijke infrastructuur voor de communicatie van gegevens tussen bedrijven en de overheid, inclusief btw-aangiftes.</span><span class="sxs-lookup"><span data-stu-id="7b356-109">It provides the common infrastructure for the communication of information between companies and the government, including VAT declarations.</span></span> <span data-ttu-id="7b356-110">De rapporten hebben de XBRL-indeling.</span><span class="sxs-lookup"><span data-stu-id="7b356-110">The reports are in XBRL format.</span></span>  
  
 <span data-ttu-id="7b356-111">Het installatieprogramma van [!INCLUDE[navnow](../../includes/navnow_md.md)] installeert de .dll op de volgende locatie: c:Program Files (x86)Microsoft Dynamics NAV<version>RoleTailored ClientAdd-insMicrosoft.Dynamics.NL.Digipoortservice.dll.</span><span class="sxs-lookup"><span data-stu-id="7b356-111">[!INCLUDE[navnow](../../includes/navnow_md.md)] installer installs the .dll to the following location: c:Program Files (x86)Microsoft Dynamics NAV<version>RoleTailored ClientAdd-insMicrosoft.Dynamics.NL.Digipoortservice.dll.</span></span>  
  
 <span data-ttu-id="7b356-112">Het Digipoort-kanaal vervangt de BAPI-methode voor het doen van verzendingen.</span><span class="sxs-lookup"><span data-stu-id="7b356-112">The Digipoort channel replaces the BAPI method for making submissions.</span></span>  
  
## <a name="certificate-storage"></a><span data-ttu-id="7b356-113">Certificaatopslag</span><span class="sxs-lookup"><span data-stu-id="7b356-113">Certificate Storage</span></span>  
 <span data-ttu-id="7b356-114">Als u via Digipoort elektronisch wilt communiceren met de Nederlandse overheid, hebt u twee certificaten nodig (PKIoverheid).</span><span class="sxs-lookup"><span data-stu-id="7b356-114">In order to communicate electronically using Digipoort with the Dutch government, you will need two certificates (PKIoverheid).</span></span> <span data-ttu-id="7b356-115">U hebt een privécertificaat voor het bedrijf nodig en een openbaar certificaat van de website van de Nederlandse belastingdienst.</span><span class="sxs-lookup"><span data-stu-id="7b356-115">You will need a private certificate for the company as well as a public certificate from the website of the Dutch tax authorities.</span></span> <span data-ttu-id="7b356-116">een privécertificaat voor het bedrijf nodig en een openbaar certificaat van de website van de Nederlandse autoriteiten.</span><span class="sxs-lookup"><span data-stu-id="7b356-116">need a private certificate for the company as well as a public certificate from the Dutch authorities.</span></span> <span data-ttu-id="7b356-117">U kunt meer specifieke informatie van de website van de Nederlandse belastingdienst krijgen.</span><span class="sxs-lookup"><span data-stu-id="7b356-117">You can get more specific information from the website of the Dutch tax authority.</span></span> <span data-ttu-id="7b356-118">Zie voor meer informatie de website van de Nederlandse belastingdienst[Logius](https://aansluiten.procesinfrastructuur.nl/site/en/).</span><span class="sxs-lookup"><span data-stu-id="7b356-118">For more information, see the Dutch Tax Administration website[Logius](https://aansluiten.procesinfrastructuur.nl/site/en/).</span></span>  
  
 <span data-ttu-id="7b356-119">U moet de certificaten importeren die u in het certificaatarchief van Windows hebt ontvangen.</span><span class="sxs-lookup"><span data-stu-id="7b356-119">You will have to import the certificates that you receive into the Windows Certificate store.</span></span> <span data-ttu-id="7b356-120">Dit is een wijziging van eerdere versies, waarin u certificaten in [!INCLUDE[navnow](../../includes/navnow_md.md)] ontving.</span><span class="sxs-lookup"><span data-stu-id="7b356-120">This is a change from prior releases, in which you stored your certificates in [!INCLUDE[navnow](../../includes/navnow_md.md)].</span></span>  
  
 <span data-ttu-id="7b356-121">Zie voor meer informatie [Procedure: Certificaten instellen voor gebruik met Digipoort](how-to-set-up-certificates-for-use-with-digipoort.md).</span><span class="sxs-lookup"><span data-stu-id="7b356-121">For more information, see [How to: Set Up Certificates for use with Digipoort](how-to-set-up-certificates-for-use-with-digipoort.md).</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="7b356-122">Zie ook</span><span class="sxs-lookup"><span data-stu-id="7b356-122">See Also</span></span>  
 [<span data-ttu-id="7b356-123">Procedure: Certificaten instellen voor gebruik met Digipoort</span><span class="sxs-lookup"><span data-stu-id="7b356-123">How to: Set Up Certificates for use with Digipoort</span></span>](how-to-set-up-certificates-for-use-with-digipoort.md)
