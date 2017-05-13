# WpDevOps Elixir Browsersync Support

First ensure, that you're WpDevOps Elixir version is up to date.


## Step 1: Install

```bash
npm install @wpdevops/elixir-browsersync --save-dev
```

## Step 2: Use It

Within your Gulpfile, add:

```js
elixir(function(mix) {
  mix.browserSync();
});
```

Once you run `gulp watch`, access your web application using port 3000 to enable browser syncing: `http://wpdevops.dev:3000`. 
If you're using a domain other than `wpdevops.dev` for local development (likely), you may pass an array of options as the first argument to the browserSync method:

```js
elixir(function(mix) {
  mix.browserSync({
    proxy: 'project.app'
  });
});
```

---

This package was originally ([laravel-elixir-browsersync-official](https://github.com/JeffreyWay/laravel-elixir-browsersync-official)) 
written by [Jeffrey Way](https://github.com/JeffreyWay)