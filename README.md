# Storybook v7 & addon-svelte-csf v3 errors

This repo reproduces two errors with storybook v7 and addon-svelte-csf v3.

## First Error

To reproduce the first error, run these commands and then try to open the `Button CSF` story in storybook.
```shell
npm install
npm run storybook
```

After opening the Story `Button CSF`, there is an error shown in the browser and in the server console.

To fix this error, it seems that you just have to execute `npm i -D @storybook/client-api@next` (and restart storybook of course).

## Second Error

After installing `@storybook/client-api`, try to open the Story `Button CSF` again. The browser shows a blank screen now, but the browser console shows several error message.
