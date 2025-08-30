# In-silico-antibody-screen-PacBio-NGS-analysis
Python script for clonal analysis of translated NGS sequences. Calculates the frequency of each mutant in pooled screen outputs and the input library. Input sequences were generated via PacBio and translated using Geneious.

**NGS (PacBio) clonal analysis**
This script:
- Parses a list of NGS-translated protein sequences (from PacBio sequencing, translated in Geneious)
- Extracts in-frame antibody sequences (based on defined start/end anchors)
- Matches them against predefined mutant clone lists (e.g., from screens or pooled outputs)
- Counts their frequencies and exports results to Excel

**CDR-colored heatmap of antibodies**
This script:
- Generates a color-coded heatmap of clone enrichment across NGS input library and screen outputs.
- Highlights mutations across CDR regions using right-aligned mutation segments and color legends.
- Input: CSV file containing clone names, labels, and frequency percentages in with `Mutant`, `Label`, and `% frequency` columns, respectively.
- Output: A `.png` heatmap showing clone abundance and CDR-colored mutation segments.
CDRs are color-coded as follows:
  - CDRH1: red
  - CDRH2: orange
  - CDRH3: blue
  - CDRL1: pink
  - CDRL2: lime
  - CDRL3: cyan
