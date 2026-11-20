# Krinal Gami: Portfolio

Personal portfolio of **Krinal Gami**, an AI/ML engineer who builds AI that answers from your code and documents.

The whole site is one static file, `index.html`. There is no build step and no dependencies to install.

## What's on the site

- **Hero:** the name is made of particles that scatter when you move or drag the cursor, and its colors change on their own. A cartoon avatar's eyes follow the cursor. You can change its skin, hair and outfit colors, and click it to say hello.
- **Cursor:** a round ring cursor with a glowing trail that gets thicker while you drag.
- **Work gallery:** drag-to-scroll project cards. Three of them open a case study with a live demo that runs on sample data:
  - **PR Sentinel:** AI code review that comments right on your pull request.
  - **DevMind:** ask a codebase questions and get answers, explanations and docs.
  - **PDF RAG Bot:** chat with a document, with every answer citing its source.
- **More projects:** Cricket Data Analytics, Movie Recommender, Spam Message Verifier and Car Price Predictor, linked to GitHub.
- **Contact:** email (click to copy), CV download, GitHub and LinkedIn.
- A small avatar guide in the corner comments as you scroll.

## Run it locally

Open `index.html` in a browser. That's all.

To serve it instead:

```bash
npx serve .
```

## Deploy on GitHub Pages

1. Create a **public** repository. Name it `Krinal09.github.io` for the short address `https://krinal09.github.io`. With any other name, the address becomes `https://krinal09.github.io/<repo-name>/`.
2. Upload `index.html` and `README.md` to the top level of the repository. The file must be named exactly `index.html`.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, set **Source** to **Deploy from a branch**. Choose branch **main** and folder **/ (root)**, then click **Save**.
5. Wait 1 to 2 minutes. The Pages screen then shows the live link.

Or push from a terminal:

```bash
git init
git add .
git commit -m "Add portfolio"
git branch -M main
git remote add origin https://github.com/Krinal09/Krinal09.github.io.git
git push -u origin main
```

To update the site later, replace `index.html` and commit. The site refreshes in about a minute.

## Customize

Everything is inside `index.html`.

| What | Where to look |
| --- | --- |
| Colors | the `:root` CSS variables at the top of the `<style>` block |
| Project cards and links | the `#work` section |
| Email, CV, GitHub and LinkedIn links | the `#contact` section |
| Tab logo | the `<link rel="icon">` tag in `<head>` |
| Name effect colors | the `PAL` list in the script |

The CV button points to a Google Drive file. Share that file as **Anyone with the link can view**, or visitors will see a request-access page.

## Built with

Plain HTML, CSS and JavaScript. Fonts are Unbounded, Hanken Grotesk and JetBrains Mono from Google Fonts.

## Contact

- Email: krinalgami@gmail.com
- GitHub: [github.com/Krinal09](https://github.com/Krinal09/)
- LinkedIn: [linkedin.com/in/krinal-gami-3aaa83239](https://www.linkedin.com/in/krinal-gami-3aaa83239/)
