# orbitdb-lint

Linter and linting rules for [OrbitDB](https://github.com/orbitdb/orbit-db) JavaScript modules.

Uses [eslint](https://eslint.org) and [OrbitDB linting rules](https://github.com/orbitdb/eslint-config-orbitdb) to provide linting for development of [OrbitDB](https://github.com/orbitdb/orbit-db) and its modules.

## Using in your project

Install the [`orbitdb-lint`](https://github.com/haadcode/orbitdb-lint) and add the module to your project's dev dependencies:
```
npm install @orbitdb/lint --save-dev
```

This will install [eslint](https://eslint.org) (the linter), [eslint-config-orbitdb](https://github.com/orbitdb/eslint-config-orbitdb) (linting rules) and [their dependencies](https://github.com/haadcode/orbitdb-lint/blob/master/package.json#L11) to your project.


Create `.eslintrc` file in your project's root directory:
```
touch .eslintrc
```

Edit `.eslintrc` to contain:
```json
{
  "extends": ["@orbitdb/eslint-config-orbitdb"]
}
```

Add a `lint` script to your project's `package.json`:
```json
"scripts": {
  "lint": "eslint src/"
}
```

Finally, to test it all works, run the linter:
```
npm run lint
```

## Contribute

TODO

## License

[MIT](LICENSE) © 2018 OrbitDB Community