---
title: Configure GitHub CLI to clone with SSH
date: 2020-12-01T22:10:11.153Z
---

By default, [`gh repo clone`](https://cli.github.com/manual/gh_repo_clone) uses HTTPS. To configure `gh` to clone with SSH, run the following command:

```shell
gh config set git_protocol ssh
```

Thanks for the tip, [@ampinsk](https://twitter.com/ampinsk)!
