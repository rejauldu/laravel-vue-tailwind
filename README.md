<ul>
<li>Install laravel<br/>
<pre>
composer create-project --prefer-dist laravel/laravel laravel-vue-tailwind
cd laravel-vue-tailwind</pre>
</li>
<li>Install vue<br/>
<ul><li>
<pre>npm install vue
npm install @vitejs/plugin-vue --save-dev</pre>
</li>
<li>Update vite.config.js</li>
<li>Update app.js</li>
<li>Add App.vue</li>
<li>Update welcome.blade.php</li></ul>
<li>Install tailwind form tailwind website>framework>laravel>using vite</li>
<ul>
<li>
<pre>
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p</pre>
</li>
<li>Update tailwind.config.js's content:<br/>
<pre>
content: [
    "./resources/**/*.blade.php",
    "./resources/**/*.js",
    "./resources/**/*.vue",
  ],
</pre></li>
<li>Update ./resources/css/app.css<br/>
<pre>
@tailwind base;
@tailwind components;
@tailwind utilities;
</pre></li>
</ul>
</li>
<li>Install TypeScript:</li>
<ul>
<li><code>npm install --save-dev typescript</code></li>
<li><code>npx tsc --init</code> //Creates tsconfig.json</li>
<li>Add some code to <code>tsconfig.json</code></li>
<li>Change <code>app.js</code> &gt; <code>app.ts</code> and <code>bootstrap.js</code> &gt; <code>bootstrap.ts</code></li>
<li>Add <code>lang="ts"</code> to javascript like: <code>&lt;script lang="ts"&gt;</code></li>
<li>Change <code>export default ({</code> to <code>export default defineComponent({</code></li></ul>
<li>Install Sass</li>
<ul>
<li><code>npm install sass</code></li>
<li>Create <code>resources/sass/app.scss</code> and <code>resources/sass/_variables.scss</code></li>
<li>Add the following lines to <code>app.scss</code></li>
<pre>@tailwind base;
@tailwind components;
@tailwind utilities;
@import 'variables';
</pre>
<li>In <code>vite.config.js</code> and in view page change <code>app.css</code> to <code>app.scss</code></li>
</ul>
</ul>
