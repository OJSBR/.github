# OJSBR

Open-source **plugins for PKP software** — [Open Journal Systems (OJS)](https://pkp.sfu.ca/software/ojs/)
and [Open Monograph Press (OMP)](https://pkp.sfu.ca/software/omp/) — maintained by the
Brazilian community at **[ojsbr.com](https://ojsbr.com)**.

> 🇧🇷 Plugins de código aberto para os softwares da **PKP** (OJS e OMP), mantidos pela OJSBR.
> Tudo aqui é distribuído sob a **GNU GPL v3**, para toda a comunidade usar e contribuir.

Each plugin lives in its own repository, with **one branch per supported PKP version**
(`stable-3_5_0`, `stable-3_4_0`, …). Installable `.tar.gz` packages are available on each
repo's **Releases** page and in the **[Packages](https://github.com/orgs/OJSBR/packages)**
tab (GitHub Container Registry).

When a plugin exists for both applications, the OMP edition lives in its own repository with
an **`Omp` suffix** (`staticEditorialTeam` → `staticEditorialTeamOmp`). The plugin folder
inside the package keeps the original name — PKP derives the class namespace from the
installation directory, so never rename it.

> 🇧🇷 Quando o plugin existe para as duas aplicações, a versão de OMP tem repositório próprio
> com o sufixo **`Omp`**. A pasta do plugin dentro do pacote mantém o nome original — o PKP
> deriva o namespace da classe do diretório de instalação, então não renomeie a pasta.

## Plugins

### Works on both OJS and OMP

The same package installs on either application.

> 🇧🇷 O mesmo pacote serve para as duas aplicações.

| Plugin | What it does | Versions | Download |
|--------|--------------|----------|----------|
| [accessibility](https://github.com/OJSBR/accessibility) | Sidebar accessibility controls for readers: zoom in/out, high-contrast toggle and reset (preferences persist) | 3.3 · 3.4 · 3.5 | [Releases](https://github.com/OJSBR/accessibility/releases) |
| [vlibras](https://github.com/OJSBR/vlibras) | Embeds the VLibras widget (Brazilian government's Portuguese→Libras sign-language translator) with its floating avatar | 3.3 · 3.4 · 3.5 | [Releases](https://github.com/OJSBR/vlibras/releases) |
| [languageToggleByFlag](https://github.com/OJSBR/languageToggleByFlag) | Sidebar language switcher with country flags (also works on OPS); adapted for 3.5 by OJSBR, original by Lepidus Tecnologia | 3.5 | [Releases](https://github.com/OJSBR/languageToggleByFlag/releases) |
| [shariff](https://github.com/OJSBR/shariff) | Privacy-friendly social media share buttons (Shariff) — unofficial OJSBR build of ojsde/shariff with the Portuguese fixes proposed in ojsde/shariff#54, maintained until the official release | 3.5 | [Releases](https://github.com/OJSBR/shariff/releases) |

### Open Journal Systems (OJS)

| Plugin | What it does | Versions | Download |
|--------|--------------|----------|----------|
| [viewcounter](https://github.com/OJSBR/viewcounter) | Shows each article's abstract views and downloads on summaries and article pages | 3.4 · 3.5 | [Releases](https://github.com/OJSBR/viewcounter/releases) |
| [mostRead](https://github.com/OJSBR/mostRead) | Sidebar block with the most-read articles of a time window | 3.4 · 3.5 | [Releases](https://github.com/OJSBR/mostRead/releases) |
| [keywordCloudClassicBeautiful](https://github.com/OJSBR/keywordCloudClassicBeautiful) | Packed keyword cloud sized by frequency (the classic behaviour restored), self-contained; original keywordCloud by PKP/SFU, maintained by Lepidus | 3.4 · 3.5 | [Releases](https://github.com/OJSBR/keywordCloudClassicBeautiful/releases) |
| [whatsAppContributor](https://github.com/OJSBR/whatsAppContributor) | Adds a Phone/WhatsApp (E.164) field to the contributor form | 3.4 · 3.5 | [Releases](https://github.com/OJSBR/whatsAppContributor/releases) |
| [doiInSummary](https://github.com/OJSBR/doiInSummary) | Shows the article DOI in the issue summary and journal home page | 3.4 · 3.5 | [Releases](https://github.com/OJSBR/doiInSummary/releases) |
| [ojsbrFilenameRename](https://github.com/OJSBR/ojsbrFilenameRename) | Renames the file delivered on download (configurable pattern) | 3.4 · 3.5 | [Releases](https://github.com/OJSBR/ojsbrFilenameRename/releases) |
| [reviewerRecommendationManager](https://github.com/OJSBR/reviewerRecommendationManager) | Rename (multilingual), reorder and disable reviewer recommendations, preserving review history | 3.4 · 3.5 | [Releases](https://github.com/OJSBR/reviewerRecommendationManager/releases) |
| [orcidManualEntry](https://github.com/OJSBR/orcidManualEntry) | Restores a manual ORCID field (contributor form, user registration and profile) when ORCID OAuth is not configured (authenticated ORCID stays recommended) | 3.5 | [Releases](https://github.com/OJSBR/orcidManualEntry/releases) |
| [staticEditorialTeam](https://github.com/OJSBR/staticEditorialTeam) | Brings back the static Editorial Team page: shows the journal's free-text setting instead of the dynamic masthead listing introduced in 3.5 | 3.5 | [Releases](https://github.com/OJSBR/staticEditorialTeam/releases) |
| [classicUserEditor](https://github.com/OJSBR/classicUserEditor) | Restores direct editing of users (given name, family name, email and roles) for managers and administrators, alongside the 3.5 invitation manager | 3.5 | [Releases](https://github.com/OJSBR/classicUserEditor/releases) |
| [blindReviewGuard](https://github.com/OJSBR/blindReviewGuard) | Checks the files a reviewer is about to receive for anything that identifies the authors and can remove the identifying metadata | 3.5 | [Releases](https://github.com/OJSBR/blindReviewGuard/releases) |
| [authorContributorEditor](https://github.com/OJSBR/authorContributorEditor) | Gives authors back the editing of the contributor list of their own submissions when their user group is allowed to edit submission metadata, as in 3.3/3.4 | 3.5 | [Releases](https://github.com/OJSBR/authorContributorEditor/releases) |
| [reviewerDirectory](https://github.com/OJSBR/reviewerDirectory) | Editor-only directory of reviewers (profiles + review stats, active-submission IDs, configurable columns, Excel export) and a period/issue reviewer roster (nominata) | 3.5 | [Releases](https://github.com/OJSBR/reviewerDirectory/releases) |
| [controlledVocabSplitter](https://github.com/OJSBR/controlledVocabSplitter) | Splits keywords, subjects, disciplines and supporting agencies pasted as a single line into separate terms, in the field and on every save (semicolon, comma or period; keeps legal references and species initials whole) | 3.5 | [Releases](https://github.com/OJSBR/controlledVocabSplitter/releases) |
| [crossrefConference](https://github.com/OJSBR/crossrefConference) | Deposits DOIs with Crossref as conference proceedings (`<conference>`/`<conference_paper>`) instead of journal records, as a DOI registration agency: event name, edition number, dates and location, and the proceedings DOI the papers hang off | 3.5 | [Releases](https://github.com/OJSBR/crossrefConference/releases) |
| [requiredMultilingualMetadata](https://github.com/OJSBR/requiredMultilingualMetadata) | Require the title, the abstract and the keywords in metadata languages beyond the submission language | 3.5 | [Releases](https://github.com/OJSBR/requiredMultilingualMetadata/releases) |
| [epubJsViewer](https://github.com/OJSBR/epubJsViewer) | Embedded EPUB galley reader (zoom, table of contents, reading modes) powered by epub.js; continues the `epubViewer` by Lepidus Tecnologia, discontinued in 2025 when the Bibi engine stopped being maintained | 3.5 | [Releases](https://github.com/OJSBR/epubJsViewer/releases) |
| [citations](https://github.com/OJSBR/citations) | Citation counts and the list of citing works from Crossref Cited-by, Scopus, Europe PMC and Google Scholar, on the article page; OJS 3.5 fork of `RBoelter/citations`, original plugin by Ronny Bölter | 3.5 | [Releases](https://github.com/OJSBR/citations/releases) |
| [pln](https://github.com/OJSBR/pln) | PKP Preservation Network (PLN / PKP PN) — unofficial OJS 3.5 build (based on pkp/pln#117), maintained until the official release | 3.5 | [Releases](https://github.com/OJSBR/pln/releases) |
| [ojsbr-webhook](https://github.com/OJSBR/ojsbr-webhook) | Sends HTTP webhooks when submissions are created and articles published | 3.4 | [Releases](https://github.com/OJSBR/ojsbr-webhook/releases) |

### Open Monograph Press (OMP)

| Plugin | What it does | Versions | Download |
|--------|--------------|----------|----------|
| [crossref](https://github.com/OJSBR/crossref) | Crossref DOI registration/export for monographs and chapters (fills a gap OMP core lacks) | 3.4 · 3.5 | [Releases](https://github.com/OJSBR/crossref/releases) |
| [customMetadata](https://github.com/OJSBR/customMetadata) | Configurable extra metadata fields on the publication Metadata tab | 3.4 · 3.5 | [Releases](https://github.com/OJSBR/customMetadata/releases) |
| [assignEditorGeneral](https://github.com/OJSBR/assignEditorGeneral) | Automatically assigns all active General Editors to each new submission | 3.5 | [Releases](https://github.com/OJSBR/assignEditorGeneral/releases) |
| [keywordCloudClassicBeautifulOmp](https://github.com/OJSBR/keywordCloudClassicBeautifulOmp) | Packed keyword cloud of the press's books, sized and coloured by frequency, self-contained (no CDN) | 3.5 | [Releases](https://github.com/OJSBR/keywordCloudClassicBeautifulOmp/releases) |
| [mostReadOmp](https://github.com/OJSBR/mostReadOmp) | Sidebar block with the most-read books of a time window | 3.5 | [Releases](https://github.com/OJSBR/mostReadOmp/releases) |
| [staticEditorialTeamOmp](https://github.com/OJSBR/staticEditorialTeamOmp) | Brings back the static Editorial Team page: shows the press's free-text setting instead of the dynamic masthead listing | 3.5 | [Releases](https://github.com/OJSBR/staticEditorialTeamOmp/releases) |
| [classicUserEditorOmp](https://github.com/OJSBR/classicUserEditorOmp) | Restores direct editing of users (name, email and roles) for managers and administrators, alongside the 3.5 invitation manager | 3.5 | [Releases](https://github.com/OJSBR/classicUserEditorOmp/releases) |
| [controlledVocabSplitterOmp](https://github.com/OJSBR/controlledVocabSplitterOmp) | Splits keywords, subjects, disciplines and supporting agencies pasted as a single line into separate terms, in the field and on every save | 3.5 | [Releases](https://github.com/OJSBR/controlledVocabSplitterOmp/releases) |
| [ojsbrFilenameRenameOmp](https://github.com/OJSBR/ojsbrFilenameRenameOmp) | Renames the file delivered on download (configurable pattern), without touching the file on disk | 3.5 | [Releases](https://github.com/OJSBR/ojsbrFilenameRenameOmp/releases) |
| [orcidManualEntryOmp](https://github.com/OJSBR/orcidManualEntryOmp) | Restores a manual ORCID field on the contributor form when ORCID OAuth is not configured | 3.5 | [Releases](https://github.com/OJSBR/orcidManualEntryOmp/releases) |
| [requiredMultilingualMetadataOmp](https://github.com/OJSBR/requiredMultilingualMetadataOmp) | Require the title, the abstract and the keywords in languages beyond the submission language | 3.5 | [Releases](https://github.com/OJSBR/requiredMultilingualMetadataOmp/releases) |
| [reviewerDirectoryOmp](https://github.com/OJSBR/reviewerDirectoryOmp) | Editor-only directory of reviewers (profiles + review stats) and a per-period or per-series reviewer roster (nominata) | 3.5 | [Releases](https://github.com/OJSBR/reviewerDirectoryOmp/releases) |

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
tar -xzf <plugin>-*.tar.gz -C /path/to/ojs-or-omp/plugins/generic/   # block plugins → plugins/blocks/
```

> 🇧🇷 Baixe o `.tar.gz` da versão do seu OJS/OMP em **Releases** e envie em
> **Configurações → Website → Plugins → Enviar um novo plugin**; ou use o `oras pull` acima.

## Contributing

Contributions are welcome in each plugin's repository — see its `CONTRIBUTING.md` and
`CODE_OF_CONDUCT.md`. Please target the branch matching the PKP version you are working on.

## Contact

- Site: [ojsbr.com](https://ojsbr.com)
- GitHub: [github.com/OJSBR](https://github.com/OJSBR)
