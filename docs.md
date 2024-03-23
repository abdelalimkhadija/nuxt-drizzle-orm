## create project of nuxt with drizzle orm 
```sh
npx nux@latest init appname
```
## choose bun

## install the follwing dependencies 
```sh
bun add drizzle-orm better-sqlite3
```
## add drizzle kit also
```sh
bun add -D drizzle-kit
```
## add @types/better-sqlite3
```sh
bun add -D @types/better-sqlite3
```

## create drozzile.config.ts and insert configuration
```ts
import { Config } from 'drizzle-kit'

export default {

  schema:"./db/schema.ts",
  out: "./drizzle",
  driver:"better-sqlite",
  dbCredentials:{

    url:"./sqlite.db"
}

} satisties Config


