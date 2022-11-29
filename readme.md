# incremental-compiler-js

incremental compiler in javascript

## status

early draft

## demo

[incremental-compiler-js demo](https://milahu.github.io/incremental-compiler-js/demo/dist/)

## documentation

see [docs/](docs/)

## install

```sh
git clone --recurse-submodules https://github.com/milahu/incremental-compiler-js
cd incremental-compiler-js
pnpm install
```

### offline demo

```sh
cd demo
pnpm install
npm run dev
```

## goals

### incremental compiler

create a prototype for an **incremental** compiler

#### example

input version 1

```jsx
function App(props) {
  return (
    <div>hello</div>
  )
}
```

input version 2

```jsx
function App(props) {
  return (
    <div>hello world</div>
  )
}
```

input difference

```diff
-    <div>hello</div>
+    <div>hello world</div>
```

## related

* [nix-eval-js](https://github.com/milahu/nix-eval-js) - nix interpreter in javascript, based on lezer-parser

## keywords

* incremental compiler in javascript
* incremental compilation in javascript
* chain of multiple compilers
* compiler pipeline
* compiler chain
* low latency
