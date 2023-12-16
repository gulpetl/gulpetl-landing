<script lang="ts">
  import FeatureItem from './FeatureItem.svelte';
  import Bolt from './icons/Bolt.svelte';
  import CircleStackOutlined from './icons/CircleStackOutlined.svelte';
  import CloudMini from './icons/CloudMini.svelte';
  import Edit from './icons/Edit.svelte';
  import DocumentDuplicateOutlined from './icons/DocumentDuplicateOutlined.svelte';
  import LinkOutlined from './icons/LinkOutlined.svelte';
  import Plugin from './icons/Plugin.svelte';
  import LinkButton from './LinkButton.svelte';

</script>

<main>
  <section
    class="flex flex-col items-center justify-center bg-zinc-900 bg-gradient-to-br 
    from-sky-500 via-violet-400 to-pink-300 px-4 py-10 pt-14 
dark:from-sky-800 dark:via-violet-800 dark:to-pink-500 md:px-20 lg:px-0 lg:pt-28"
  >
    <h1
      class="max-w-3xl text-center text-5xl font-semibold text-gray-700 dark:text-zinc-200 lg:text-7xl"
    >
      Extensible, Affordable, Performant ETL
    </h1>
    <p
      class="mt-10 max-w-2xl px-4 text-center text-lg font-light text-gray-800 dark:text-zinc-100/80 md:px-16 lg:px-0 lg:text-xl"
    >
      "Are you looking for an easy Extract Transform Load (ETL) tool? Consider Node-RED. In an
      ever-changing world of data integrations, we found Node-RED to be a low-cost, reliable, and
      secure platform that is capable of moving millions of records."" <cite> -- Ondrej Lehota, in <strong class="underline"><a target="_blank" href="https://developer.ibm.com/articles/implementing-etl-flows-with-node-red">an article</a></strong> that inspired us to
      bring Node-RED to gulp-etl
      </cite>
    </p>
    <div class="w-full text-right">
    <p class="w-auto mt-1 max-w-2xl px-4 text-right text-lg font-light text-gray-800 dark:text-zinc-100/80 md:px-16 lg:px-0 lg:text-xl">
      
    </p>
  </div>
    <br><br>
    <h1
      class="max-w-3xl text-center text-5xl font-semibold text-gray-700 dark:text-zinc-200 lg:text-7xl"
    >
      Gulp + Singer...
    </h1>
    <p
      class="mt-10 max-w-2xl px-4 text-center text-lg font-light text-gray-800 dark:text-zinc-100/80 md:px-16 lg:px-0 lg:text-xl"
    >
      Gulp-etl is built around a battle-tested tool for composing code blocks into build pipelines and a popular open-source ETL framework.
    </p>

    <div class="mt-12">
      <picture class="px-8 md:px-0">
        <source
          srcset="gulpfile.png"
          media="(prefers-color-scheme: dark) and (min-width: 1024px)"
        />
        <source srcset="gulpfile.png" media="(min-width: 1024px)" />
        <source
          srcset="gulpfile.png"
          media="(prefers-color-scheme: dark) and (min-width: 768px)"
        />
        <source srcset="gulpfile.png" media="(min-width: 768px)" />
        <source
          srcset="gulpfile.png"
          media="(prefers-color-scheme: dark) and (max-width: 768px)"
        />
        <source srcset="gulpfile.png" media="(max-width: 768px)" />
        <img
          src="/gulpfile.png"
          title="gulp-etl code"
          alt="gulp-etl code"
          loading="eager"
          width="800"
          height="600"
        />
      </picture>
    </div>

    <br><br>
    <h1
      class="max-w-3xl text-center text-5xl font-semibold text-gray-700 dark:text-zinc-200 lg:text-7xl"
    >
      ...now with Node-RED!
    </h1>
    <p
      class="mt-10 max-w-2xl px-4 text-center text-lg font-light text-gray-800 dark:text-zinc-100/80 md:px-16 lg:px-0 lg:text-xl"
    >
      The power, speed and convenience of gulp-etl, now all visual and low-codey.
    </p>

    <div class="mt-12">
      <picture class="px-8 md:px-0">
        <source
          srcset="node-red-tap-csv.png"
          media="(prefers-color-scheme: dark) and (min-width: 1024px)"
        />
        <source srcset="node-red-tap-csv.png" media="(min-width: 1024px)" />
        <source
          srcset="node-red-tap-csv.png"
          media="(prefers-color-scheme: dark) and (min-width: 768px)"
        />
        <source srcset="node-red-tap-csv.png" media="(min-width: 768px)" />
        <source
          srcset="node-red-tap-csv.png"
          media="(prefers-color-scheme: dark) and (max-width: 768px)"
        />
        <source srcset="node-red-tap-csv.png" media="(max-width: 768px)" />
        <img
          src="/node-red-tap-csv.png"
          title="gulp-etl in Node-red"
          alt="gulp-etl in Node-red"
          loading="eager"
          width="800"
          height="600"
        />
      </picture>
    </div>

    <div class="mt-16 flex space-x-4 px-4">
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
    


  </section>

  <section
    class="bg-gradient-to-br from-pink-100 via-violet-100 to-sky-100 px-4 pb-14 dark:from-transparent dark:to-transparent dark:py-14 lg:px-0 lg:py-14 lg:pt-8 dark:lg:py-14 xl:mx-auto"
  >
    <h2
      class="mx-auto w-fit bg-gradient-to-r from-blue-500 via-indigo-400 to-purple-500 bg-clip-text text-center text-xl font-semibold text-transparent dark:from-indigo-500 dark:via-violet-500 dark:to-purple-500 lg:text-2xl"
    >

    </h2>
    <h3 class="text-center text-3xl font-medium text-gray-700 dark:text-zinc-200 lg:text-5xl">
      Stackable, swappable, flexible; tons of tools to manage your data
    </h3>
    <div
      class="mt-10 grid grid-cols-1 gap-2 md:grid-cols-2 md:gap-4 lg:max-w-screen-xl lg:grid-cols-3 lg:gap-8 lg:px-10 xl:max-w-screen-2xl 2xl:mx-auto"
    >
      <FeatureItem
        title="Plugins/Nodes"
        description='Gulp-etl uses gulp plugins as its building blocks. Open source gulp (4000+) and gulp-etl plugins can be easily upgraded to also function as Node-RED nodes, and the core gulp-etl plugins are being upgraded.'
      >
        <Plugin slot="icon" />
      </FeatureItem>

      <FeatureItem
        title="Fast and efficient"
        description="Use Node Streams to process data of unlimited size by processing only what fits in memory."
      >
        <Bolt slot="icon" />
      </FeatureItem>

      <FeatureItem
        title="Customizable and Reusable"
        description="Use built-in and open-source (4500+) Node-RED nodes to manage data, or write small javascript snippets, or create your own reusable nodes to add new functionalities"
      >
        <Edit slot="icon" />
      </FeatureItem>
<!-- 
      <FeatureItem
        title="S3-compatible"
        description="Use your local filesystem or any S3-compatible storage of your choice"
      >
        <CircleStackOutlined slot="icon" />
      </FeatureItem>

      <FeatureItem
        title="Duplicates finder"
        description="You can easily find duplicates and nearly-identical images to keep your files organized"
      >
        <DocumentDuplicateOutlined slot="icon" />
      </FeatureItem>

      <FeatureItem
        title="Public Sharing"
        description="Share your files with your friends and colleguages"
      >
        <LinkOutlined slot="icon" />
      </FeatureItem> -->
    </div>
  </section>

</main>