# nuxt-layer-sample

## System Requirements

- Node.js - 18.x
- Yarn

## Library

- nuxt - 3.6.x

## Usage

```bash
# package installation
$ yarn

# nuxt-app run - http://localhost:3000, http://localhost:3000/layer1, http://localhost:3000/layer2
$ yarn workspace @nuxt-layer-sample/nuxt-app run dev

# layer1 run - http://localhost:3001/layer1
$ yarn workspace @nuxt-layer-sample/layer1 run dev

# layer2 run - http://localhost:3002/layer2
$ yarn workspace @nuxt-layer-sample/layer2 run dev
```

## Directory structure

```
├── layer-lib     Nuxt Layer for libraries
├── layer1        Nuxt Layer for /layer1
├── layer2        Nuxt Layer for /layer2
└── nuxt-app      For Nuxt launch
```

## Reference URL

- https://nuxt.com/docs/getting-started/layers
