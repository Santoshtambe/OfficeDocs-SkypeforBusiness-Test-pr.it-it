﻿---
title: 'Lync Server 2013: Requisiti dei certificati per i dispositivi mobili'
TOCTitle: Requisiti dei certificati per i dispositivi mobili
ms:assetid: bb0e97af-cf60-4271-a0ab-654429d884ea
ms:mtpsurl: https://technet.microsoft.com/it-it/library/Hh690044(v=OCS.15)
ms:contentKeyID: 49301792
ms.date: 08/24/2015
mtps_version: v=OCS.15
ms.translationtype: HT
---

# Requisiti dei certificati per i dispositivi mobili in Lync Server 2013

 

_**Ultima modifica dell'argomento:** 2015-03-09_

Se si distribuisce la funzionalità di mobilità e si supporta l'individuazione automatica per i client mobili, è necessario includere determinate voci di nomi alternativi soggetto nei certificati per supportare le connessioni sicure dai client mobili.

È necessario includere voci di nomi alternativi soggetto per l'individuazione automatica nei certificati seguenti:

  - pool di server Director

  - pool Front End

  - Proxy inverso

In questa sezione vengono descritte le voci di nomi alternativi soggetto richieste nei certificati per l'individuazione automatica.


> [!NOTE]
> La riemissione di certificati tramite un'autorità di certificazione interna è in genere un processo semplice, ma l'aggiunta di più voci di nomi alternativi soggetto ai certificati pubblici utilizzati dal proxy inverso può essere un compito oneroso. Se esistono molti domini SIP, nel qual caso l'aggiunta di nomi alternativi soggetto è particolarmente onerosa, è possibile configurare il proxy inverso per l'utilizzo di HTTP per la richiesta iniziale del servizio di individuazione automatica, anziché HTTPS come da configurazione predefinita. Per informazioni dettagliate, vedere <A href="lync-server-2013-technical-requirements-for-mobility.md">Requisiti tecnici per i dispositivi mobili in Lync Server 2013</A>.



### Requisiti relativi ai certificati per il pool di Director

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th>Descrizione</th>
<th>Voce nome alternativo soggetto</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>URL servizio di individuazione automatica interno</p></td>
<td><p>SAN=lyncdiscoverinternal.&lt;dominiosip&gt;</p></td>
</tr>
<tr class="even">
<td><p>URL servizio di individuazione automatica esterno</p></td>
<td><p>SAN=lyncdiscover.&lt;dominiosip&gt;</p></td>
</tr>
</tbody>
</table>



> [!NOTE]
> In alternativa, è possibile utilizzare SAN=*.&lt;dominiosip&gt;



### Requisiti relativi ai certificati per il pool Front End

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th>Descrizione</th>
<th>Voce nome alternativo soggetto</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>URL servizio di individuazione automatica interno</p></td>
<td><p>SAN=lyncdiscoverinternal.&lt;dominiosip&gt;</p></td>
</tr>
<tr class="even">
<td><p>URL servizio di individuazione automatica esterno</p></td>
<td><p>SAN=lyncdiscover.&lt;dominiosip&gt;</p></td>
</tr>
</tbody>
</table>



> [!NOTE]
> In alternativa, è possibile utilizzare SAN=*.&lt;dominiosip&gt;



### Requisiti relativi ai certificati del proxy inverso (CA pubblica)

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th>Descrizione</th>
<th>Voce nome alternativo soggetto</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>URL servizio di individuazione automatica esterno</p></td>
<td><p>SAN=lyncdiscover.&lt;dominiosip&gt;</p></td>
</tr>
</tbody>
</table>



> [!NOTE]
> Questo nome alternativo del soggetto viene assegnato al certificato assegnato al listener SSL nel proxy inverso.




> [!NOTE]
> Il listener del proxy inverso avrà nomi alternativi del soggetto per gli URL dei servizi Web esterni, ad esempio SAN=lyncwebextpool01.contoso.com e dirwebexternal.contoso.com se è stato distribuito il Server Director facoltativo.


