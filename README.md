# No Accessor Attempt to Reproduce

A slack user reports that by following these steps:

1. `npx graphweaver@latest init`
2. select REST-Backend
3. Copy person.ts file from git repo
4. Copy vehicle.ts file from repo
5. Copy utils.ts file from repo
6. Update index.ts file(s) where required
7. pnpm i and pnpm start

They get the error `Error: Attempting to run a find on a Rest Backend Provider that does not have an accessor.`.

I followed these steps, and the result is in this repo, which works for me.

Things to double check:

- Are the versions of the Graphweaver packages up to date?
- Are the imports of `@exogee/graphweaver-rest` in particular identical to the files in this repo?

If so, it should work for you as it does for me in this repo. If not, a diff of these files to yours should help find the source of the issue.
