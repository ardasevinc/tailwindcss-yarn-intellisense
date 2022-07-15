# Reproducing Yarn PnP TailwindCSS Intellisense Bug

## Steps to reproduce the error

1. Scaffold the project with the commands given below
2. Add the tailwind config including daisyui as a plugin (see the config in this repo)
3. Open the folder in vs code

## Steps taken to scaffold this project

1. `yarn create vite appName --template react`

2. `cd appName`

3. `yarn`

4. `yarn add -D tailwindcss postcss autoprefixer daisyui`

5. `npx tailwindcss init -p`

After these, I added the necessary tailwind config as can be seen in the repo.
Removing the plugin "daisyui" fixes the error.
