Reproduce: `npm i && npm run check`



Output:
```
.../src/App.svelte:7:11
Error: Type '{ sayHello: (name: string) => void; } & { $set?: any; $on?: any; }' is not assignable to type 'SvelteComponent<{ sayHello?: ((name: string) => void) | undefined; }, { [evt: string]: CustomEvent<any>; }, {}> & { $$bindings?: string | undefined; } & { ...; }'.
  Type '{ sayHello: (name: string) => void; } & { $set?: any; $on?: any; }' is missing the following properties from type 'SvelteComponent<{ sayHello?: ((name: string) => void) | undefined; }, { [evt: string]: CustomEvent<any>; }, {}>': $$prop_def, $$events_def, $$slot_def, $destroy (ts)
  onMount(() => {
    const mounted: MyComponent = mount(MyComponent, { target: div })
  })


====================================
svelte-check found 1 error and 0 warnings in 1 file
```