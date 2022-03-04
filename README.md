<h1 align="center" style="font-size: 48px; border-bottom: 0"> Shopify Boilerplate Theme for Online Store 2.0 <img src="https://c.tenor.com/Wx9IEmZZXSoAAAAi/hi.gif" width="40" height="40" alt="hi" /> </h1>

<p align="center"> <img src="https://img.shields.io/badge/release-1.0-green" alt="release badge" /> </p>

---

Shopify Theme Boilerplate is made for saving your time while building new theme from scratch. It's based on ***TailwindCSS*** framework. It has everything in the directory, you just need to replace your content and settings as per your requirements.

## :point_down: Theme init with CLI :point_down:

Paste the code in your terminal and replace `[Your theme name]` with your actual theme name. It can be anything. :slightly_smiling_face: 

```sh
shopify theme init [Your theme name] --clone-url https://github.com/m-rokon/shopify-theme-boilerplate.git
```

Boilerplate is now cloned in your machine. Play with it, build your theme and enjoy :tada: 

<br />

<img src="https://raw.githubusercontent.com/tailwindlabs/tailwindcss/master/.github/logo-dark.svg" width="300" height="" alt="tailwind css logo" /> <br /><br />

Let's install **_tailwindCSS_** in this project. At first let's init the `package.json`. Paste the code in your terminal `npm init -y`. 

```sh
npm install -D tailwindcss postcss autoprefixer
```

Now, let's create the tailwind `config` file using terminal. It will also create the `postcss` config file, so you don't have to create it manuallay and place `autoprefixer` and `tailwindcss` plugins.

```sh
npx tailwindcss init --postcss
```

### # Configure your template paths

Add the paths to all of your template files in your `tailwind.config.js` file.

```diff
module.exports = {
  content: ["./src/**/*.{html,js}"],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

### # Add the Tailwind directives to your CSS

Now let's create a folder and name it `src` or whatever you like to name it. Then, create `tailwind.css` stylesheet and place these code in the css file.

```sh
@tailwind base;
@tailwind components;
@tailwind utilities;
```

### # Start the Tailwind CLI build process

```sh
npx tailwindcss -i ./src/tailwind.css -o ./assets/tailwind.css --watch
```

Finally, addd the newly build tailwindcss to your `theme.liquid` file. You will find the file in your `layout` directory.

So, you are done setting up the Shopify theme project with TailwindCSS. Let's dive into the code and build an amazing theme. Enjoy :tada: :love_you_gesture: 

