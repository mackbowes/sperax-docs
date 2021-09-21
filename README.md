
# Sperax Documentation Front End

This project uses Next.Js to handle routing and Static Site Generation in a React framework, giving access to easy to extend or change component based architecture. 

Add or edit `.md*` files in `/docs` to add documentation. 

Views are stored in `/pages` and automatically handle routing. `/pages/index.js` routes to `https://domain.tld/`, `pages/about.js` routes to `https://domain.tld/about`. Dead simple. 

You can add folders to `/pages` that are handled like directories - `/pages/about/index.js` also routes to `https://domain.tld/about`, `/pages/about/team.js` would route to `https://domain.tld/about/team`. Take care to avoid collisions. 

There are also dynamic routes - this is how we generate the docs from `.md*` files. They are identified by square brackets, ie `/pages/docs/[slug].js`, when hydrated by `overview.md`, would be accessible at `https://domain.tld/docs/overview`. 



## Getting Started

```
// Install packages
npm i
or
yarn add

// Start development server
yarn dev
```

## Next.JS Stuff

This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

### Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

### Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.