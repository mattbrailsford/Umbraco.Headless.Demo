# Umbraco Headless Demo - Frontend

This branch represents the frontend of the Umbraco Headless Demo and consists of a Next.js application fully configured with common features, including:

- Next.js App Router
- Optimized for SEO using Next.js's Metadata
- React Server Components (RSCs) and Suspense
- Server Actions for mutations
- Edge Runtime
- Latest fetching and caching paradigms
- Dynamic OG images
- Styling with Tailwind CSS

## Configuration

You will need to use the environment variables [defined in `.env.example`](.env.example) to configure this project. It's recommended you use [Vercel Environment Variables](https://vercel.com/docs/concepts/projects/environment-variables) for this, but a `.env` file is all that is necessary.

> Note: You should not commit your `.env` file or it will expose secrets that will allow others to control your store.

1. Install Vercel CLI: `npm i -g vercel`
2. Link local instance with Vercel and GitHub accounts (creates `.vercel` directory): `vercel link`
3. Download your environment variables: `vercel env pull`

## Running locally

```bash
npm install
npm run dev
```

Your app should now be running on [localhost:3000](http://localhost:3000/).

## Deploying

This project is designed to be deployed to [Vercel](https://vercel.com). Checkout the [Deploying to Vercel docs](https://vercel.com/docs/concepts/deployments/overview) for full details.

## Known Issues

* `Error: invariant expected app router to be mounted` or `Method expects to have requestAsyncStorage, none available`  
  If you are running this project locally on Windows and experience either of these two errors, you'll want to run the `npm` run commands thought WSL. There appear to be some issues running on Windows but running through the Linux subsystem works fine.


## License

Copyright © 2023 Umbraco A/S

This demo store is [licensed under MIT](LICENSE.md). The core Umbraco products are licensed under Umbraco's commercial license.
