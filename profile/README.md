# OJSBR

Open-source **plugins for PKP software** — [Open Journal Systems (OJS)](https://pkp.sfu.ca/software/ojs/)
and [Open Monograph Press (OMP)](https://pkp.sfu.ca/software/omp/) — maintained by the
Brazilian community at **[ojsbr.com.br](https://ojsbr.com.br)**.

> 🇧🇷 Plugins de código aberto para os softwares da **PKP** (OJS e OMP), mantidos pela OJSBR.
> Tudo aqui é distribuído sob a **GNU GPL v3**, para toda a comunidade usar e contribuir.

Each plugin lives in its own repository, with **one branch per supported PKP version**
(`stable-3_5_0`, `stable-3_4_0`, …). Installable `.tar.gz` packages are available on each
repo's **Releases** page and in the **[Packages](https://github.com/orgs/OJSBR/packages)**
tab (GitHub Container Registry).

## Plugins

### Open Journal Systems (OJS)

| Plugin | What it does | Versions | Download |
|--------|--------------|----------|----------|
| [viewcounter](https://github.com/OJSBR/viewcounter) | Shows each article's abstract views and downloads on summaries and article pages | 3.4 · 3.5 | [Releases](https://github.com/OJSBR/viewcounter/releases) |
| [mostRead](https://github.com/OJSBR/mostRead) | Sidebar block with the most-read articles of a time window | 3.4 · 3.5 | [Releases](https://github.com/OJSBR/mostRead/releases) |
| [whatsAppContributor](https://github.com/OJSBR/whatsAppContributor) | Adds a Phone/WhatsApp (E.164) field to the contributor form | 3.4 · 3.5 | [Releases](https://github.com/OJSBR/whatsAppContributor/releases) |
| [doiInSummary](https://github.com/OJSBR/doiInSummary) | Shows the article DOI in the issue summary and journal home page | 3.4 · 3.5 | [Releases](https://github.com/OJSBR/doiInSummary/releases) |
| [ojsbrFilenameRename](https://github.com/OJSBR/ojsbrFilenameRename) | Renames the file delivered on download (configurable pattern) | 3.4 · 3.5 | [Releases](https://github.com/OJSBR/ojsbrFilenameRename/releases) |
| [orcidManualEntry](https://github.com/OJSBR/orcidManualEntry) | Restores a manual ORCID field when ORCID OAuth is not configured (authenticated ORCID stays recommended) | 3.5 | [Releases](https://github.com/OJSBR/orcidManualEntry/releases) |
| [ojsbr-webhook](https://github.com/OJSBR/ojsbr-webhook) | Sends HTTP webhooks when submissions are created and articles published | 3.4 | [Releases](https://github.com/OJSBR/ojsbr-webhook/releases) |
| [reviewerRecommendationManager](https://github.com/OJSBR/reviewerRecommendationManager) | Rename (multilingual), reorder and disable reviewer recommendations, preserving review history | 3.4 · 3.5 | [Releases](https://github.com/OJSBR/reviewerRecommendationManager/releases) |
| [accessibility](https://github.com/OJSBR/accessibility) | Sidebar accessibility controls for readers: zoom in/out, high-contrast toggle and reset (preferences persist) | 3.3 · 3.4 · 3.5 | [Releases](https://github.com/OJSBR/accessibility/releases) |

### Open Monograph Press (OMP)

| Plugin | What it does | Versions | Download |
|--------|--------------|----------|----------|
| [customMetadata](https://github.com/OJSBR/customMetadata) | Configurable extra metadata fields on the publication Metadata tab | 3.4 · 3.5 | [Releases](https://github.com/OJSBR/customMetadata/releases) |
| [crossref](https://github.com/OJSBR/crossref) | Crossref DOI registration/export for monographs and chapters (fills a gap OMP core lacks) | 3.4 · 3.5 | [Releases](https://github.com/OJSBR/crossref/releases) |
| [assignEditorGeneral](https://github.com/OJSBR/assignEditorGeneral) | Automatically assigns all active General Editors to each new submission | 3.5 | [Releases](https://github.com/OJSBR/assignEditorGeneral/releases) |

📚 The full catalog with direct download links per version is at
**[OJSBR/plugins](https://github.com/OJSBR/plugins#downloads)**.

## Installing a plugin

1. On the plugin's repository, open **Releases** and download the `.tar.gz` matching your
   OJS/OMP version.
2. In your site: **Settings → Website → Plugins → Upload A New Plugin**, upload the package,
   then enable it.

Or pull the package from **GitHub Packages** (GHCR) with [ORAS](https://oras.land):

```bash
oras pull ghcr.io/ojsbr/<plugin>:3.5.latest      # or 3.4.latest
tar -xzf <plugin>-*.tar.gz -C /path/to/ojs-or-omp/plugins/generic/
```

> 🇧🇷 Baixe o `.tar.gz` da versão do seu OJS/OMP em **Releases** e envie em
> **Configurações → Website → Plugins → Enviar um novo plugin**; ou use o `oras pull` acima.

## Contributing

Contributions are welcome in each plugin's repository — see its `CONTRIBUTING.md` and
`CODE_OF_CONDUCT.md`. Please target the branch matching the PKP version you are working on.

## Contact

- Site: [ojsbr.com.br](https://ojsbr.com.br)
- GitHub: [github.com/OJSBR](https://github.com/OJSBR)
