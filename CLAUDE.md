# Rassegna Stampa AI — Istruzioni per Claude

## Obiettivo
Ogni mattina produci una rassegna stampa completa sulle notizie AI delle ultime 24 ore.
Usa il web search per trovare fonti fresche e verificate. Includi sempre il link diretto all'articolo originale.

---

## Ricerca delle fonti

Cerca notizie nelle ultime 24 ore su queste fonti prioritarie:

**News e blog tecnici**
- The Verge (theverge.com)
- TechCrunch (techcrunch.com)
- Wired (wired.com)
- MIT Technology Review (technologyreview.com)
- VentureBeat (venturebeat.com)
- Ars Technica (arstechnica.com)

**Ricerca e modelli**
- Anthropic Blog (anthropic.com/news)
- OpenAI Blog (openai.com/news)
- Google DeepMind Blog (deepmind.google/discover/blog)
- Hugging Face Blog (huggingface.co/blog)
- arXiv AI section (arxiv.org/list/cs.AI/recent)

**SEO, Marketing e AI Search**
- Search Engine Journal (searchenginejournal.com)
- Search Engine Land (searchengineland.com)
- Search Engine Roundtable (seroundtable.com)
- Semrush Blog (semrush.com/blog)
- Barry Schwartz / RustyBrick feed

**Query di ricerca da usare**
- "AI news today"
- "artificial intelligence latest 24 hours"
- "LLM model release"
- "AI SEO search update today"
- "generative AI marketing"
- "AI regulation news"

---

## Struttura del file di output

Salva il file in: `output/YYYY-MM-DD.md`

Usa esattamente questa struttura:

```
# Rassegna Stampa AI — [DATA IN FORMATO GG MESE YYYY]

> Rassegna generata automaticamente. Fonti verificate nelle ultime 24 ore.
> **Notizie trovate:** XX | **Tempo di lettura stimato:** ~10 min

---

## 🤖 Modelli & Ricerca

### [Titolo notizia]
**Fonte:** [Nome Testata] | **Link:** [URL completo e cliccabile]

[2-4 righe di sintesi in italiano. Spiega cosa è successo, perché è rilevante, 
quale impatto può avere. Tono professionale e diretto.]

---

### [Titolo notizia]
...

---

## 🏢 Business & Enterprise AI

### [Titolo notizia]
**Fonte:** [Nome Testata] | **Link:** [URL completo e cliccabile]

[2-4 righe di sintesi]

---

## 🔍 AI per SEO & Marketing

### [Titolo notizia]
**Fonte:** [Nome Testata] | **Link:** [URL completo e cliccabile]

[2-4 righe di sintesi]

---

## ⚖️ Regolamentazione & Policy

### [Titolo notizia]
**Fonte:** [Nome Testata] | **Link:** [URL completo e cliccabile]

[2-4 righe di sintesi]

---

## 🌍 Altro & Segnalazioni

### [Titolo notizia]
**Fonte:** [Nome Testata] | **Link:** [URL completo e cliccabile]

[2-4 righe di sintesi]

---

*Generata il [DATA] alle [ORA]. Prossima rassegna domani alle 07:00.*
```

---

## Regole obbligatorie

1. **Minimo 15 notizie**, distribuite tra le categorie. Priorità a Modelli & Ricerca e AI per SEO & Marketing.
2. **Ogni notizia DEVE avere il link diretto** all'articolo originale — URL completo, non abbreviato.
3. **Non inventare notizie.** Se non trovi abbastanza contenuti recenti, riduci il numero e segnalalo nel file con una nota.
4. **Sintesi in italiano**, anche se la fonte è in inglese.
5. **Non duplicare** la stessa notizia in più categorie.
6. Se una notizia è particolarmente rilevante per il settore SEO/AI Search (es. aggiornamenti Google, AI Overviews, nuovi modelli di ricerca), mettila sempre in evidenza nella categoria **AI per SEO & Marketing**.
7. Verifica che i link siano reali e raggiungibili prima di includerli.

---

## Commit e push

Al termine, esegui sempre:

```bash
git add output/
git commit -m "rassegna: $(date +%Y-%m-%d)"
git push
```

---

## Nota sul contesto
Questa rassegna è pensata per un AI Engineer che lavora in un'agenzia digitale italiana focalizzata su e-commerce e SEO. Dai priorità a notizie con impatto pratico su: AI Search (Google SGE / AI Overviews), modelli LLM di nuova generazione, strumenti AI per marketing e contenuti, automazione e agenti AI in contesti business.
