# Contributing

If you'd like to help improve this extension, we welcome you to [file an issue](https://github.com/lupomikti/migoto-vscode/issues) first for any new features or bug fixes. This is mostly for tracking and history purposes and allows for focused and meaningful discussion before code is written. This isn't some large project so there are no CLAs or a formal Code of Conduct.

Machine-assisted contributions must be both endorsed and thoroughly reviewed by a human before submission and must also state that such tools were used including the specifc tool(s).

# Development and Building

This project is making use of [Bun](https://bun.sh/docs/pm/cli/install) for package management.

First you will need to run `bun install` from the project root.

To build the VS Code Extension VSIX package, you will need to have installed `vsce` (`bun install -g @vscode/vsce`) and then should do one of the following:

1. `bun run package <version>`

2. `vsce package <version> [--pre-release] --no-git-tag-version`

`<version>` can be like "0.4.3" or "minor" to increment only the minor number from the previous value in `package.json`.

This will change the `package.json` version, so it is a good idea to make a version bump commit at this point too.