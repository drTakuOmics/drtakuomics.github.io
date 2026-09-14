# Interactive project portfolio

The homepage now displays eight research projects, each with an inline SVG graphical summary, a concise finding, and controls for the question, approach, and interpretation. All content remains readable if JavaScript is disabled. Each project has a stable URL fragment, such as `/#proend` or `/#tric`.

## Publish

1. Review and merge the portfolio pull request into `master`.
2. In Settings → Pages, confirm that the existing publishing source uses `master` and `/ (root)`, or that your existing Actions workflow publishes `master`. Wait for the Pages deployment to finish.
3. Open https://drtakuomics.github.io/ and select a project. If an older page is cached, perform a hard refresh.

GitHub Pages supports this existing Jekyll setup. Keep Jekyll enabled: do not add `.nojekyll`. No npm installation or new hosting service is required.

## Edit

- `_includes/project-explorer.html` is the complete standalone HTML, CSS, SVG, and JavaScript source. Download it and open it directly in a browser to review the explorer before merging.
- Each project starts with a `PROJECT` comment. Edit its visible summary and the SVG title/description together.
- `index.md` selects the `portfolio` layout, which includes the explorer.
- Existing project pages, images, configuration, and project URLs remain available. The dairy-cow and gestational-diabetes summaries have been revised for accuracy.
- The default project-page layout now includes a return link to all projects.

The diagrams summarize relationships and study designs; they are not experimental plots or quantitative simulations. Published research, the PA28 review, ongoing research, and earlier research experience are labeled separately.

## Validation

Checked eight SVGs for valid XML, all fragment targets and unique IDs, 24 detail controls, JavaScript syntax, and the Jekyll include wiring. No browser testing or complete Jekyll build was performed in this environment; check the GitHub Pages build after merging.

## Source corrections

The dairy-cow paper reports 12 cows, subcutaneous adipose tissue only, sampling at −11 ± 3.6, +6 ± 1, and +13 ± 1.4 days relative to calving, and 1,946 / 1,524 differentially expressed genes postpartum versus prepartum. These replace the inconsistent values in the previous portfolio summary. Source: https://doi.org/10.1186/s12864-020-07235-0.

Gestational-diabetes copy describes the verified study design without carrying forward the unverified cohort count in the previous summary. Source: https://doi.org/10.1038/s41597-022-01457-5.
