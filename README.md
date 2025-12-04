# nextjs-lab

A lab repo for exploring nextjs.

Next.js is an open source JavaScript web framework for React that ships with a rich set of features out of the box, such as:

- server-side rendering
- static site generation
- incremental static regeneration

You need to install Node.js and npm.

Since I utilize nvm, installing the latest version of node is accomplished like this:

```shell
nvm install node
nvm alias default node
```

[Examples](https://github.com/PacktPublishing/Real-World-Next.js)

## The problem with React

By default, React runs on the client side (meaning that it runs on the web browser), so a web application written entirely with that library could negatively affect Search Engine Optimization (SEO) and initial load performance, as it takes time to be correctly rendered on screen.

Vercel came up with Next.js, which was a game changer. It provides many innovative features such as automatic code-splitting, server-side rendering, file-based routing systems, route pre-fetching, and so on.

Next.js showes how easy it should be to write universal web applications by allowing developers to write reusable code for both client and server sides and making very complex tasks effortless to implement.

Next.js follows a convention-over-configuration approach for most of its settings. In a single Next.js app, you can specify which pages shall be server-side rendered and which shall be statically generated at build time without the need to write any configuration files or anything else like that. You just have to export a specific function from your page and let Next.js do its magic.


Every server-side rendered or statically generated page will run on Node.js, so you will lose access to some browser-specific global objects such as:

- fetch,
- window, and
- document

as well as some HTML elements such as canvas.

You will always need to keep that in mind when you're writing your Nex.js pages, even if the framework provides its own way for dealing with components that must use such global variables and HTML elements.

There might be times when you want to use Node.js specific libraries or APIs, such as fs or child_process, and Next.js allows you to use them by running your server-side code on each request or at build time before sending the data to the client.

## Getting started with Next.js

Creating a new Next.js app

```shell
npx create-next-app <app-name>
```

It will install all of the required dependencies and create a couple of default pages. At this point, you can just run `npm run dev`, and a development server will start on port `3000`, showing a landing page.

Next.js will initialize your project using the Yarn package manager if installed on your machine. You can override this option by passing a flag to tell create-next-app to use npm instead:

```shell
npx create-next-app <app-name> --use-npm
```

The [Next.js examples](https://github.com/vercel/next.js/tree/canary/examples) can be used to create new projects from the examples.

```shell
npx create-next-app <app-name> --example with-docker
```


## Server-Side Rendering


## Static Site Generation

## Incremental Static Regeneration

## Native TypeScript Support

## Automatic Polyfils

## Image Optimization

## Support for internationalization

## Performance analytics






