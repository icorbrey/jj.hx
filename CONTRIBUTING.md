# How to contribute

## Policies

### Commit guidelines

Unlike many GitHub projects (but like many VCS projects), we care more about the
contents of commits than about the contents of PRs. We review each commit
separately, and we don't squash-merge the PR (so please manually squash any
fixup commits before sending for review).

Each commit should ideally do one thing. For example, if you need to refactor a
function in order to add a new feature cleanly, put the refactoring in one
commit and the new feature in a different commit. If the refactoring itself
consists of many parts, try to separate out those into separate commits. You can
use `jj split` to do it if you didn't realize ahead of time how it should be
split up. Include tests and documentation in the same commit as the code they
test and document.

The commit message should describe the changes in the commit;
the PR description can even be empty, but feel free to include a personal
message. We start the commit message with `<topic>: `  and don't use
[conventional commits](https://www.conventionalcommits.org/en/v1.0.0/). This
means if you modified a command in the CLI, use its name as the topic, e.g.
`next/prev: <your-modification>` or `conflicts: <your-modification>`. We don't
currently have a specific guidelines on what to write in the topic field, but
the reviewers will help you provide a topic if you have difficulties choosing
it. [How to Write a Git Commit Message](https://cbea.ms/git-commit/) is a good
guide if you're new to writing good commit messages. We are not particularly
strict about the style, but please do explain the reason for the change unless
it's obvious.
