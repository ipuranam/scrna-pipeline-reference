# scRNA-seq Pipeline Reference

An interactive single-page reference covering the end-to-end multiplexed single-cell RNA sequencing pipeline — from sample prep through sequencing through analysis.

**[→ View the live reference](https://YOUR_USERNAME.github.io/scrna-pipeline-reference/)** *(update this link after deploying to GitHub Pages)*

## What This Covers

The reference is organized as 10 tabs that flow upstream → downstream through the full pipeline:

| Tab | What It Covers |
|-----|---------------|
| **Overview** | What scRNA-seq is, how droplet-based capture works, what cell hashing / HTOs are, key terminology, and the central doublet vs. contamination problem |
| **Sample Prep** | Fixation methods (fresh vs. methanol vs. PFA), dissociation artifacts, viability, dead cell removal, and how each choice cascades downstream |
| **Experimental Design** | Loading density vs. doublet rate tradeoffs, multiplexing strategy, sequencing depth, and controls (barnyard, HTO-negative spike-ins) |
| **Sequencing Platforms** | Illumina vs. Element AVITI comparison — base diversity, PhiX requirements, accuracy, index hopping, and how platform chemistry affects barcode/UMI quality |
| **UMI Fundamentals** | How UMI deduplication works, four failure modes (collisions, PCR errors, chimeras, low diversity), and how UMI failures affect doublet detection and HTO demux |
| **Doublet Taxonomy** | Four types of doublets (cross-sample heterotypic/homotypic, within-sample heterotypic/homotypic) with detectability by HTO and transcriptome methods |
| **Contamination Sources** | Where ambient HTO comes from (wet lab + sequencing level), and HTO-specific mitigations |
| **Demux Tools** | Comparison of HTODemux, GMM-Demux, deMULTIplex2, hashedDrops, demuxmix, HashSolo, vireo/demuxlet, and Demuxafy — with robustness ratings for noisy data |
| **Raw vs Processed QC** | How each transformation step (cell calling → normalization → scaling → integration → PCA/UMAP) hides quality problems, and what to check at each layer |
| **Diagnostics** | Step-by-step protocol for determining whether you have a doublet problem or a contamination problem |

## Usage

This is a single self-contained HTML file with no build step, no dependencies, and no server required.

**To view locally:** Download `index.html` and open it in any browser.

**To deploy on GitHub Pages:**
1. Fork or clone this repo
2. Go to **Settings → Pages → Source → Deploy from branch → main**
3. Your reference will be live at `https://YOUR_USERNAME.github.io/scrna-pipeline-reference/`

## Who This Is For

- Bench scientists designing multiplexed scRNA-seq experiments
- Bioinformaticians building or debugging demultiplexing pipelines
- Team leads who need a shared reference for pipeline discussions
- Anyone new to the field who needs to understand the full stack from sample to analysis

## Contributing

This is a living document. To suggest additions or corrections, open an issue or submit a PR editing `index.html`.

## License

Internal reference — adapt the license to your needs.
