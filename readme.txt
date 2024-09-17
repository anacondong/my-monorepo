ref: https://nx.dev/getting-started/tutorials/npm-workspaces-tutorial


--- run ---
npx nx run-many -t build
npx nx run-many -t typecheck

--- build ---
npx nx build @mymonorepo/demo
npx nx run-many --target=build --all --verbose

--- graph ---
npx nx graph
npx nx show project @mymonorepo/demo

--- release ---
npx nx release --first-release --dry-run

--- Start Demo project ---
npx nx serve @mymonorepo/demo
