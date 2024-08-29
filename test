# Forgend: Workflow del Funzionamento (Playbook)

## Diagramma Interattivo del Workflow

<div id="workflow-diagram" style="width: 100%; height: 600px; border: 1px solid #ddd; position: relative;"></div>

<script src="https://cdnjs.cloudflare.com/ajax/libs/vis-network/9.1.2/vis-network.min.js"></script>

<script>
document.addEventListener('DOMContentLoaded', function() {
  const container = document.getElementById('workflow-diagram');

  const nodes = new vis.DataSet([
    { id: 1, label: 'Inserimento contenuti', shape: 'box' },
    { id: 2, label: 'Estrazione dei Contenuti', shape: 'box' },
    { id: 3, label: 'Elaborazione testo in SEO', shape: 'box' },
    { id: 4, label: 'Review o schedulazione dei Post', shape: 'box' },
    { id: 5, label: 'Pubblicazione Multicanale', shape: 'box' },
    { id: 6, label: 'Feed', shape: 'circle' },
    { id: 7, label: 'Trends', shape: 'circle' },
    { id: 8, label: 'Follow People', shape: 'circle' },
  ]);

  const edges = new vis.DataSet([
    { from: 1, to: 2, arrows: 'to' },
    { from: 2, to: 3, arrows: 'to' },
    { from: 3, to: 4, arrows: 'to' },
    { from: 4, to: 5, arrows: 'to' },
    { from: 1, to: 6, arrows: 'to' },
    { from: 1, to: 7, arrows: 'to' },
    { from: 1, to: 8, arrows: 'to' },
  ]);

  const data = {
    nodes: nodes,
    edges: edges
  };

  const options = {
    layout: {
      hierarchical: {
        direction: 'UD',
        sortMethod: 'directed'
      }
    },
    physics: false,
    interaction: {
      dragNodes: false,
      zoomView: false,
      dragView: false
    }
  };

  new vis.Network(container, data, options);
});
</script>

## Descrizione Dettagliata del Workflow

1. **Inserimento contenuti**
   - L'utente configura i propri target:
     - Feed
     - Trends
     - Follow people

2. **Estrazione dei Contenuti**
   - **Scelta della Fonte**:
     - **Se si sceglie Feed**:
       - `Parsing Feed`: Estrai contenuti da feed RSS e Atom.
       - `Trend Extraction`: Estrai i trend attuali da Google Trends.
       - `Web Scraping`: Estrai dati da fonti non standard.
   - Schedulazione manuale per ogni scansione dei feed

3. **Elaborazione testo in SEO**
   - `Rielaborazione dei Contenuti`: Rielabora i contenuti estratti secondo le linee guida SEO.
   - `Ottimizzazione Automatica`: Ottimizza meta tag, titoli, descrizioni, hashtag, e parole chiave.
   - `Analisi Semantica`: Analizza e inserisce naturalmente le parole chiave nei contenuti.
   - `Generazione Immagini`: Crea o modifica immagini correlate al contenuto.

4. **Review o schedulazione dei Post**
   - L'utente rivede i contenuti generati e può:
     - Approvare per la pubblicazione immediata
     - Schedulare per una pubblicazione futura
     - Modificare manualmente il contenuto

5. **Pubblicazione Multicanale**
   - `Integrazione con Piattaforme`: Integra con piattaforme social e CMS.
   - `Pianificazione Intelligente`: Pianifica la pubblicazione basata su analisi dell'engagement.
   - `Adattamento dei Contenuti`: Adatta automaticamente i contenuti per ciascuna piattaforma.
