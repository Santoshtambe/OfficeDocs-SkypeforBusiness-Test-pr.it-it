﻿---
title: 'Lync Server 2013: Rapporto Dettagli sessione peer-to-peer'
TOCTitle: Rapporto Dettagli sessione peer-to-peer
ms:assetid: 6be1d676-68f7-4a53-a72a-de73296c5571
ms:mtpsurl: https://technet.microsoft.com/it-it/library/Gg558659(v=OCS.15)
ms:contentKeyID: 49300888
ms.date: 08/24/2015
mtps_version: v=OCS.15
ms.translationtype: HT
---

# Rapporto Dettagli sessione peer-to-peer in Lync Server 2013

 

_**Ultima modifica dell'argomento:** 2015-03-09_

Nel rapporto Dettagli sessione peer-to-peer vengono fornite informazioni dettagliate sulle sessioni peer-to-peer. Ad esempio, se si seleziona una sessione di messaggistica istantanea, nel rapporto sarà indicato il numero di messaggi inviato da ciascuno dei due utenti della sessione.

## Accedere al Rapporto Dettagli sessione peer-to-peer

È possibile accedere al rapporto Dettagli sessione peer-to-peer da uno dei seguenti rapporti (ai quali è possibile accedere dalla pagina principale dei rapporti di monitoraggio):

  - Rapporto inventario telefoni IP

  - Rapporto attività utente

  - Rapporto controllo di ammissione di chiamata

  - Rapporto Elenco errori

Dal rapporto Dettagli sessione peer-to-peer è possibile accedere al [Rapporto di diagnostica in Lync Server 2013](lync-server-2013-diagnostic-report.md) facendo clic sulla metrica del rapporto di diagnostica (dettagli). Facendo clic su una delle seguenti due metriche, è inoltre possibile accedere al Rapporto errori principali:

  - Risposta

  - ID diagnostica

## Utilizzare al meglio il Rapporto Dettagli sessione peer-to-peer

Il Rapporto Dettagli sessione peer-to-peer include molte metriche, alcune delle quali potrebbero essere sconosciute agli amministratori di sistema. Spesso, tuttavia, è possibile visualizzare un tooltip contenente la descrizione della metrica, semplicemente passando il mouse sull'etichetta della metrica.

Tenere sempre presente che le metriche reali mostrate in un rapporto dipendono dal tipo di sessione peer-to-peer selezionato. Una sessione audio/video riporta un set di metriche diverso rispetto a quello di una sessione di messaggistica istantanea.

Passando il mouse sulle metriche Codice di risposta e ID diagnostica, è possibile ottenere una descrizione dei valori:

## Filtri

Nessuno. Non è possibile filtrare il rapporto Dettagli sessione peer-to-peer.

## Metriche di informazioni sulla sessione

Nella tabella seguente sono elencate le informazioni disponibili nel rapporto Dettagli sessione peer-to-peer per ogni sessione.

### Metriche di informazioni sulla sessione

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th>Nome</th>
<th>Descrizione</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><strong>FQDN pool</strong></p></td>
<td><p>Nome di dominio completo (FQDN) del pool di registrazione o server perimetrale interessato dalla sessione.</p></td>
</tr>
<tr class="even">
<td><p><strong>Ora invito</strong></p></td>
<td><p>Data e ora in cui è stato inviato in origine l'invito alla sessione.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Ora risposta</strong></p></td>
<td><p>Data e ora in cui è stata ricevuta l'informazione che l'invito è stato accettato.</p></td>
</tr>
<tr class="even">
<td><p><strong>Da utente</strong></p></td>
<td><p>Indirizzo SIP dell'utente che ha avviato la sessione.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Da agente utente</strong></p></td>
<td><p>Software utilizzato dall'endpoint dell'utente che ha avviato la sessione.</p></td>
</tr>
<tr class="even">
<td><p><strong>Da utente interno</strong></p></td>
<td><p>Indica se l'utente che ha avviato la sessione ha effettuato l'accesso alla rete interna.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Da utente integrato con telefono da tavolo</strong></p></td>
<td><p>Indica se l'endpoint utilizzato dall'utente che ha avviato la sessione è integrato con il telefono desktop dell'utente stesso.</p></td>
</tr>
<tr class="even">
<td><p><strong>Priorità sessione</strong></p></td>
<td><p>Priorità assegnata alla sessione. Le priorità valide sono: Sconosciuto, Non urgente, Normale, Urgente ed Emergenza.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Codice di risposta</strong></p></td>
<td><p>Codice di risposta SIP inviato per la sessione non riuscita.</p></td>
</tr>
<tr class="even">
<td><p><strong>Front End</strong></p></td>
<td><p>Nome del server Front End Server utilizzato nella conferenza.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Ora di acquisizione</strong></p></td>
<td><p>Data e ora in cui sono state registrate le informazioni sulla sessione.</p></td>
</tr>
<tr class="even">
<td><p><strong>Ora fine</strong></p></td>
<td><p>Data e ora di fine della sessione.</p></td>
</tr>
<tr class="odd">
<td><p><strong>A utente</strong></p></td>
<td><p>Indirizzo SIP dell'utente che è stato invitato nella sessione.</p></td>
</tr>
<tr class="even">
<td><p><strong>Ad agente utente</strong></p></td>
<td><p>Software utilizzato dall'endpoint dell'utente invitato alla sessione.</p></td>
</tr>
<tr class="odd">
<td><p><strong>A utente interno</strong></p></td>
<td><p>Indica se l'utente invitato alla sessione ha effettuato l'accesso alla rete interna.</p></td>
</tr>
<tr class="even">
<td><p><strong>A utente integrato con telefono da tavolo</strong></p></td>
<td><p>Indica se l'endpoint utilizzato dall'utente invitato alla sessione è integrato con il telefono desktop dell'utente stesso.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Sessione ripetuta</strong></p></td>
<td><p>Indica se la sessione è un tentativo di ripetizione di una sessione non riuscita in precedenza.</p></td>
</tr>
<tr class="even">
<td><p><strong>ID diagnostica</strong></p></td>
<td><p>Identificatore univoco, sotto forma di intestazione ms-diagnostics, allegato a un messaggio SIP che include spesso informazioni utili per la risoluzione degli errori. Posizionare il puntatore del mouse sull'ID per visualizzare informazioni aggiuntive sull'ID stesso.</p></td>
</tr>
</tbody>
</table>


## Metriche per le modalità

Nella tabella seguente sono elencate le informazioni disponibili nel rapporto Dettagli sessione peer-to-peer per ogni modalità di sessione.

### Metriche per le modalità

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th>Nome</th>
<th>Elemento utilizzabile per eseguire l'ordinamento?</th>
<th>Descrizione</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><strong>Modalità</strong></p></td>
<td><p>No</p></td>
<td><p>Modalità utilizzate nella sessione, ad esempio messaggistica istantanea o trasferimento di file.</p></td>
</tr>
<tr class="even">
<td><p><strong>Messaggi da utente</strong></p></td>
<td><p>No</p></td>
<td><p>Numero di messaggi inviati dall'utente che ha avviato la sessione.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Messaggi a utente</strong></p></td>
<td><p>No</p></td>
<td><p>Numero di messaggi inviati dall'utente invitato a partecipare alla sessione.</p></td>
</tr>
</tbody>
</table>


## Metriche per i rapporti di diagnostica

Nella tabella seguente sono elencate le informazioni disponibili nel rapporto Dettagli sessione peer-to-peer per ogni rapporto di diagnostica.

### Metriche per i rapporti di diagnostica

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th>Nome</th>
<th>Elemento utilizzabile per eseguire l'ordinamento?</th>
<th>Descrizione</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><strong>Dettagli</strong></p></td>
<td><p>No</p></td>
<td><p>Quando si fa clic su questo elemento, nel rapporto viene visualizzato il rapporto di diagnostica per la sessione.</p></td>
</tr>
<tr class="even">
<td><p><strong>Ora rapporto</strong></p></td>
<td><p>No</p></td>
<td><p>Data e ora di registrazione del rapporto.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Richiesta</strong></p></td>
<td><p>No</p></td>
<td><p>Tipo di richiesta SIP, ad esempio INVITE o BYE.</p></td>
</tr>
<tr class="even">
<td><p><strong>ID diagnostica</strong></p></td>
<td><p>No</p></td>
<td><p>Identificatore univoco (in forma di intestazione ms-diagnostics) associato a un messaggio SIP che spesso fornisce informazioni utili per la risoluzione dei problemi e degli errori.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Tipo di contenuto</strong></p></td>
<td><p>No</p></td>
<td><p>Tipo di contenuto multimediale utilizzato nella conferenza. Un tipo di contenuto comune, ad esempio, è Application/sdp. SDP (Session Description Protocol) è un protocollo Internet standard utilizzato per annunci di sessioni, inviti a sessioni e altre forme di avvio di sessioni multimediali.</p></td>
</tr>
<tr class="even">
<td><p><strong>Segnalato da</strong></p></td>
<td><p>No</p></td>
<td><p>Computer, ovvero client o server, che ha segnalato il problema.</p></td>
</tr>
</tbody>
</table>

