## web next test

npx create-next-app@latest --empty

✔ What is your project named? … web

✔ Would you like to use TypeScript? … Yes

✔ Would you like to use ESLint? … No 

✔ Would you like to use Tailwind CSS? … No 

✔ Would you like your code inside a `src/` directory? … Yes

✔ Would you like to use App Router? (recommended) …  Yes

✔ Would you like to use Turbopack for `next dev`? …  Yes

✔ Would you like to customize the import alias (`@/*` by default)? … No 

Creating a new Next.js app in /home/miguel/workspaces/nlw/web.

Installing dependencies:

- react
- react-dom
- next

Installing devDependencies:

- typescript
- @types/node
- @types/react
- @types/react-dom

### Instalação do tailwindcss

npm install tailwindcss @tailwindcss/postcss postcss

criar na raiz do projeto: postcss.config.mjs

Colocar no arquivo:

const config = {

  plugins: {

    "@tailwindcss/postcss": {},

  },

};

export default config;

Na raiz do projeto "locals.css":

@import "tailwindcss";

No layout.tsx    -   importar o locals.css

No VScode, instalar as extensões:

TailwindCSS IntelliSense e PostCSS Language Support. Este último para construção do theme.

@theme {

    --color-*: initial; Faz com que não tenha mais as cores do tailwind só estas

  --color-blue: #6f9de2;
}

Na className=" antialiased "  Deixa a font melhor nos navegadores chrome



