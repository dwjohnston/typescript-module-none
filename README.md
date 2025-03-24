Repro for this Stack Overflow question: https://stackoverflow.com/questions/79530271/typescript-module-none-does-not-error


Instructions: 

```
npm i
```

```
npx tsc
```

Observe no errors and the outputted code is CJS. 

```
npx tsc --module none --outfile dist/o.js src/index.ts
```

Observe we see an error: 

```
src/other.ts:1:17 - error TS1148: Cannot use imports, exports, or module augmentations when '--module' is 'none'.

1 export function foo() {
                  ~~~


Found 1 error in src/other.ts:1
```
