# install with vite

```
npm create vite@latest
cd {app_name}
npm install
npm run dev
npm i axios
npm i react-query
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p
npm install @formkit/auto-animate
```

# tailwind.config.cjs

```
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: [
    "./index.html",
    "./src/**/*.{js,ts,jsx,tsx}"
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}
```
# index.css
```
@tailwind base;
@tailwind components;
@tailwind utilities;
```
# add polling on vite.config.ts for hot reload on WSL
```
export default defineConfig({
  plugins: [react()],
  server: {
    watch:{
      usePolling: true
    }
  }
})
```
