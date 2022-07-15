# Reproducing Yarn PnP TailwindCSS Intellisense Bug

## Steps to reproduce the error

1. Clone the repo
2. `$ yarn`
3. Open the folder in vs code

## Steps taken to scaffold this project

1. `yarn create vite appName --template react`

2. `cd appName`

3. `yarn`

4. `yarn add -D tailwindcss postcss autoprefixer daisyui`

5. `npx tailwindcss init -p`

After these, I added the necessary tailwind config as can be seen in the repo.
Removing the plugin "daisyui" fixes the error.
