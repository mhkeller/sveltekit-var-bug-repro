sveltekit-var-bug-repro
===

Svelte kit throws the error `Not implemented undefined` when you use `var` in a for-loop like this:

```js
for ( var i = 0; i < 300; i += 1 ) {
	console.log(i);
}
```

Changing it to `let i = 0` solves the problem.

## Steps to reproduce

```sh
npm install
npm run dev
# navigate to localhost:3000
```

