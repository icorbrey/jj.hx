# jj.hx

`jj.hx` provides [Jujutsu][jj] integration for [Helix][hx]. Until the
[Steel plugin pull request][steel-pr] is merged, you will need to have Helix
compiled with this branch.

## Installation

Install `jj.hx` with Forge, the Steel package manager:

```sh
forge pkg install --git https://github.com/icorbrey/jj.hx
```

Once installed, require it in your `init.scm`:

```scm
(require "jj/jj.scm")
```

## License

`jj.hx` is distributed under the [MIT license](./LICENSE.md).

[jj]: https://jj-vcs.github.io/jj "Jujutsu, a Git-compatible VCS that is both simple and powerful"
[hx]: https://helix-editor.com "Helix, a post-modern modal text editor"
[steel-pr]: https://github.com/helix-editor/helix/pull/8675
