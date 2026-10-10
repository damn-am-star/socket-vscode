.

## Development

```shell
pnpm install
```

Press `F5` in VS Code to build the extension and launch an Extension Development Host. Development builds include source maps for breakpoints in `src/`.

`pnpm run build` defaults to `build:dev`. Use `pnpm run build:prod` for a minified production build.

Run the `Socket: watch` task or `pnpm run watch` to rebuild on edits. Reload the Extension Development Host to load each rebuild.

Run the `Socket: test` task or `pnpm test --all` for the full test suite. Use `pnpm test test/repo/unit/auth.test.mts` to run one test file.

Run `pnpm run package-for-vscode` to build and package the production `.vsix`.

Run `pnpm run test:extension --vsix <path>` to test the packaged extension in an isolated VS Code Extension Host.
The smoke test checks activation, Login registration, logged-out state, and JavaScript document opening.
It requires the `code` executable on `PATH`, or `--code <executable>`.

## License

MIT
