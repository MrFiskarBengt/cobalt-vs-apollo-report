# Apollo + TypeGraphQL vs Cobalt

A self-contained report comparing two implementations of a small authenticated
application. Both APIs run on Bun and share the same data behavior. The report
covers setup, client usage, security boundaries, test evidence, and measured
startup, code generation, API, payload, and browser-flow performance.

## View locally

Open `index.html` in any modern browser. It has no build step, scripts, external
fonts, images, or network dependencies.

## Host with GitHub Pages

1. Add `README.md` and `index.html` to the root of a new GitHub repository.
2. Push the `main` branch.
3. In **Settings → Pages**, choose **Deploy from a branch**, select `main` and
   `/ (root)`, then save.

## Scope

The Apollo schema counts cover the sample implementation: one resolver class,
two output types, one input type, 16 fields, four root operations, and three
authorization declarations.

The comparison's 12 integration tests pass. The measured results are limited to
the local sample: three startup and code-generation samples, 50 requests per
operation, and three browser samples per implementation. The report does not
establish production security parity or estimate a full-service migration.
