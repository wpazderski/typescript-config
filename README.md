# typescript-config

Common [TypeScript](https://www.typescriptlang.org/) configs with strict options enabled; designed for modern projects

## Installation and usage

Start by installing this package, for example with `pnpm`:

```sh
pnpm i -D @wpazderski/typescript-config
```

Then create `tsconfig.json` file:

```jsonc
{
    "$schema": "https://json.schemastore.org/tsconfig",
    "extends": "@wpazderski/typescript-config/<CONFIG_NAME>.tsconfig.json",
    "compilerOptions": {
        /* Custom options */
    },
}
```

Replace `<CONFIG_NAME>` with chosen config (see [Available configs](#available-configs) section), for example:

```jsonc
{
    "$schema": "https://json.schemastore.org/tsconfig",
    "extends": "@wpazderski/typescript-config/baseNodeJs.tsconfig.json",
    "compilerOptions": {
        /* Custom options */
    },
}
```

## Available configs

- `base` - used as base for other configs (it can be used directly, but in most cases one of the following configs is a better choice),
- `baseNodeJs` - for general Node.js environments,
- `baseWeb` - for general web environments,
- `angular` - for Angular projects,
- `nextJs` - for Next.js projects,
- `react` - for React projects,
- `vue` - for Vue projects.

## Related projects

- [@wpazderski/prettier-config](https://github.com/wpazderski/prettier-config),
- [@wpazderski/eslint-config](https://github.com/wpazderski/eslint-config),
- [@wpazderski/playwright-config](https://github.com/wpazderski/playwright-config),
- [@wpazderski/playwright-utils](https://github.com/wpazderski/playwright-utils),
- [@wpazderski/configs-utils-example](https://github.com/wpazderski/configs-utils-example) - an example project that shows how to use all configs and utils.
