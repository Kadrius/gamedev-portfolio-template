# Gamedev Portfolio

This repo contains Adrián Blanco Costas's English-language XR and Unity portfolio. The current source branch is `vite-vue3`. The app is a static site built with Vue 3, Vue Router 4, TypeScript, Vite 4, and Less. It has no backend. The sibling repo `../kadrius.github.io` contains the generated site for GitHub Pages on `main`.

## Where to edit

| Area | Source |
| --- | --- |
| Bio and profile photo | `src/views/About.vue` |
| Work experience, skills, education, languages, and résumé download link | `src/views/Resume.vue` |
| Project titles, write-ups, screenshots, and video embeds | `src/data/GameProjectsData.ts` |
| Project cards, detail overlay, and styling | `src/components/ProjectsList.vue`, `src/components/ProjectDetailsOverlay.vue`, `src/css/projects.less` |
| Contact links and site navigation | `src/views/Contact.vue`, `src/components/Header.vue`, `src/router/index.ts` |
| Shared colors and site metadata | `src/css/variables.less`, `.env`, `index.html` |
| Images, icons, and PDFs copied into the build | `public/` |

The visible navigation is About me, Projects, Resume, and Contact. The Projects page showcases 3D Wind Training, 7 Cidades - Patrones, La Pinta VR, AR Plumbing Configurator, Aquis Querquennis, Timetrip Narahío, and XTAS. The `/other-projects` route contains sample entries from the original template. Its navigation link is commented out.

## Local workflow

Run these commands from the source repo:

```powershell
npm ci
npm run dev
npm run build
npm run serve
```

- `npm ci` installs the versions in `package-lock.json`. Node 26.13.1 and npm 11.20.0 successfully built this checkout. The repo does not pin a Node or npm version. If PowerShell blocks `npm.ps1`, `npm.cmd` runs the same npm.
- `npm run dev` starts Vite for local editing. `npm run build` writes the production site to the ignored `dist/` folder. `npm run serve` previews that built output.
- `npm run lint` runs ESLint with `--fix` and can modify source files.

## Publishing

Make changes in this source repo. Build and preview them, then copy the **contents** of `dist/` to the root of `../kadrius.github.io` when publishing. Review the deployment diff, including stale generated bundles, before committing and pushing the publish repo's `main` branch.

## Baseline for future updates

- The June 2024 portfolio still lists Xoia as the current employer and links to `public/d/AdrianBlancoResume2024.pdf`. Verify current bio and résumé details before updating them.
- The local source build and the files used by the checked-in GitHub Pages site matched when compared, apart from line endings and the favicon URL. The source `index.html` uses `/dist/favicon.ico`. For the next deployment, check that it points to `/favicon.ico`, which is copied from `public/` to the deployed site root.
