# Hey, I'm Ed

I'm a data scientist. Most of my work has been in fraud modeling and data
engineering, but outside work I like tennis, piano, photography, and messing
around with image and video models.

This is where I put side projects and tools I've made for recurring problems.
Some are small experiments; the ministry reader has grown into a fuller local app.

### [Ministry Search RAG](https://github.com/datdatasciguy/ministry-rag-lab)

I built a local reading and question-answering app for a collection that you
supply. It indexes book sections with source details in SQLite, combines FTS5
keyword search with optional Nomic text embeddings, and merges the rankings
with reciprocal rank fusion before a local Ollama model answers from retrieved
passages. I wanted the answer to lead back to the actual page, rather than just
sound convincing.

The interface lets you search or ask questions across ministry books, Bible
verses, and footnotes, with book and author filters when that metadata is
verified. Numbered citations open source cards with more surrounding text. I
added checks for citation numbers and quotations, a way to say when the evidence
doesn't directly answer a question, and a separate opt-in area for extrapolation.
Longer questions can use a checkpointed deep-research flow. There is also song
and hymn search with local model review of whole-song meaning, plus
[desktop installer previews](https://github.com/datdatasciguy/ministry-rag-lab/releases).

This is retrieval and local-model integration, not a new LLM I trained. The
checks catch some clear mistakes but don't prove every sentence is supported.
The repo contains the app and [pipeline details](https://github.com/datdatasciguy/ministry-rag-lab/blob/main/docs/model_and_retrieval.md),
not the private books, lyrics, indexes, or model weights.

### [Tennis Match Lab](https://github.com/datdatasciguy/tennis-match-lab)

For comparing players and digging into matches. Right now it's serve and return
stats from charted matches. I'd like to get into playing styles and matchups
next. Basically, more numbers to bring into a tennis argument.

### [Photo Select Lab](https://github.com/datdatasciguy/photo-select-lab)

For sorting through similar photos without opening every file one at a time.
It groups likely duplicates and puts them in a contact sheet, with a few image
stats to help compare them.

I'm also working toward bringing over a local GUI I built with AI assistance
for face swaps and other image/video edits. The useful bits are picking clips,
previewing masks, comparing results, and keeping track of renders. That part
isn't in the repo yet.

### [Tools](https://github.com/datdatasciguy/tools)

An older collection of scripts I made to save time on data science chores.
`EDA_functions.py` covers single-variable and pairwise exploration, plots,
outlier flags, Cramér's V and correlation ratio, and statistical tests.
`optimizeCommand` uses YAML-defined Optuna trials to tune command-line
parameters, watch runtimes and errors, run local or SSH workers, and save
optimization plots. `kaggle.py` downloads and extracts datasets; `ruler.py`
marks column positions in fixed-width text. It's a shelf of standalone
utilities, not one end-to-end package.

### Piano, eventually

Finding the next piece to learn, cleaning up messy piece names, and trying out
some recommendations. Still in the ideas stage. Plenty of room to overthink
what to practice next.
