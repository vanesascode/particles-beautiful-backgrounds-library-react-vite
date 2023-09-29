# Particles.js - beautiful and dynamic backgrounds library demo

## 🌟BACKGROUND PARTICLES

![image](https://github.com/vanesascode/introduction-to-sqlalchemy-sqlite-python-venv-dbbrowser/assets/131259155/e38528da-b55a-4045-a401-3fa62abdf0ca)

Installation:

- [x] run: `react-tsparticles`
- [x] run: `tsparticles`
- [x] run: `tsparticles-slim`

Configure a component like this:

```
import Particles from "react-tsparticles";
import { loadSlim } from "tsparticles-slim"; // loads tsparticles-slim
import { useCallback, useMemo } from "react";

const ParticlesComponent = (props) => {

  const options = useMemo(() => {

    return {

      //HERE YOUR OPTIONS: https://particles.js.org/
      //HERE a website to pass the JSON to without quotes: https://csvjson.com/json_beautifier

         };
  }, []);

  const particlesInit = useCallback((engine) => {
    loadSlim(engine);
  }, []);

  return <Particles id={props.id} init={particlesInit} options={options} />;
};

export default ParticlesComponent;
```

Then, import the component into the main/app.js file, and set it as the last component in the return.

Here is a [demo and explanation](https://github.com/tsparticles/react-demo/blob/main/src/components/Particles.js)

## 🌟TO DEPLOY

- [x] run: `npm run build`

The `public` folder is resulted. Drag it into the Netlify deployment service manual deploy feature.

(If you are working with codespace, download the whole project to get the public folder)

## 🌟VITE

- To create a project:

- [x] run: `npm create vite@latest`

select 'React' as the framework and select 'Javascript' as the variant.

- [x] run: `npm install` to install all the dependencies

---

- To run the project:

- [x] run: `npm run dev`

---

## 🌟TAILWIND

Go to the frameworks guides. [In this case for Vite](https://tailwindcss.com/docs/guides/vite)

- [x] `npm install -D tailwindcss postcss autoprefixer`

- [x] `npx tailwindcss init -p`

To generate a TypeScript config file, use the --ts flag:

- [x] `npx tailwindcss init --ts`

💡 Generate a complete configuration file that includes all of Tailwind’s default configuration:

- [x] `npx tailwindcss init --full`

---

## 🌟DEPLOYMENT - VITE & VERCEL

Prepare your Vite application:

- [x] Run `npm run build`

In Vite, running the npm run build command triggers the build process, which generates a production-ready build of your application, the folder `dist`

If you don't have Vercel installed:

- [x] Create an account in Vercel.com
- [x] Install the Now package in the terminal, globally: `npm install now -g`
- [x] Run: `now` in the terminal, inside the root folder of the project.
- [x] The terminal will ask you your email.
- [x] Then, you'll receive an email in which you will have to verify your credentials.

Deployment steps:

- [x] Run: `now` again.
- [x] It will ask you if you want to deploy. You say Y
- [x] Asks the scope (your name)
- [x] Asks if you want to link to existing project. You say N
- [x] In which directory is your code located? If it's in the root folder just leave it like this: ./
- [x] You want to override the settings? You say N
- [x] You can now get the URL that is in the ✅ production line. It's live!

Add new changes to the live URL

- [x] Run: `now --prod` Then, changes are saved in the same URL you published before.

---
