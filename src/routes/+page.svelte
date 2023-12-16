<script>
  import Header from '$lib/components/Header.svelte';
  import Content from '$lib/components/Content.svelte';

  export const prerender = true;
</script>

<svelte:head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <meta name="theme-color" content="#fff" media="(prefers-color-scheme: light)" />
  <meta name="theme-color" content="#18181b" media="(prefers-color-scheme: dark)" />
  <meta name="msapplication-TileColor" content="#603cba" />

  <link rel="icon" href="/favicon.png" />
  <title>gulp-etl</title>
</svelte:head>

<div class="flex min-h-screen w-full flex-col bg-white font-sans dark:bg-zinc-900/95">
  <Header />
  <Content />

  <footer class="bg-gray-100 pb-8 text-sm dark:bg-zinc-900">
    <p
      class="mx-4 border-t pt-8 text-gray-400 dark:border-zinc-800 dark:text-zinc-500 md:mx-8 lg:max-w-screen-xl lg:px-10 xl:max-w-screen-2xl 2xl:mx-auto"
    >
    </p>
  </footer>
</div>
