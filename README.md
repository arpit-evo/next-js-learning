# next-js-learning

## What is next js?

- framework that uses react and use for fullstack application

### Main Features

- routing based on page directory.
- support both server side rendering and client side rendering
- Support custom styling using tailwind css.
- simplify data fetching using fetch api and it supports memoization, data caching and revalidation

## getting started

- command for initialize next project:

```bash
npx create-next-app@latest
```

```after running command
What is your project named? my-app
Would you like to use TypeScript? No / Yes
Would you like to use ESLint? No / Yes
Would you like to use Tailwind CSS? No / Yes
Would you like to use `src/` directory? No / Yes
Would you like to use App Router? (recommended) No / Yes
Would you like to customize the default import alias (@/*)? No / Yes
What import alias would you like configured? @/*
```

### Folder Structure

- it has `src` as root but some times it has `app` folder as root.
- Routing depends on Folder structure of file.
- If we give folder name `chai` then in app it is called as `/chai` routes.
- each folder has `page.tsx` file for rendering content on that route and it might have it's own `layout file`.

```bash
my-nextjs-app/
├── public/
│   ├── images/
│   └── ...
├── src/
│   ├── app/
│   │   ├── global.css
│   │   ├── layout.tsx
│   │   └── page.tsx
│   │   ├── chai/
│   │   └── page.tsx
│   └── ...
├── .eslintrc.json
├── .gitignore
├── next-env.d.ts
├── next.config.mjs
├── package.json
├── postcss.config.mjs
├── README.md
├── tailwind.config.ts
└── tsconfig.json
```

- we can not use ant react hooks or state management directly in nextjs.
- But we can add `'use client'` on top of file so we can use hook in file.
