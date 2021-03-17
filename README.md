StackStorm Exchange Web Front-end
=================================

[exchange.stackstorm.org](https://exchange.stackstorm.org) is a front-end for
StackStorm Exchange, a collection of packs contributed by StackStorm users and 
engineers. 

It's a simple React app rendering [the pack index](https://github.com/StackStorm-Exchange/index);
there is no server-side to it at all, and the index is available for consumption
as a JSON file.

Just look at that page: packs, packs everywhere! Maybe it's time to go
create even more?

#### Further Reading

CI: [StackStorm-Exchange/ci](https://github.com/StackStorm-Exchange/ci).

Index: [StackStorm-Exchange/index](https://github.com/StackStorm-Exchange/index).

## Building Website

To build the website, run the commands listed below.

If you are building on windows machine  install 

```
npm install -g windows-build-tools
```

1. Install all the dependencies

```bash
npm install
```

2. Make sure linting passes

```bash
npm run lint
```

3. Build it

for linux: 

```bash
npm run build-linux
```

for windows :

```bash
npm run build-windows
```



If you want to run a development server locally, you can run:

```bash
npm run dev
```

## Deploying new versions

This website is hosted by Github Pages. When code is merged to master, if it passes linting and tests, it will
automatically get pushed to the `gh-pages` branch, and served at https://exchange.stackstorm.org/
