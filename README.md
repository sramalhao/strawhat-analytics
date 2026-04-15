# 🏴‍☠️ One Piece Data Analysis: Manga vs. Anime

An in-depth data analysis project exploring the structural differences between Eiichiro Oda's original *One Piece* manga and its television adaptation by Toei Animation. 

Using Python, Pandas, and Data Visualization libraries (Seaborn/Matplotlib), this notebook investigates the pacing, filler content, and structural evolution of one of the longest-running series in history.

## 📊 Dataset
The analysis is based on the `OnePieceArcs.csv` dataset [1], which contains comparative metrics for every story arc, including:
* **Manga Metrics:** `TotalChapters`, `TotalPages`, `Manga%` [1].
* **Anime Metrics:** `TotalEpisodes`, `TotalMinutes`, `Anime%` [1].

## 🔍 Analyses Performed

This project is divided into 5 narrative parts, containing 8 distinct analyses:

### Part 1: The Size of the World
**1. Identification of the Largest Arcs**
We measure the colossal scale of *One Piece* by ranking the longest arcs in screen time and reading material. For instance, the data reveals that the *Dressrosa Arc* alone spans 118 episodes (2,832 minutes), followed closely by the *Whole Cake Island Arc* with 95 episodes [1].

### Part 2: The Original Work
**2. Manga Density (Pages per Chapter)**
Before looking at the anime, we analyze how Eiichiro Oda structures the source material. By dividing `TotalPages` by `TotalChapters` [1], we observe the historical trends in chapter length and density throughout the decades of publication.

### Part 3: The TV Transition
**3. Filler Analysis (Anime Original Content)**
Identifying arcs with `0` manga chapters (e.g., the 11-episode *G-8 Arc* or the 8-episode *Warship Island Arc* [1]) to quantify the total number of episodes and hours dedicated entirely to non-canon TV storylines.

**4. Story Expansion and Proportion**
By comparing the `Manga%` and `Anime%` metrics [1], we calculate the percentage discrepancy to reveal which storylines received disproportionate spotlights on TV compared to their original comic counterparts.

### Part 4: The Great Fan Debate (Pacing)
**5. Adaptation Pacing (Manga vs. Anime)**
Calculating the classic pacing metric (`TotalChapters / TotalEpisodes`) [1] to see which arcs moved quickly (adapting multiple chapters per episode, like early arcs) and which ones dragged out the source material.

**6. The "Dragging" Level (Screen Minutes per Page)**
A more precise pacing metric. By crossing the total screen minutes with the exact number of manga pages read (`TotalMinutes / TotalPages`) [1], we calculate exactly how much screen time Toei Animation used to adapt a single page of the manga, revealing the true density of the episodes scene-by-scene.

### Part 5: Historical View
**7. Pacing Evolution Over Time**
Plotting the pacing metric against the arc's starting episode (`Start onEpisode`) [1] on a timeline. This visualizes the historical decline in adaptation speed, culminating in anomalies like the *Levely Arc* (6 chapters stretched across 12 episodes) [1].

**8. Era Analysis (Pre-Timeskip vs. Post-Timeskip)**
The ultimate conclusion. We split the dataset into two distinct eras using the *Return to Sabaody Arc* (Chapter 598 / Episode 517) [1] as the dividing line. This analysis proves a radical shift in the studio's strategy: abandoning long filler seasons in exchange for drastically slowing down the pacing of canon episodes.

## 🚀 How to Run
1. Clone this repository.
2. Ensure you have Python installed along with the required libraries (`pandas`, `matplotlib`, `seaborn`).
3. Run `jupyter notebook` in your terminal.
4. Open the `One_Piece_Analysis.ipynb` notebook and run the cells to see the generated charts and insights.
