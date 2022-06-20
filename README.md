# ts-typescript

## 1.typescript

```
yarn init -y
yarn add -D typescript
npx tsc --init
```

## edit package.json

```package.json
"scripts": {
    "start": "node src/index.js",
    "build": "tsc"
    }
```

#### 2.install nodemon ts-node for dev

```nodemon
yarn add -D ts-node nodemon
```

#### 3.create file nodemon.json

```
touch nodemon.json
```

```nodemon.json
{
    "watch": ["src"],
    "ext": "ts",
    "exec": "ts-node"
}
```

#### 4.add script to package.json

```
"scripts": {
        "start": "node src/index.js",
        "build": "tsc",
        "dev": "nodemon src/index.ts"
    },
```

#### run

```dev
yarn dev
```

<hr>

# setting vscode

#### install extensions vscode prettier

#### cmd + shift + p : >open Workspace Settings (JSON)

```setup
{
    "editor.formatOnSave": true
}
```

```
touch .prettierrc
```

#### >> .prettierrc

```prettierrc
{
    "semi": false,
    "singleQuote": true
}
```
