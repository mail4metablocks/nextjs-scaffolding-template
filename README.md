# nextjs-scaffolding-template

This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app --typescript`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Next.JS Dashboard

A Next.JS boilerplate with the famous Open Source Boostrap Admin Template, [CoreUI](https://coreui.io/).

This dashboard is built with `Typescript` and implement some layouts, with [React Bootstrap](https://react-bootstrap.github.io/).

## Screenshot

### Dashboard

https://nextjs-dashboard-olive.vercel.app

[<img alt="Dashboard" width="400" src="https://user-images.githubusercontent.com/7660346/180629352-f92216e3-7cf4-4fba-92fa-089dd96b4478.png" />](https://nextjs-dashboard-olive.vercel.app)

| Mobile (collapsed)                                                                                                                                                                           | Mobile (expand)                                                                                                                                                                              |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [<img alt="Dashboard" height="278" src="https://user-images.githubusercontent.com/7660346/190973509-f681c230-54ba-4ee5-bd8c-7929ef24b6aa.png" />](https://nextjs-dashboard-olive.vercel.app) | [<img alt="Dashboard" height="278" src="https://user-images.githubusercontent.com/7660346/190973862-29c311ab-8867-4399-ad4d-01f2d073d7a2.png" />](https://nextjs-dashboard-olive.vercel.app) |

### Sample page

https://nextjs-dashboard-olive.vercel.app/pokemons

[<img alt="Sample page" width="400" src="https://user-images.githubusercontent.com/7660346/183112188-75ffbd15-e7ef-455f-994b-945df16e5846.png">](https://nextjs-dashboard-olive.vercel.app/pokemons)

### Login

https://nextjs-dashboard-olive.vercel.app/login

[<img alt="Login" width="400" src="https://user-images.githubusercontent.com/7660346/180629556-539b6157-b34f-4ecc-aed9-b34f94d5d2ef.png" />](https://nextjs-dashboard-olive.vercel.app/login)

### Register

https://nextjs-dashboard-olive.vercel.app/register

[<img alt="Register" width="400" src="https://user-images.githubusercontent.com/7660346/180629498-1b23eb9a-cfd4-4909-8c02-58eaf6b06ff5.png" />](https://nextjs-dashboard-olive.vercel.app/register)

## Getting Started

First, setup the application:

```bash
pnpm install
```

Then, run the development server:

```bash
pnpm run dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `pages/index.tsx`. The page auto-updates as you edit the file.

[API routes](https://nextjs.org/docs/api-routes/introduction) can be accessed on [http://localhost:3000/api/hello](http://localhost:3000/api/hello). This endpoint can be edited in `pages/api/hello.ts`.

The `pages/api` directory is mapped to `/api/*`. Files in this directory are treated as [API routes](https://nextjs.org/docs/api-routes/introduction) instead of React pages.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Next.JS Rendering

### Pre-rendering

By default, Next.js pre-renders every page. This means that Next.js generates HTML for each page in advance, instead of having it all done by client-side JavaScript. Pre-rendering can result in better performance and SEO.

### SSR: Server-side rendering

Next.js will pre-render this page on **each request** using the data returned by `getServerSideProps`.

https://nextjs.org/docs/basic-features/data-fetching/get-server-side-props

### SSG: Static-site generation

Next.js will pre-render this page at **build time** using the props returned by `getStaticProps`.

* In development (next dev), getStaticProps will be called on every request.

https://nextjs.org/docs/basic-features/data-fetching/get-static-props

### CSR: Client-side rendering

If done at the page level, the data is fetched at runtime, and the content of the page is updated as the data changes. When used at the component level, the data is fetched at the time of the component mount, and the content of the component is updated as the data changes.

It is **highly recommended** to use [SWR](https://swr.vercel.app/) if you are fetching data on the client-side. It handles caching, revalidation, focus tracking, refetching on intervals, and more.

https://nextjs.org/docs/basic-features/data-fetching/client-side

### ISR: Incremental Static Regeneration

Next.js allows you to create or update static pages **after you’ve built** your site.

To use ISR, add the `revalidate` prop to `getStaticProps`.

https://nextjs.org/docs/basic-features/data-fetching/incremental-static-regeneration

## Installed Packages

1. [Redux](https://redux.js.org/tutorials/fundamentals/part-1-overview)
   1. [React redux](https://react-redux.js.org/introduction/getting-started)
   2. [Redux toolkit](https://redux-toolkit.js.org/tutorials/quick-start)
2. [Axios](https://github.com/axios/axios)
3. [React-bootstrap](https://react-bootstrap.github.io/)
4. [Immer](https://github.com/immerjs/immer)
5. [react-fontawesome](https://fontawesome.com/docs/web/use-with/react/)
   1. https://fontawesome.com/docs/web/use-with/react/use-with#next-js
   2. https://fontawesome.com/docs/web/use-with/react/add-icons#dynamic-icon-importing
6. [SWR](https://swr.vercel.app/)
7. [Eslint](https://eslint.org/)
   1. https://github.com/typescript-eslint/typescript-eslint
   2. https://github.com/jsx-eslint/eslint-plugin-react
   3. https://reactjs.org/docs/hooks-rules.html#eslint-plugin
   4. https://www.npmjs.com/package/eslint-config-airbnb
   5. https://www.npmjs.com/package/eslint-config-airbnb-typescript
   6. https://github.com/prettier/eslint-config-prettier
8. https://react-typescript-cheatsheet.netlify.app/docs/basic/getting-started/function_components/
