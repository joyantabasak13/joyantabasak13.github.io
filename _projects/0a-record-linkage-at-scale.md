---
title: "Scalable Record Linkage and Entity Resolution"
excerpt: "Fast string-similarity algorithms and blocking techniques for linking large, noisy datasets, developed under a U.S. Census Bureau–University of Connecticut cooperative agreement. Includes a linear-time Jaro similarity algorithm, SuperBlocking, and phonetic blocking."
collection: projects
---
Record linkage finds records across datasets that refer to the same person or entity. At scale, two costs dominate: comparing strings, and the huge number of candidate record pairs.

* **Linear-time Jaro similarity.** Standard algorithms for the Jaro similarity metric take quadratic time in the worst case. We gave an O(l<sub>1</sub> + l<sub>2</sub>) algorithm that computes the same measure ([ISBRA 2023](https://doi.org/10.1007/978-981-99-7074-2_3); [Journal of Computational Biology 2026](https://doi.org/10.1177/15578666261421965)).
* **SuperBlocking.** A blocking technique that removes unnecessary comparisons while keeping likely matches, with parallel record-linkage algorithms achieving near-linear speedups ([IEEE BigData 2023](https://doi.org/10.1109/BigData59044.2023.10386738)).
* **Phonetic and LLM-era blocking.** Soundex and Double Metaphone blocking ([IEEE BigData 2024](https://doi.org/10.1109/BigData62323.2024.10825041); [ISBRA 2025](https://doi.org/10.1007/978-981-95-0695-8_12)), and blocking for LLM-based record linkage ([Algorithms 2025](https://doi.org/10.3390/a18110723)).

This work is in collaboration with researchers at the U.S. Census Bureau and the University of Florida.
