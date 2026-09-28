# ok-to-test sandbox

Throwaway repository to test whether `GITHUB_TOKEN` (with `actions: write`)
can approve fork pull request workflow runs.

1. From a second GitHub account, fork this repo and open a PR.
2. The `CI` run should wait for approval.
3. Comment `/ok-to-test` on the PR.
4. Check the `ok-to-test` run log: HTTP `201` means GITHUB_TOKEN works.
