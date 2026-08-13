# The Burger Debugger

An open-access, browser-based engineering lab that asks high school students to design the most sustainable burger their classmates would actually eat.

**Live demo:** https://jchery25.github.io/Burger-Debugger/

Students blend six protein sources, watch the land, water and climate costs of their design update in real time against a class-sized resource budget, and then defend their choice on a printable worksheet. Every environmental figure traces to peer-reviewed research, and the app is explicit about which numbers are measurements and which are teaching estimates.

---

## Why this exists

Most alternative protein materials tell students that some proteins are more efficient than others. This lab makes them feel it. The budget is finite, the class has to eat, and no single protein wins on every axis — so students have to make and defend a trade-off, which is what engineering design actually is.

The central constraint is the one students never expect: a burger that scores perfectly on land, water and pollution but that nobody will eat is a failed design. Acceptance is a hard requirement, not a bonus.

---

## What's in it

### Screen 1 — Mission brief
Sets up the scenario (an end-of-year class party) and teaches feed-to-food conversion efficiency with a 100-square grid. Students see how much protein actually leaves the farm as edible food per pathway — beef converts about 3%, so 97 of the 100 squares leak out. This is the conceptual foundation for everything on the next screen.

### Screen 2 — The lab
The build environment. Students:

- blend **six protein sources** — beef, pork, chicken, legumes, soy protein, and fermented (microbial) protein
- set the **party size**, which scales the class resource budgets and changes how many classmates need to be satisfied
- watch a **3D burger** rebuild itself as the blend changes
- track live **percentage-of-budget** readouts for land, water and climate pollution
- pass or fail **five design rules**: land, water and pollution inside budget; taste score at or above 70; at least 60% of the class would eat it

Five in-context info buttons explain the protein sources, the taste score, the budgets, the class panel and the score breakdown in plain language — no prior chemistry or life-cycle-assessment vocabulary required.

**Print the worksheet** on this screen opens the browser print dialog with the two-page student worksheet only.

### Screen 3 — Sources & data
Twelve citations grouped by what they control in the simulation, each with a DOI or permanent link and a sentence on which number it drives. Below that, a panel naming the six figures that are teaching estimates rather than measurements. Students are told plainly that cultivated meat's published footprint spans roughly 2 to 1,500 kg CO₂e per kg, and that the lab uses a middle value because nobody knows yet.

This screen exists so students can interrogate the model instead of trusting it, and so teachers can answer "where did that number come from?" in one click.

### The student worksheet
Two letter-size pages, prints front and back:

- **Page 1** — record the design (name, blend, party size, three budget percentages, final score), check the five rules with a my-number column, and log two rejected designs with the reason each lost
- **Page 2** — four evidence-based reflection questions (each requires a number from the lab), a predict/test/result iteration grid, and a student-facing success-criteria checklist

---

## Standards alignment

| Standard | Where it's addressed |
| --- | --- |
| **HS-ETS1-2** — Design a solution to a complex real-world problem by breaking it into smaller, solvable problems | The lab separates the burger into six independently adjustable protein inputs, each with its own resource profile |
| **HS-ETS1-3** — Evaluate a solution to a complex real-world problem based on prioritized criteria and trade-offs | The five design rules are simultaneous constraints that cannot all be maximized; worksheet section D2 requires naming the trade-off |
| **HS-LS2-7** — Design, evaluate and refine a solution for reducing the impacts of human activities on the environment and biodiversity | Land, water and eutrophying-emissions budgets, plus the required iteration in worksheet section E |
| **SEP: Using mathematics and computational thinking** | Percentage-of-budget arithmetic scaled by class size |
| **SEP: Engaging in argument from evidence** | Every worksheet answer must cite a number produced by the lab |
| **CCC: Systems and system models** | Sources & Data screen surfaces the model's assumptions and uncertainty ranges as objects of study |

Suggested fit: 2–3 class periods, or one period plus homework. Works in environmental science, biology, food science, and introductory engineering.

---

## Data sources

All environmental figures are rescaled so one conventional beef burger equals 100% of a plain-beef reference. This keeps the arithmetic doable mentally on a Chromebook without changing the ratios between protein sources.

**Core dataset**
- Poore, J. & Nemecek, T. "Reducing food's environmental impacts through producers and consumers." *Science* 360, 987–992 (2018). [doi:10.1126/science.aaq0216](https://doi.org/10.1126/science.aaq0216) — a meta-analysis of 38,700 farms in 119 countries covering 40 food products
- Ritchie, H., Rosado, P. & Roser, M. "Environmental Impacts of Food Production." *Our World in Data* (2022)

**Water**
- Mekonnen, M. M. & Hoekstra, A. Y. "A Global Assessment of the Water Footprint of Farm Animal Products." *Ecosystems* 15, 401–415 (2012). [doi:10.1007/s10021-011-9517-8](https://doi.org/10.1007/s10021-011-9517-8)

**Conversion efficiency**
- Shepon, A., Eshel, G., Noor, E. & Milo, R. "Energy and protein feed-to-food conversion efficiencies in the US and potential food security gains." *Environmental Research Letters* 11, 105002 (2016). [doi:10.1088/1748-9326/11/10/105002](https://doi.org/10.1088/1748-9326/11/10/105002)

**Newer protein pathways**
- Humpenöder, F. et al. "Projected environmental benefits of replacing beef with microbial protein." *Nature* 605, 90–96 (2022). [doi:10.1038/s41586-022-04629-w](https://doi.org/10.1038/s41586-022-04629-w)
- Sinke, P. et al. "Ex-ante life cycle assessment of commercial-scale cultivated meat production in 2030." *Int. J. Life Cycle Assess.* 28, 234–254 (2023). [doi:10.1007/s11367-022-02128-8](https://doi.org/10.1007/s11367-022-02128-8)
- Risner, D. et al. "Environmental impacts of cultured meat: a cradle-to-gate life cycle assessment." *bioRxiv* preprint (2023) — preprint, not yet peer-reviewed
- Tuomisto, H. L. & Teixeira de Mattos, M. J. "Environmental impacts of cultured meat production." *Environ. Sci. Technol.* 45, 6117–6123 (2011). [doi:10.1021/es200130u](https://doi.org/10.1021/es200130u)

**Nutrition**
- USDA FoodData Central, Agricultural Research Service
- Willett, W. et al. "Food in the Anthropocene: the EAT–Lancet Commission on healthy diets from sustainable food systems." *The Lancet* 393, 447–492 (2019). [doi:10.1016/S0140-6736(18)31788-4](https://doi.org/10.1016/S0140-6736(18)31788-4)

**Further reading for teachers**
- FAO GLEAM — Global Livestock Environmental Assessment Model
- IPCC Special Report on Climate Change and Land (2019), Ch. 5: Food Security

### Known limitations

Stated in the app and repeated here so anyone adapting it knows what they are inheriting:

- **Nutrient pollution** is modelled from the eutrophying-emissions column of Poore & Nemecek and simplified into a single index. Directionally correct, not an LCA result.
- **Taste and nutrition scores** are teaching estimates. No sensory panel produced them; they exist so the puzzle has more than one workable answer.
- **Resource budgets** were set by the author, not a standards body, and are tuned so several very different blends can pass.
- **Class acceptance** is a curve derived from the taste score, not survey data.
- **Cultivated meat** uses a middle value from a literature spanning roughly three orders of magnitude.
- **The 100-point scale** is a presentation choice, not a unit.

---

## Running and deploying it

The app is a single self-contained `index.html`. No build step, no server, no dependencies, no network access at runtime.

**Locally:** download `index.html` and open it in any browser. It works offline, which matters for Chromebook carts on school networks.

**GitHub Pages:** Settings → Pages → Source: Deploy from a branch → `main` / `/ (root)`. The site appears at `https://<user>.github.io/Burger-Debugger/` within a minute or two.

**Anywhere else:** drag `index.html` onto Netlify Drop, drop it in Google Drive, or attach it to an LMS assignment.

### Repository contents

| File | Purpose |
| --- | --- |
| `index.html` | The deployable app — everything inlined, this is the only file you need |
| `Burger Lab.dc.html` | Editable source for the three-screen app |
| `Burger Lab Worksheet.dc.html` | Editable source for the two-page student worksheet |
| `burger-3d.js` | The 3D burger renderer |
| `doc-page.js` | Print/pagination shell used by the worksheet |
| `support.js` | Runtime for the source files |

To modify the app, edit the `.dc.html` sources and re-bundle into `index.html`. To use it as-is, ignore everything but `index.html`.

---

## Adapting it for your classroom

Reasonable places to intervene:

- **Change the budgets** to make the puzzle harder or easier for your students
- **Change the acceptance threshold** from 60% if your class has a different composition
- **Swap the scenario** — a school cafeteria menu, a food truck, a dorm dining hall all work with the same math
- **Add a protein source** relevant to your region or your students' diets
- **Have students challenge the data** using FAO GLEAM for their own part of the world; the Sources & Data screen is built to support this

If you adapt it and it works, open an issue or a pull request. Classroom evidence about what actually lands with students is the most useful contribution this project can receive.

---

## Contributing

Issues and pull requests welcome, particularly:

- corrections or updates to the underlying data, with citations
- accessibility improvements
- translations
- worksheet variants for different grade levels or course contexts
- reports from classroom use — what worked, what confused students, what you cut

---

## License

Curriculum content and worksheet: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Use it, remix it, teach with it, sell a course that includes it — just credit the source.

Code: MIT.

---

## Acknowledgments

Developed following the Good Food Institute's Train-the-Trainer Program and the Future of Food course.
