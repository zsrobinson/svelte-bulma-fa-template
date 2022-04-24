# Svelte, Bulma, & FA Template

This is a template allowing for easy creation of web development projects. It uses [Svelte](https://svelte.dev/) as a front-end Javascript framework, [Bulma v0.9.3](https://bulma.io/) as a CSS Framework, [Bulma Prefers Dark](https://github.com/jloh/bulma-prefers-dark) (as of April 2022) for dark-mode support, and [Font Awesome Free v6.1.1](https://fontawesome.com/) for icons. `index.html` is already configured with links to the different CSS files needed, and the project can function entirely offline once built.

## Installation Instructions

In the terminal, you can instantly create a new project by using [degit](https://github.com/Rich-Harris/degit):

```bash
npx degit zsrobinson/svelte-bulma-fa-template new-project
cd new-project
# to use TypeScript run:
# node scripts/setupTypeScript.js

npm install
npm run dev
```

This will create a new project in the `new-project` directory, install its dependencies, and start a server on http://localhost:8080. You can find more information about using TypeScript [here](https://svelte.dev/blog/svelte-and-typescript). Run `npm run build` to create a production-ready version of your app.

**Note:** Bulma, Bulma Prefers Dark, and Font Awesome are not installed via npm. Rather, they are implemented using CSS and font files that are statically linked to from `index.html`. This is done to simplify the process, but I also just wasn't able to get it working correctly when going through the trouble of using npm for all of that. Either way, this solution ensures that websites developed using this template are able to be deployed on an air-gapped network.
