<script>
  import LinkButton from './LinkButton.svelte';
  import CloudMini from './icons/CloudMini.svelte';
</script>

<header class="bg-gradient-to-r from-sky-500 to-violet-400 dark:from-sky-800 dark:to-violet-800">
  <div class="px-4 py-4">
    <div class="flex w-full items-center justify-between lg:mx-auto lg:max-w-7xl">
      <div class="flex">
        <div class="flex">
          <div class="mr-2 flex items-center rounded-xl bg-white p-2 dark:bg-white/5">
            <img
              src="gulpetl.png"
              class="h-7 w-7 shrink-0 text-gray-600 dark:text-zinc-300"
              title="Application Logo"
              alt="Application Logo"
              width="28"
              height="28"
              loading="eager"
            />
          </div>
          <div
            class="inline-block h-7 py-1 font-mono text-2xl font-bold text-gray-800 dark:text-zinc-200"
          >
            gulp-etl
          </div>
        </div>

        <!-- <div class="ml-10 space-x-8 text-lg flex items-center justify-center font-medium dark:text-zinc-200">
          <div>Features</div>
          <div>Pricing</div>
          <div>Roadmap</div>
          <div>Self-hosting</div>
        </div> -->
      </div>

      <div class="space-x-4">
          <LinkButton to="https://docs.gulpetl.com">
            <CloudMini slot="icon" />
            <slot>
              <span class="hidden md:inline">View Docs</span>
              <span class="md:hidden">Get started</span>
            </slot>
          </LinkButton>
    
          <a
            href="https://github.com/gulpetl"
            target="_blank"
            rel="noreferrer"
            class="inline-block rounded-lg bg-gradient-to-b from-gray-700 to-gray-800 px-3 py-2 text-gray-100 shadow-lg transition-colors ease-in-out hover:bg-gray-100 hover:from-gray-700/90 hover:to-gray-800/90 dark:from-zinc-700 dark:to-zinc-800 dark:text-zinc-200 dark:hover:from-zinc-700/90 dark:hover:to-zinc-800/90 lg:rounded-xl lg:px-4"
          >
            <div class="flex items-center">
              <div>
                <picture>
                  <img
                    src="/GitHub-Mark-Light-64px.png"
                    class="h-5 w-5"
                    title="GitHub Invertocat Logo"
                    alt="GitHub Invertocat Logo"
                    width="20"
                    height="20"
                    loading="eager"
                  />
                </picture>
              </div>
              <div class="ml-2 block md:hidden">Source code</div>
              <div class="ml-2 hidden md:block">View on GitHub</div>
            </div>
          </a>
        </div>
      </div>
    </div>
</header>
