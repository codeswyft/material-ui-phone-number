# codeswyft-material-ui-phone-number

This project is a fork of https://github.com/alexplumb/material-ui-phone-number

We had trouble with using that repo in a Gatsby (SSR) setup. We found that the `npm run build` command needed to be run and the resulting `dist/index.js` included in the repo.

That is currently the only difference between this package and the original.

The reason we published this to NPM was because we were struggling with some GitHub Actions issues. For a while, everything worked fine when we simply listed our dependency to point at the repo:

```
"material-ui-phone-number": "https://github.com/codeswyft/material-ui-phone-number.git",
```

But now it seems GitHub actions aren't able to access that repo.
We wanted to see if publishing it to NPM would get past that problem. It does. There are probably better ways to solve it. But here we are, it works, and we're moving on.
