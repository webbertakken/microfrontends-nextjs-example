# Micro frontends Next.js Example


## Resources

- [Micro-frontends](https://martinfowler.com/articles/micro-frontends.html) (Martin Fowler blog) 

## Software references

- [Next.js repo with turbo](https://github.com/vercel/turbo/tree/main/examples/with-yarn)
- [Next.js Module Federation](https://github.com/module-federation/module-federation-examples/blob/master/nextjs-v13)
- [Next.js Module Federation plugin](https://github.com/module-federation/universe/tree/main/packages/nextjs-mf)

## Requirements

Must work with latest:

  - React, Next.js for rendering
  - Redux for state management

## Quests

- Is there any difficulty applying SSR (runtime) and SSG (build time) rendering strategies for both container and page?
- Derive whether a separately deployed container application is preferred or not
- Illustrate sharing both code and state between apps as well as isolated app state.
 
## Rationale

Here I'll describe the assumptions and decisions I've taken while building this example.

#### Step 1: Monorepo

For a monorepo with multiple Next.js apps, Vercel recommends using Turborepo.

This repository uses the Turborepo [example](https://github.com/vercel/turbo/tree/main/examples/with-yarn) as the basis for everything else.

#### Step 2: Rigging the application

There are a few technologies out there that allow you to create micro-frontends.

The Module Federation [plugin](https://github.com/module-federation/universe/tree/main/packages/nextjs-mf) for Next.js seems to be a solid low-code solution.

In this step I'm replacing the example apps with the ones from the Next.js Module Federation [example](https://github.com/module-federation/module-federation-examples/blob/master/nextjs-v13).


