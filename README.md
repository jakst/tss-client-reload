# Tanstack Solid Start - Client navigation breaks with custom client.tsx

**To reproduce**

1. `pnpm install && pnpm dev`
2. Open app in browser. Navigate around. Notice all navigations go to the server.
3. Delete the file `./src/client.tsx` and restart the dev server
4. Repeat step 2, and notice that client navigation works again.

I suspect hydration is completely broken, but client navigation is the most directly visible issue.
