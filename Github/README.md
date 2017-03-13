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
      <td>Accepts rebase and merges from issue, feature, and hotfix branches/td>
    </tr>
    <tr>
      <td>Issues</td>
      <td>issue-[name]</td>
      <td>Always branch off HEAD of Development Stage</td>
    </tr>
    <tr>
      <td>Features</td>
      <td>feature-[name]</td>
      <td>Always branch off HEAD of Development Stage</td>
    </tr>
    <tr>
      <td>Hotfixes</td>
      <td>hotfix-[name]</td>
      <td>Always branch off HEAD of Development Stage</td>
    </tr>
  </tbody>
</table>

## Git Workflow

### Pull Requests

- `master` branch *always* merge commit from `dev`
- `dev` branch *always* accept *rebase & merge* from issue, hotfix, and feature branches

### Locally

Always run `git pull` in `dev` branch if it isn't updated to local.

For creating branch from `dev`, run this command:

- `git checkout -b <new-branch> dev`
  - This will create and switch to a new branch from `dev`
    - Example: `git checkout -b hotfix-auth dev`
    - Example: `git checkout -b feature-message dev`
    - Example: `git checkout -b issue-cors dev`

Every first push in your branch, *always* run this:

```
git push origin <branch-name> -u
```

**Note:** The `-u` option automatically sets that upstream for you, linking your repo to a central one. That way, in the future, Git "knows" where you want to push to and where you want to pull from, so you can use `git pull` or `git push` without arguments.

For the next push in your branch, *always* run this:

```
git push origin <branch-name> -f
```

**Note:** The `-f` option is short for `--force`

If you're branch is outdated to `dev`, run this in your terminal:

```
git rebase dev 
```

Make sure that you run `git pull` in `dev` branch. If not, your branch will not be fixed.

After that, if there are conflicts, use the following commands below:

- `git add .`
- `git rebase --continue` *// If only you have 2 or more conflicts to fix*

## Branch Hierarchy

![Branch Hierarchy](https://cloud.githubusercontent.com/assets/21231662/23843177/e179dfda-07f4-11e7-8685-3f0b01b2ff96.png)

## Credits

[digitaljhelms](https://gist.github.com/digitaljhelms/4287848)

## LICENSE

This project is licensed under the MIT License - see the [LICENSE](https://github.com/TMJPEngineering/Standard-Workflow-Rules/blob/master/LICENSE) for details.

Copyright (c) 2017 [TMJ](http://www.tmj.jp) Philippines