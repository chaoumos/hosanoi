---
import Layout from '../../layouts/BlogPost.astro'

export const frontmatter = {
  title: 'Welcome to hosanio',
  description: 'This is the first post on hosanio, an AI blog.',
  pubDate: '2024-07-03',
  layout: '../../layouts/BlogPost.astro'
}

const { title, description, pubDate } = frontmatter;
---

<Layout title={title} description={description}>
  <article class="prose lg:prose-xl">
    <h1>{title}</h1>
    <time>{pubDate}</time>
    <p>Welcome to hosanio, your go-to source for all things AI.</p>
    <img src="https://placehold.co/600x300.png" alt="AI Image" data-ai-hint="an abstract representation of artificial intelligence"/>
    <p>We'll be covering topics ranging from the latest breakthroughs in machine learning to the ethical implications of AI.</p>
    <p>Stay tuned for more!</p>
  </article>
</Layout>