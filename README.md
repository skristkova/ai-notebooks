# ai-notebooks

Sbírka Jupyter notebooků z mých experimentů s AI a kvantovými výpočty. Notebooky jsou připravené pro Google Colab.

## Obsah

| Notebook | Téma | Otevřít |
|---|---|---|
| [QuantumComputing.ipynb](QuantumComputing.ipynb) | Úvod do kvantových obvodů v Qiskitu | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/skristkova/ai-notebooks/blob/main/QuantumComputing.ipynb) |
| [Testchatbot.ipynb](Testchatbot.ipynb) | Tři přístupy ke konverzačnímu chatbotu | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/skristkova/ai-notebooks/blob/main/Testchatbot.ipynb) |

## QuantumComputing.ipynb

Dvouqubitový obvod s Hadamardovou bránou na qubitu 0 (superpozice).

- simulace měření v `AerSimulator` (1024 shotů) a histogram výsledků
- simulace stavového vektoru (`method='statevector'`)
- vizualizace stavu na Blochově sféře (`plot_bloch_multivector`)

**Knihovny:** `qiskit`, `qiskit-aer`, `matplotlib`

## Testchatbot.ipynb

Porovnání přístupů k jednoduchému chatbotu v češtině:

1. **DialoGPT-small + Gradio** – generativní model z Hugging Face s chatovacím rozhraním přímo v notebooku.
2. **DialoGPT-small s 8-bit kvantizací** – nižší paměťová náročnost díky `bitsandbytes` (vyžaduje GPU runtime).
3. **Stromový (rule-based) chatbot** – konverzační strom s volbou možností (počasí, nálada, koníčky, vtipy…). Neběží na žádném modelu, takže je stabilní a nenáročný na zdroje.

**Knihovny:** `transformers`, `torch`, `gradio`, `bitsandbytes`, `accelerate`

## Spuštění

1. Otevři notebook v Colabu přes odznak výše.
2. Spusť buňky postupně shora dolů. Potřebné balíčky se nainstalují v první buňce.
3. Stromový chatbot čte vstup přes `input()`. Odpovídá se číslem možnosti, konverzaci ukončíš slovem `konec`.

## Autorka

Simona ([skristkova](https://github.com/skristkova)) – System Automation & AI Specialist
