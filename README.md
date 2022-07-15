# Reproducing Yarn PnP TailwindCSS Intellisense Bug

## Steps to reproduce the error

If you have installed `daisyui` in any project with yarn v3, you won't be able to reproduce the issue.
I don't know how to clean the packages or  where yarn plug'n'play saves them.

1. Clone this repo
2. Run `yarn` inside of the folder
3. Open the folder in vs code.


## Steps taken to scaffold this project

1. `yarn create vite appName --template react`

2. `cd appName`

3. `yarn`

4. `yarn add -D tailwindcss postcss autoprefixer daisyui`

5. `npx tailwindcss init -p`

After these, I added the necessary tailwind config as can be seen in the repo.
Removing the plugin "daisyui" fixes the error.
