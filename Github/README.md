# Github Standard

List of TMJP Engineering rules &amp; standard workflow in Github

## Table of Contents

- [Git Branch Conventions](https://github.com/TMJPEngineering/Standard-Workflow-Rules/tree/master/Github#quick-legend)
- [Git Workflow](https://github.com/TMJPEngineering/Standard-Workflow-Rules/tree/master/Github#git-workflow)
- [Branch Hierarchy](https://github.com/TMJPEngineering/Standard-Workflow-Rules/tree/master/Github#branch-hierarchy)
- [Credits](https://github.com/TMJPEngineering/Standard-Workflow-Rules/tree/master/Github#credits)
- [LICENSE](https://github.com/TMJPEngineering/Standard-Workflow-Rules/tree/master/Github#license)

## Git Branch Conventions

<table>
  <thead>
    <tr>
      <th>Stage</th>
      <th>Branch</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Stable</td>
      <td>master</td>
      <td>Accepts merges from dev</td>
    </tr>
    <tr>
      <td>Development</td>
      <td>dev</td>
      <td>Accepts merges from Developer Stage</td>
    </tr>
    <tr>
      <td>Developer</td>
      <td>[name]-branch</td>
      <td>Accepts rebase and merge from features, issues, and hotfixes</td>
    </tr>
    <tr>
      <td>Issues</td>
      <td>issue-[name]</td>
      <td>Always branch off HEAD of Developer Stage</td>
    </tr>
    <tr>
      <td>Features</td>
      <td>feature-[name]</td>
      <td>Always branch off HEAD of Developer Stage</td>
    </tr>
    <tr>
      <td>Hotfixes</td>
      <td>hotfix-[name]</td>
      <td>Always branch off HEAD of Developer Stage</td>
    </tr>
  </tbody>
</table>

## Git Workflow

### Pull Requests

- `master` branch *always* merge commit from `dev`
- `dev` branch *always* merge commit from Developer Stage
- In Developer Stage, *always* accept *rebase & merge* from issue, hotfix, and feature branches

### Locally

Always run `git pull` in Developer Stage, `dev` branch, and `master` branch if those branches aren't updated in local.

For creating branch from Developer Stage, run this command:

- `git checkout -b <new-branch> <source-branch>`
  - This will create and switch to a new branch from source branch
    - Example: `git checkout -b hotfix-auth john-branch`
    - Example: `git checkout -b feature-message jam-branch`

Every first push in your branch, *always* run this:

```
git push origin <branch-name> -u
```

For the next push in your branch, *always* run this:

```
git push origin <branch-name> -f
```

If you're branch is outdated to `dev`, run this command from Developer Stage:

```
git rebase dev 
```

As well as the Developer Stage, if issue, hotfix or feature branches were outdated to the Developer Stage, run this command by example:

```
git rebase john-branch // Name of your branch
```

Make sure that you run `git pull` in development stage. If not, your branch will not be fixed.

After that, if there are conflicts, use the following commands below:

- `git add .`
- `git rebase --continue`

## Branch Hierarchy

![Branch Hierarchy](https://cloud.githubusercontent.com/assets/21231662/23155841/3734819c-f84f-11e6-888f-e25b550e38ab.png)

## Credits

[digitaljhelms](https://gist.github.com/digitaljhelms/4287848)

## LICENSE

This project is licensed under the MIT License - see the [LICENSE](https://github.com/TMJPEngineering/Standard-Workflow-Rules/blob/master/LICENSE) for details.

Copyright (c) 2017 [TMJ]() Philippines