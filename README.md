# In-silico-antibody-screen-PacBio-NGS-analysis
Python script for clonal analysis of translated NGS sequences. Calculates the frequency of each mutant in pooled screen outputs and the input library. Input sequences were generated via PacBio and translated using Geneious.

**NGS (PacBio) clonal analysis**
This script:
- Parses a list of NGS-translated protein sequences (from PacBio sequencing, translated in Geneious)
- Extracts in-frame antibody sequences (based on defined start/end anchors)
- Matches them against predefined mutant clone lists (e.g., from screens or pooled outputs)
- Counts their frequencies and exports results to Excel
