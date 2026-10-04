# haoruizhang.com

Source for my personal portfolio site, live at **[haoruizhang.com](https://haoruizhang.com)**.

I'm Henry (Haorui) Zhang, a data scientist working across machine learning, LLM/AI systems and quantitative finance. The site covers my background, skills, selected projects, experience and education. All of that content lives in one file, [`src/config.ts`](src/config.ts); the components only render it.

## Stack

- [Astro](https://astro.build/) 5 — static site generator
- [Tailwind CSS](https://tailwindcss.com/) v4
- [Tabler Icons](https://tabler.io/icons)
- TypeScript for the site configuration
- GitHub Actions → GitHub Pages on every push to `main`; `public/CNAME` pins the custom domain

## Layout

```
src/
  config.ts            # all site content: name, bio, skills, projects, experience, education
  pages/index.astro    # single-page layout
  components/          # Hero, About, Projects, Experience, Education, Header, Footer
  styles/global.css
public/
  CNAME                # custom domain
  favicon.svg
.github/workflows/     # build + deploy to GitHub Pages
```

## Local development

```bash
npm install
npm run dev        # http://localhost:4321
npm run build      # static output in dist/
npm run preview
```

## Credits

Built on the [DevPortfolio](https://github.com/RyanFitzgerald/devportfolio) template by Ryan Fitzgerald, released under the MIT License (see [`LICENSE.md`](LICENSE.md)). [`CHANGELOG.md`](CHANGELOG.md) is the template's changelog.
