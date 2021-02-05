# benchmarks

Benchmark tooling for the `npm` cli

### Options:

##### `manager` (alias `-m`)

Type: `Array`

Options: `all`, `npm`, `yarn`, `pnpm` ...

List of package managers to benchmark (must be npm installable strings)

##### `fixture` (alias `-f`)

Type: `Array`

Options: `all`, `angular-quickstart`, `app-large`, `app-medium`, `ember-quickstart`, `eslint-config`, `mixcreant`, `react-app`, `tsconfig`

List of fixtures to run the given benchmarks against

##### `benchmark` (alias `-b`)

Type: `Array`

Options: `all`, `clean`, `lock-only`, `cache-only`, `modules-only`, `no-lock`, `no-cache`, `no-modules`, `no-clean`

List of benchmarks to run

##### `report` (alias `-r`)

Type: `Boolean`

Generate a text report

##### `graph` (alias `-g`)

Type: `Boolean`

Generate a svg graph

### Example usage:

```bash
./benchmark.js -m all -b all -f app-large -g
```

<img src="https://github.com/larsenwork/benchmarks/raw/feature/dark-mode-support/test/alotta-files.svg" alt="" width="100%">

**Note:** Graph generation pulled from [pnpm/benchmarks-of-javascript-package-managers](https://github.com/pnpm/benchmarks-of-javascript-package-managers)
