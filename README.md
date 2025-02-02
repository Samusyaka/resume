**Do you have any questions about GraphQL, TypeScript, or React?**

I'm happy to assist you via Remotehour. Feel free to call me if I'm online → \

[![CircleCI](https://circleci.com/gh/acro5piano/resume/tree/master.svg?style=svg)](https://circleci.com/gh/acro5piano/resume/tree/master)

# Resume

Resume of Ssamus, built with Webpack + Pug + Postcss.

We can create static website really easilly with Netlify. Thanks!!



![screenshot]

Why I created this repository: https://dev.to/acro5piano/5-reasons-why-git-based-resume-is-awesome-127

# Getting started

After checking out the repo, run:

```
yarn install
yarn start
```

open http://localhost:3000 and you can see my resume.

# Write your resume with this template

Feel free to write your resume with this template, if you are odd enough to do so.

- `src/app.postcss` is for css
- `src/index.pug` is for template
- If you want to write your resume with sass, just add `sass-loader`

# Internationalization

Unfortunatelly, we only have really legacy option to this setting.

To create Japanese resume, `HtmlWebpackPlugin` in `webpack.config.js` like this:

```
  plugins: [
    new HtmlWebpackPlugin(
      {
        template: './index.ja.pug',
        filename: 'index.html',
        inject: false
      }
    )
  ]
```

# Screenshot

To take a screenshot, just run

- `yarn build:html`
- `yarn screenshot`

This runs your Chrome headlessly and take an image.

# Production build

To build all assets, run:

```
yarn build
```

This does:

- Bundle files with Webpack production mode
- Take screenshot as `png` and `pdf`

# Netlify

Soon

# TODO

- [x] Add script for taking screenshot.
- [x] Create GitHub page or something to render this as actual web page. → netlify
- [x] Add script for build. Generate multilingual PDF to `/dist`.
- [ ] Page too big to fit A4. Time to divide.
- [ ] Use React.js or Vue.js for template rendering. This is for HMR and scoped CSS and internationalization.
- [ ] Add ESLint for stability.
- [ ] Add Flow for type-safe and null-safe.
- [ ] Internationalization. currently I need `en` and `ja`. For the time being create `index.ja.pug`.
- [ ] `screenshot` command for all languages.

# Contribution

I am not a native English speaker, so if you find something wrong, please create an issue or send a pr.

Thanks in advance.
