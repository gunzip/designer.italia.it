---
template: post.html
title: Dispositivi
published: true
---

I contenuti e le funzionalità di un sito o un servizio devono poter essere fruibili
su tutti i dispositivi più utilizzati dagli utenti.

<!-- <div class="lg-callout lg-callout-must">
<mark>SI DEVE</mark> -->

<div class="lg-callout lg-callout-should">
<mark>SI DOVREBBE</mark>
Analizzare regolarmente l'utilizzo dei dispositivi e delle diverse risoluzioni
che gli utenti adoperano per accedere al sito.
</div>

È necessario assicurare la compatibilità con almeno i seguenti browser:

- Internet Explorer 10+
- Edge 12+
- Safari 8+
- Google Chrome (ultime versioni)
- Opera (ultime versioni)
- Mozilla Firefox (ultime versioni)
- IE Mobile	10+
- iOS Safari 8+ (versione del sistema operativo)
- Android	Browser 4+ (versione del sistema operativo)

<!-- </div> -->

La lista comprende più del 95% delle versioni utilizzate in Italia (e nel mondo)
secondo i dati raccolti da [StatCounter](http://gs.statcounter.com/#browser-IT-monthly-201506-201606)

Non è necessario che l'aspetto del sito sia identico sui diversi dispositiv;
va tuttavia garantita un'esperienza utente equivalente.

<!-- Per versioni di Explorer inferiori alla 10 si consiglia un supporto
-- funzionale (contenuti accessibili) ma non necessariamente conforme
-- (l'esperienza utente può esser qualitativamente inferiore).
-->

### Garantire la compatibilità

Nel web design si sono adottati spesso gli approcci **graceful degradation** (decadimento parziale) o **progressive enhancement**
(miglioramento progressivo). Si tratta di due risposte diverse alla stessa esigenza: rendere il contenuto accessibile su dispositivi diversi. Nel primo approccio ci si fa carico di verificare che il progetto, inizialmente pensato per i dispositivi più completi, resti navigabile anche man mano che si usano tecnologie più obsolete o meno interattive. Nel secondo, si parte da un nucleo solido e irrinunciabile di contenuti che vengono arricchiti via via che il dispositivo diventa più potente e all'avanguardia.

 Tecnicamente il sito web può rilevare quale dispositivo lo sta navigando. È possibile capire:
 - lo **user agent**, ovvero quale browser e quale sistema operativo è in collegamento
 - la **risoluzione** dello schermo, ovvero quanti pixel abbiamo a disposizione
 - il **tipo di media**, ovvero se stiamo andando in stampa o su schermo

Tecniche apposite come l'uso di **media queries** permettono di dare istruzioni ai CSS per comportarsi in modo diverso a seconda della risoluzione (*breakpoint*). Individuato il dispositivo, la risoluzione e il browser utilizzato, il contenuto (il nucleo) viene arricchito o meno da informazioni e funzioni aggiuntive.

### Validazione dei fogli di stile CSS

Per compensare le incompatibilità dei diversi browser è spesso necessario introdurre nei fogli di stile
(<abbr title="Cascading Style Sheets">CSS</abbr>) codice non conforme
che non passa quindi i [controlli di validità del W3C](https://jigsaw.w3.org/css-validator/).

La validazione è importante laddove un errore pregiudica una funzionalità;
oggi i browser sono più "resilienti" e spesso non si verifica il caso.

Non è necessario pertanto che un CSS rispetti perfettamente gli standard.

D'altro canto, un CSS (o HTML) perfettamente validi non assicurano di per sé che [il sito sia accessibile](/linee-guida/accessibilita).