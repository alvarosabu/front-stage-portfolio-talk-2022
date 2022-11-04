---
# try also 'default' to start simple
theme: penguin
layout: text-image
colorSchema: light
media: 'http://www.blogcdn.com/es.engadget.com/media/2011/12/it-crowd-moss.jpg'
themeConfig:
  logoHeader: https://res.cloudinary.com/alvarosaburido/image/upload/v1666359605/as-portfolio/Pixel_Avatar_lhbjva.png
  eventLogo: 'https://media-exp1.licdn.com/dms/image/C4E0BAQElQZVuvPqSGg/company-logo_200_200/0/1645085342263?e=1674691200&v=beta&t=sa9vm9bOmITbvljQpb9HHBEf4S6BRlETUOrifxHzJ2I'
  eventUrl: 'https://frontdevstage.com/'
  twitter: '@alvarosabu'
  twitterUrl: 'https://twitter.com/alvarosabu'
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: false
css: unocss
drawings:
  persist: false

---
# This is Moss

A fullstack developer working at 'Reynholm Industries'

---
layout: text-image
reverse: true
media: https://img.buzzfeed.com/buzzfeed-static/static/2022-01/10/23/asset/c48c64da9172/sub-buzz-739-1641855695-5.jpg?crop=1428:795;0,49
---
# This is his boss Douglas

And he just got a juicy business deal 🤝 with a Software Company to use their **monolithic tech stack** for their websites.

---

**Moss** is condeem to use this tech stack for the next 3 years. He spends most of his time trying to make it work.

![Moss](https://media4.giphy.com/media/dbtDDSvWErdf2/giphy.gif?cid=790b761180bac36985be58ff26df83e1512a40d5de26fc4e&rid=giphy.gif&ct=g)

He would love to use a `modern tech stack`, go headless, but he is stuck with this one.

---
layout: text-image
media: https://media2.giphy.com/media/ghutdpgRkhkxq/giphy.gif?cid=ecf05e47avwg9gy6sd9ldbjjjcutnwg3j8ad2pqe27uaxni0&rid=giphy.gif&ct=g
---
**Moss** is frustrated and losing motivation.



---

# Sounds familiar right?

<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>

PD: Any resemblance with a real real-life is purely coincidental 🙄

---
layout: intro
---
# ~~Create a modern static portfolio~~
## Let's help Moss to create a modern static portfolio
---

# Why a static generated portfolio?

- It's the best side project you can do to learn a **new tech stack**
- **Moss** will be able to use <a href="https://v3.nuxtjs.org/" target="_blank"><logos-nuxt-icon mr-1 />Nuxt</a> and <a href="https://vitejs.dev/" target="_blank"><logos-vitejs mr-2 />Vite</a> to create a modern static portfolio
- **Moss** will be able to use a headless CMS like <a href="https://www.storyblok.com/"><logos-storyblok-icon /> Storyblok</a> to manage his content
- **Moss** will learn about Rendering modes and why **SSG** (static site-generation) is the best option for his portfolio
- Maybe **Moss** gets enough knowledge to propose a change in his company
- Or he can use it as a fancy online CV
- It can open **Moss** the door to **better job opportunities**

<!--
Mention the anecdote that Porsche Digital decided to hire me after seeing my portfolio
-->

---

# What we are going to do

1. Create a new Nuxt project with Vite ⚡️
2. Setup the basics 😎
3. Create a new space at Storyblok 🪐
4. Connect Storyblok to Nuxt using the official SDK
5. Create the components aka "bloks" 🧱
6. Fetch projects and articles from Storyblok
7. Rich Text 🤑
8.  Generate static pages

---
layout: text-window
---
# My Portfolio

Check it here 👉 <a href="https://next.alvarosaburido.dev" target="_blank">next.alvarosaburido.dev</a>

::window::

![](https://res.cloudinary.com/alvarosaburido/image/upload/v1666364033/next.alvarosaburido.dev__hwiagl.png)

---
layout: text-image
media: https://i.ytimg.com/vi/PkdY8vfNxQs/maxresdefault.jpg
---

# Nuxt v3

It's a progressive framework that allows you to create **static sites**, **server-rendered apps**, and **SPA** using Vue 3, Composition API, and Vite.

> And it's all about DX (Developer Experience) 🤩

Docs: <a href="https://v3.nuxtjs.org/" target="_blank">v3.nuxtjs.org</a>

<!--
Gotta warn you, is awesome
-->
---
layout: text-window
---
# New project

Open a terminal (if you're using [Visual Studio Code](https://code.visualstudio.com/), you can open an integrated terminal) and use the following command to create a new starter project:

::window::

```bash
npx nuxi init moss-portfolio

pnpm dlx nuxi init moss-portfolio
```
---

![](/nuxt-project-created.png)

---
layout: text-image
reverse: true
media: '/nuxt-structure.png'
---

# Structure

- `layouts` Ideal for extracting common UI or code patterns into reusable layout components.
- `pages` The pages directory contains your application views and routes. The framework reads all the `*.vue` files inside this directory and creates the router of your application.
- `components` The components directory contains your Vue.js Components.

---
layout: two-cols
---
App.vue 

```vue
<template>
  <div>
    <NuxtLayout>
      <NuxtPage />
    </NuxtLayout>
  </div>
</template>
```

And this is how the `default.vue` layout looks like:

```vue
<template>
  <div>
    <TheToolbar />
    <slot />
  </div>
</template>
```
::right::

![](/localhost.png)

---
layout: text-image
reverse: true
media: https://a.storyblok.com/f/88751/1596x1058/9065d0b0ed/visual-editor.png/m/1400x0/
---

# Storyblok

Storyblok is a user friendly and powerful headless CMS. The visual editor helps you to build pages with a few clicks and the time to market shrinks dramatically.

> And it's all about DX (Developer Experience) 🤩

Docs: <a href="https://www.storyblok.com/docs/guide/getting-started#nuxtjs-example" target="_blank">Storyblok</a>

<!--
Gotta warn you, is awesome
-->
---
layout: text-image
media: '/public/storyblok-new-space.png'
---
# New space

The first step on your Storyblok journey is either [signing up for Storyblok](https://app.storyblok.com/#!/signup), or (if you already have an account) logging in. Once you are logged in, you can create a new space.


---
layout: text-window

---
# @storyblok/nuxt SDK

The official Storyblok SDK for Nuxt.

```bash
pnpm add @storyblok/nuxt -D
```
Add following code to modules section of `nuxt.config.js` and replace the accessToken with API token from Storyblok space.

<div class="bg-yellow-200 mt-4 rounded-md text-sm text-yellow-600 p-4 flex items-center">
<mdi-alert mr-2 />
Use process.env.STORYBLOK_API to save your access token and don't push it to the repo.
</div>

::window::

```typescript
import { defineNuxtConfig } from "nuxt";

export default defineNuxtConfig({
  modules: [
    ["@storyblok/nuxt",
     { 
        accessToken: process.env.STORYBLOK_API_TOKEN,
        useApiClient: true
     }
    ]
    // ...
  ]
});
```
---
layout: text-window

---
# Set up the visual editor

Navigate to Settings > Visual Editor and set the location to `https://localhost:3000/` which correspond to our local development server.

Visual editor needs `https` to work properly. To enable it with nuxt just create add to your `package.json`:

```json
"scripts": [
  "dev": "nuxt dev --https"
]
```


::window::

![Storyblok New Page](/public/visual-editor-setup.png)

---
layout: text-window

---
# Add a page

Navigate to the Content on the sidebar menu of you Storyblok space and create a new page if it's not created already.

<div class="bg-yellow-200 rounded-md text-sm text-yellow-600 p-4 flex items-center">
<mdi-alert mr-2 />
Make sure `Content Type` is set to `Page`.
</div>

::window::

![Storyblok New Page](/public/storyblok-new-page.png)

---
layout: text-window
reverse: true
---
# Home Page

This will change the `Real Path` slug to `/` to match with the default Nuxt route.

Yo can do this by open the `Entry configuration` modal.

Click save and voilá! 🎉

::window::

![Storyblok New Page](/home-page-real-path.png)
---

![Storyblok Home visual editor](/home-visual-editor.png)

---
layout: text-image
media: '/bloks.png'
---

# Bloks

Imagine that your website is a lego set. 

Echoing the lego metaphor, we call the individual pieces of your website **bloks**. 

You can add, remove, and rearrange them to create your own unique website.

---
layout: text-image
media: '/create-new-blok.png'
---

# Create a blok

Navigate to `Block Library` on the sidebar menu of you Storyblok space and create a new blok.

We are gonna build a **Hero component**, so let's name it `Hero` and set as **Nesteable Blok**

---
layout: text-image
reverse: true
media: '/add-fields-to-hero.png'
---

# Add fields

Next, we need to add some fields to our blok. Storyblok makes it easy to add them after creating the blok, just type the name of the field, select the type and click on `Add`.

For this example, we are gonna add a `Title`, `Media` and `Text`.

---
layout: text-image
reverse: true
media: '/field-types.png'
---

# Field types

Storyblok counts with a lot of field types, but for this tutorial such as:

- **Text** - A simple text field.
- **Assets** - A field to upload images or files.
- **Link** - A field to link to other pages or external websites.
- **Rich Text** - A field to add rich text content.
  
---
layout: two-cols
---

# Add blok to page

Now that we have our blok created, we can add it to our home page.

![Home add new blok](/home-add-new-blok.png)

::right::
![Hero Content](/hero-content.png)

Add a fancy title and some text to your blok and click on `Save`.

---
layout: text-image
reverse: true
media: '/upload-hero-media.png'
---

# Add and Image

Storyblok V2 comes with an amazing Asset Manager.

Also has a built-in image editor that allows you to crop, resize, and optimize your images.

Add it to our hero `Media` field and click on `Save`.
---
layout: new-section
---

# You're probably wondwerin' 

![But](/moss-confused.png)

---
layout: text-image
media: '/storyblok-folder.png'
---

# Storyblok folder

You can just place all the bloks on the ~/storyblok directory and will be discovered "automagically".

We need to create 2 Vue components:
- One for the `Page` content type
- One for our `Hero`

---
layout: text-window
---
# Page.vue

This is the component responsible of rendering the page content and all the bloks within it.

We will use `<StoryblokComponent />` component to render the bloks. Think of it as a `<component :is="blok.component" />` but with Storyblok magic.

::window::
```vue
<script setup lang="ts">
  defineProps<{ blok: Object }>();
</script>

<template>
  <div v-editable="blok">
    <StoryblokComponent
      v-for="inblok in blok.body"
      :key="inblok._uid"
      :blok="inblok"
    />
  </div>
</template>
```

---
layout: text-window
---
# Hero.vue

This is the component responsible of rendering the Hero blok.

```json
{
  "_uid": "f2599984-d586-4380-9e5d-b12831146e0e",
  "text": "And my page is flippin' awesome",
  "media": {
    "id": 6201216,
    "alt": "Moss Pixel Art Avatar",
    "filename": "https://a.storyblok.com/f/179952/1024x768/4cc45ffb63/moss-hero.png",
    "copyright": "",
    "fieldtype": "asset",
    "is_external_url": false
  },
  "title": "Hi I'm Moss",
  "component": "hero",
}
```

::window::

```vue
<script setup lang="ts">
  defineProps<{ blok: Object }>();
</script>

<template>
  <div v-editable="blok" 
      class="grid grid-cols-2 gap-8 container mx-auto"
    >
    <img 
      :src="blok.media.filename" 
      :alt="blok.media.alt" 
      class="w-full" 
    />
    <div>
      <h1 class="text-4xl font-bold">{{ blok.title }}</h1>
      <p class="text-xl">{{ blok.text }}</p>
    </div>
  </div>
</template>
```
---
layout: text-window
---

# Composable to fetch Stories

We need to create a composable under `composables` directory call `useStories.ts` to fetch the stories from Storyblok using the SDK.

A good trick is to set the `version` to `draft` when in development mode and `published` when in production mode.

::window::

```ts
export type StoryVersion = "draft" | "published";

export interface StoriesConfig {
  version: StoryVersion;
}

export const storiesConfig: StoriesConfig = {
  version: 'draft',
};

export function useStories() {
  async function getStory(id = "home") {
    const story = 
      await useAsyncStoryblok(id, storiesConfig);

    return story;
  }

  return {
    getStory,
  };
}
```
---
layout: text-window
reverse: true
---

# Home page

In our home page component `index.vue` we need to fetch the story and pass it to the `Page` component.

But no worries, you can use <StoryblokComponent /> and pass the `content` of the page.

::window::

```vue
// pages/index.vue

<script setup lang="ts">
const { getStory } = useStories();

const story = await getStory("home");
</script>
<template>
  <main role="main">
    <StoryblokComponent 
      v-if="story" 
      :blok="story.content" 
    />
  </main>
</template>
```

---
layout: new-section
---

# Tadaaaaaaa

![Tada](/home-page.png)

---
layout: text-image
reverse: true
media: /portfolio.png
---

# Portfolio

We are gonna create a `portfolio` page to show all the projects we have.

Then we are gonna create a `Project` blok to show the details of each project.

---
layout: text-image
media: /create-portfolio-folder-2.png
---
# Create a new Portfolio folder

On our Storyblok dashboard, navigate to `Content` and create a new folder called `Portfolio`.

![Create a new Portfolio folder](/create-portfolio-folder.png)

---
layout: text-image
reverse: true
media: /create-portfolio-page.png
---
# Create a new Portfolio page

Create a new page called `Portfolio` inside the new folder and add  `Page` as content type.

<div class="bg-yellow-200 rounded-md text-sm text-yellow-600 p-4">
<mdi-alert mr-2 />
Make sure to check <strong>Define as root for the folder.</strong> to make the slug be "/"
</div>

---
layout: text-image
media: /create-first-project.png
---
# Create your first project

Create a new story inside the `Portfolio` folder and add new  `Project` content type if it wasn't being created before.

You can see how the name is being used to create the slug.

---
layout: text-image
reverse: true
media: /project-fields.png
---
# Project content-type fields

Open the `Block library` (you can open it from the Project visual editor as well) and add the following fields:

- **Media**: The main thumbnail of the project (Asset)
- **Excerpt**: A short description of the project (Text)
- **Content**: The content of the project (Rich text)

---
layout: text-image
media: /first-project.png
---
# Fill the project fields

🤓

---
layout: text-image
reverse: true
media: /nuxt-portfolio-dirs.png

---

# Nuxt structure for Portfolio

To achieve it we will create a `portfolio` folder under `pages`.

The main page `/porfolio` will be `index.vue`,  and the project page will be `[slug].vue`.

For more information about dynamic routes in Nuxt check [this](https://v3.nuxtjs.org/guide/directory-structure/pages#dynamic-routes) out.

---
layout: text-window
---
# Portfolio Page

On our `portfolio/index.vue` we need to fetch the content of the `Portfolio` Story to show the title on the page and get the list of projects to show.

::window::

```vue
<script setup lang="ts">
const { getStory } = useStories();

const story = await getStory("portfolio");
</script>

<template>
  <main role="main">
    <header class="mx-auto container my-24">
      <h1 class="text-4xl font-bold">{{ story.name }}</h1>
    </header>
    <section class="mx-auto container">
      // ... Project list is gonna be here
    </section>
  </main>
</template>
```

---
layout: text-window
---
# Portfolio composable

But first, we need a way to fetch all the projects from Storyblok.

We are gonna create a new composable called `usePortfolio.ts` under `composables` directory.

<div class="bg-yellow-200 rounded-md text-sm text-yellow-600 p-4">
<mdi-alert mr-2 />
is_startpage: false is to make sure we are not fetching the Portfolio page itself.
</div>

::window::

```ts
import { useStoryblokApi } from "@storyblok/vue";

const state = reactive({
  projects: [],
});

export function usePortfolio() {
  const storyapi = useStoryblokApi();

  async function fetchProjects() {
    const { data } = 
      await storyapi.get("cdn/stories/", {
        ...storiesConfig,
        starts_with: "portfolio/",
        is_startpage: false,
      });
      state.projects = data.stories;
  }

  return {
    ...toRefs(state),
    fetchProjects,
    fetchProjectBySlug,
  };
}
```
---
layout: text-window
---

# Fetching project on portfolio page

Using the composable we just created, we can fetch the projects async and wait for the state to be updated to show a list of projects using a grid.

`NuxtLink` is used to create a link to the project single page.

Nuxt have an excelent module called [NuxtImage](https://v1.image.nuxtjs.org/components/nuxt-img) to handle images, we are gonna use it to show the project thumbnail.

::window::

```vue
<script setup lang="ts">
...
const { fetchProjects, projects } = usePortfolio();

await fetchProjects();
</script>
<template>
...
  <NuxtLink
    v-for="project in projects"
    :key="project.id"
    :project="project"
    class="bg-lime-100 shadow-lg rounded-lg overflow-hidden"
    :to="`/portfolio/${project.slug}`"
  >
    <NuxtImg
      class="w-full aspect-video"
      :src="project.content.media.filename"
      format="webp"
    />
    <div class="p-4">
      <h3>{{ project.name }}</h3>
      <p>{{ project.content.excerpt }}</p>
    </div>
  </NuxtLink>
...
</template>

```
---
layout: text-image
media: /list-of-projects.png
---
# List of projects

If we go to our `Storyblok visual editor` on the Portfolio page, we can see the list of projects we have created.

---
layout: text-image
reverse: true
media: /new-project-2.png
---
# Add second project

Without leaving that same page, we can create a new project and add it to the list.

---
layout: text-window
---
# Project single Page

On our `portfolio/[slug].vue` we need to add a fetchProjectBySlug to the composable and pass the `route` param slug.

```ts
async function fetchProjectBySlug(slug: string): Promise<any> {
  const { data } = 
    await storyapi.get("cdn/stories", {
      ...storiesConfig,
      starts_with: "portfolio/",
      // Prepend */ to match with the first part of the full_slug
      by_slugs: "*/" + slug,
    });
  const story = data.stories[0];
  return story;
}
```

::window::

```vue
<script setup lang="ts">
const route = useRoute();

const { fetchProjectBySlug } = usePortfolio();

const story = 
  await fetchProjectBySlug(route.params.slug as string);
</script>

<template>
  <div class="mx-auto container px-4">
    <header class="my-24">
      <NuxtImg
        class="w-full aspect-video"
        :src="story.content.media.filename"
        format="webp"
      />
      <h1 class="text-4xl font-bold">{{ story.name }}</h1>
    </header>
  </div>
</template>
```

---

# Rendering rich text

To render the rich text we are gonna use the `renderRichText` utility from Storyblok inside a `computed` property.

```ts
const resolvedRichText = computed(() => renderRichText(story.content.content));
```

And then we can use it on the template.

```vue
<template>
  <div v-html="resolvedRichText" class="prose" />
</template>
```

--- 

![](/rich-text-rendered.png)

--- 
layout: text-image
media: /SSG.png
---
# Static Site generation (SSG)

Static site generation (SSG) pre-renders routes of your application at build time so you can easily deploy it in your static hosting provider.

More tasty info [here](https://v3.nuxtjs.org/guide/concepts/rendering/)



--- 
layout: two-cols
---
# Let's go full static

To generate the project statically we need to run `nuxt generate` and then deploy the `dist` folder to a static hosting service.

We are gonna use [Netlify](https://www.netlify.com/) to deploy our site.

```toml
[build.environment]
  NODE_VERSION = "16"
[build]
  command = "pnpm run generate"
[[redirects]]
  from = "/*"
  to = "index.html"
  status = 200
```

Push to Github and deploy.

::right:: 

Remember to add an Environment variable with you Storyblok API token in Netlify

![](/netlify-env-variable.png)

--- 
layout: text-window
---

# Wait, there is no content in prod

![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcShXyXTcxKnl10_mhbJEdDn0luouXZOzgc0FHVDqVDi8EVZOvS2ybfUfgzj_piumHmmgqE&usqp=CAU)

::window::

<iframe src="https://moss-portfolio.netlify.app/" width="100%" height="400"></iframe>

--- 
layout: text-image
media: /we-need-to-publish.png
---

# We need to publish all the stories

We need to publish all the stories to make them available in production.

![](/publish-all.png)

---
layout: text-window
---
# Using the head

Nuxt provides the `useHead` composable to add and customize the head properties of individual pages of your Nuxt app. It uses `@vueuse/head` under the hood.

For an extend explanation on SEO and Meta refer to the [Nuxt docs](https://v3.nuxtjs.org/getting-started/seo-meta/)

::window::

```typescript
useHead({
  title: story.name,
  meta: [
    {
      hid: "description",
      name: "description",
      content: story.content.excerpt,
    },
    {
      hid: "keywords",
      property: "keywords",
      keywords: story.tag_list.join(", "),
    },
    // og
    {
      hid: "og:description",
      property: "og:description",
      content: story.content.excerpt,
    },
    {
      hid: "og:title",
      property: "og:title",
      content: story.name,
    },
    {
      hid: "og:image",
      property: "og:image",
      content: story.content.media?.filename,
    },
    {
      hid: "og:image:alt",
      property: "og:image:alt",
      content: story.content.media?.alt,
    },
  ],
});
```
--- 
layout: text-image
media: /prod.png
---

# Summary

- Moss had the oportunity to learn about Nuxt 3 and Storyblok
- Moss can easily add new projects to the portfolio
- Moss is happy again

![](https://media.giphy.com/media/e7QQ9Kawb0OTJkTM1w/giphy.gif)

---

# Next steps 💡

- Optimize image sizes 🏎
- Create a blog section with a similar structure
- Add Categories to projects and filter them
- Create a contact form with netlify forms
- Share it with the world 🌎

--- 
layout: text-window
---

# Resources 📚

Repo available on Github [alvarosabu/moss-portfolio](https://github.com/alvarosabu/moss-portfolio)

[Nuxt 3](https://v3.nuxtjs.org/)

[Storyblok Nuxt SDK](https://github.com/storyblok/storyblok-nuxt)

Sushi App Recipe App [playlist](https://www.youtube.com/playlist?list=PLi-X1Ojrrmi_MxYRcGIL0jpcStKMI8Lma) 

The Storyblok Nuxt Ultimate [Tutorial](https://www.storyblok.com/tp/add-a-headless-CMS-to-nuxt-3-in-5-minutes)

::window::

<iframe width="415" height="250" src="https://www.youtube.com/embed/videoseries?list=PLi-X1Ojrrmi_MxYRcGIL0jpcStKMI8Lma" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

---
layout: presenter
eventLogo: 'https://img2.storyblok.com/352x0/f/84560/2388x414/23d8eb4b8d/vue-amsterdam-with-name.png'
eventUrl: 'https://vuejs.amsterdam/'
twitter: '@alvarosabu'

twitterUrl: 'https://twitter.com/alvarosabu'
presenterImage: 'https://res.cloudinary.com/alvarosaburido/image/upload/v1666351649/b_w_egfb4v.png'
---
# Alvaro Saburido

FE Tech Lead Engineer at <a  href="https://bcn.porsche.digital/en/" favicon="https://www.google.com/s2/favicons?domain=porsche.com" ><simple-icons-porsche mr-1/>Porsche Digital</a>

- Barcelona, Spain 🇪🇸
- <a href="https://www.storyblok.com/"><logos-storyblok-icon /> Storyblok</a> Ambassador
- I often write at <a href="https://dev.to/alvarosaburido"> dev.to/@alvarosabu</a>
- Creating content on <a href="https://www.youtube.com/channel/AlvaroDevLabs" ><logos-youtube-icon mr-1 />AlvaroDevLabs</a>
- Blog & Portfolio <a href="https://alvarosaburido.dev">alvarosaburido.dev</a>
- Say hi at <a href="https://twitter.com/alvarosabu"><logos-twitter mr-1 />@alvarosabu</a>

---
layout: new-section
---

# Thank you 🙏

![](https://media.giphy.com/media/28HuTvEHje7v1ngGAm/giphy.gif)
---