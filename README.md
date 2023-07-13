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
</ul>