
## Build Error after integrating sentry 

Without this below module.exports, I'm able to see my logs on sentry

```bash
module.exports = {
  // https://github.com/vercel/next.js/issues/21079
  // Remove this workaround whenever the issue is fixed
  images: {
    loader: 'imgix',
    // path: '/',
    // path: 'http://localhost:3000/',
    // path: `http://{window.location.hostname}/`,
  },
}

```

But for making a build && export for production
It is throwing 

```bash
Error: Image Optimization using Next.js default loader is not compatible with next export. 
```

And please let me know how can i add dynamic url to the path? 
like,

```bash
{window.location.hostname}
```
