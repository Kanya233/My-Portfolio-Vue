# Kanya Masinda Portfolio

A responsive single-page portfolio built with Vue 3 and Vite. It presents Kanya’s background, technical skills, selected work and a Formspree-powered contact form.

## Run locally

```sh
npm install
npm run dev
```

Create a production build with:

```sh
npm run build
```

## Adding projects

Project content is data-driven in `src/components/Projects.vue`. Add a project’s title, description, technologies, GitHub URL, live/demo URL and screenshot asset there when those details are available.

## Contact form

The contact form submits to the existing Formspree endpoint configured in `src/components/Contact.vue`. Confirm that endpoint is owned and active before deployment.
