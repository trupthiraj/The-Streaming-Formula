# 🎬 The Streaming Formula

> *900,000 movies walked so you could binge watch in peace. Here's what they taught us.*

---

## The Hook

We need to talk about the algorithm. Not because it's broken — but because it's suspiciously, unnervingly good at knowing you'd rather start a new series at 11pm than go to sleep like a functional adult. Every binge watch session starts the same way. One episode. Just one. And then somewhere between episode three and the moment you realise it's 2am and you've been emotionally compromised by a slow burn romance involving a single umbrella scene — you stop questioning it and just feel it.
But here's the thing nobody thinks to ask in that moment: someone built this. Someone made decisions about genres, budgets, release dates and languages that led directly to your sleep schedule becoming a suggestion rather than a commitment. Someone, somewhere, made a very expensive spreadsheet. This project went looking for that spreadsheet — in 900,000 movies, with real budget and revenue data, and absolutely no regrets about the rabbit hole it opened.

---

## What Makes This Different

Every streaming analysis out there does the same three things: counts titles per platform, averages IMDb ratings, draws a genre pie chart. That's the entire ceiling of what's published.

This project asks different questions:

- Which genres consistently make money AND get good reviews — and which ones just pick one?
- Does Hollywood actually know when to release its best work — and is January really the graveyard everyone says it is?
- Does spending more money make better, more profitable movies — or is that just what the marketing budget wants you to believe?
- Have movies actually gotten better over the decades — or does it just feel that way?
- Is non-English content genuinely outperforming English on quality metrics — and what does that mean for every platform currently betting billions on Korean drama?

---

## Key Findings

1. **Documentary is the only genre in the top right quadrant** — high ROI AND high ratings simultaneously. It's cheap to make, critically respected, and finds a passionate audience every time. Every platform needs more of it. Most of them don't make enough of it.

2. **Horror has terrible ratings and genuinely decent ROI.** It's the fast fashion of cinema — cheap, reliably consumed, critically ignored, commercially dependable. The data confirms what every horror fan already knows: the audience shows up regardless.

3. **The release calendar is a confession.** January has the lowest average revenue AND the lowest average rating of any month. December has the highest of both simultaneously — the only month where commercial ambition and genuine quality align. If you want to know how much a studio believes in a film, don't read the press release. Check the release date.

4. **Bigger budgets buy bigger audiences, not better movies.** The trend line between budget and rating is essentially flat. The trend line between budget and ROI slopes downward. The highest returns come from low and mid budget films. The blockbuster model works when it works — the data says it works less reliably than the $200 million marketing campaigns suggest.

5. **The 2000s were the worst decade for movie quality in this dataset.** As content volume exploded, rating distributions shifted left. The 2020s median is quietly creeping back up. Whether that's streaming quality wars producing results or bad 2020s films not yet having accumulated their deserved ratings is a question worth revisiting in 2030.

6. **Korean content outperforms English by nearly half a rating point.** Japanese, Chinese, Hindi and Russian content all beat the English average too. Netflix didn't just open new markets when it went global — it accidentally discovered that the best storytelling wasn't exclusively coming from Hollywood. The audience watching with subtitles at 3am already knew. The data just confirmed it.

---

## What A Streaming Platform Should Do With This

**Content acquisition teams** should be tracking genre ROI quartiles, not just critical reception. Documentary and Horror sit at opposite ends of the rating spectrum and both consistently return on investment. Two very different bets. Both worth making.

**Release strategy teams** should be treating December like the premium real estate it demonstrably is, and January like the liability it's proven to be every single year without exception.

**International content teams** should be using rating performance by language as a commissioning signal, not just a market access strategy. Korean, Japanese and Chinese content consistently outperforms English on quality metrics. Commissioning more of it isn't cultural goodwill. It's data-driven programming.

**Finance teams** should be deeply sceptical of any pitch that justifies a $200M+ budget primarily on the basis that bigger equals better. The scatter plot disagrees. With 6,464 data points behind it.

---

## Project Structure
```
the-streaming-formula/
│
├── 01_streaming_formula_analysis.ipynb  ← Full analysis notebook
├── TheStreamingFormula.html             ← Standalone HTML export
│
├── chart1_genre_profitability.png       ← Genre ROI vs rating bubble chart
├── chart2_release_window.png           ← Revenue and rating by month
├── chart3_budget_scatter.png           ← Budget vs rating and ROI scatter
├── chart4_genre_trends_animated.png    ← Genre trends by decade (animated)
├── chart5_rating_ridge.png             ← Rating distributions by decade
└── chart6_language_analysis.png        ← Non-English vs English performance
```

---

## Tech Stack

| Tool | Purpose |
|------|---------|
| Python | Core analysis |
| pandas | Data manipulation and cleaning |
| Plotly | Interactive and animated charts |
| Seaborn + Matplotlib | Statistical visualisation |
| scikit-learn | Data preprocessing |
| scipy | KDE for ridge plots |
| Jupyter Notebook | Development environment |

---

## Data Source

**TMDB Movies Dataset 2024** — 900,000+ movies with budget, revenue, popularity, ratings, genres, release dates and production metadata. Updated daily.

🔗 [Dataset on Kaggle](https://www.kaggle.com/datasets/asaniczka/tmdb-movies-dataset-2023-930k-movies)

---

## What I Learned

The most important decision in this project wasn't analytical — it was about filtering. Starting with 1.4 million entries and ending with 16,762 felt like throwing away data. It wasn't. The 94% of entries with zero budget data and the entries with zero votes aren't movies that failed — they're entries that were never really movies in the first place, at least not in any meaningful commercial or cultural sense. Keeping them would have made every finding statistically meaningless.

The budget vs ROI finding genuinely surprised me. I expected a positive relationship — spend more, make more. The downward trend line was not what I predicted going in. It took three different ways of looking at the same data before I trusted it enough to write it up. That process — predicting, being wrong, investigating why, updating — is the part of analysis that doesn't show up in the charts but is the whole point of doing it.

The language finding was the most culturally satisfying. Korean content beating English by half a rating point isn't a statistical quirk. It's the data catching up to something anyone who has watched three episodes of a Korean drama in a row already understood intuitively. Sometimes the numbers just confirm what the audience already knows.

Finally: animated charts are worth the extra effort. The decade-by-decade genre animation in Chart 4 takes thirty seconds to watch and communicates something that would take three static charts and two paragraphs to explain. When the chart does the work, let it.

---

## About

Built by **Trupthi Raj** — data analyst with a focus on retail, luxury, entertainment and travel.

📁 [GitHub](https://github.com/trupthiraj)
📊 [Tableau Public](https://public.tableau.com/app/profile/trupthi.raj/vizzes)
