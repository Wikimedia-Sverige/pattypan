To make a Windows EXE for a new version of Pattypan, follow the steps below. "vYY.MM" is the name of the tag for the release in the upstream repo.

1. `remote add upstream https://github.com/yarl/pattypan.git`
2. `git pull upstream`
3. `git checkout vYY.MM`
4. `git rebase windows-release`
5. `git tag vYY.MM-win`
6. `git push --tag`

This should trigger a Github action in *this* repo. Once it's done there will be a new release called "vYY.MM-win".
