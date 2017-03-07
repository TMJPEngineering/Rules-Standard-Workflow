# Github Standard

List of TMJP Engineering rules &amp; standard workflow in Github

## Table of Contents

- [Git Branch Conventions](https://github.com/TMJPEngineering/Standard-Workflow-Rules/tree/master/Github#quick-legend)
- [Git Workflow](https://github.com/TMJPEngineering/Standard-Workflow-Rules/tree/master/Github#git-workflow)
- [Branch Hierarchy](https://github.com/TMJPEngineering/Standard-Workflow-Rules/tree/master/Github#branch-hierarchy)
- [Credits](https://github.com/TMJPEngineering/Standard-Workflow-Rules/tree/master/Github#credits)
- [License](https://github.com/TMJPEngineering/Standard-Workflow-Rules/tree/master/Github#license)

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
      <td>Accepts merges from *-branch</td>
    </tr>
    <tr>
      <td>Developer</td>
      <td>*-branch</td>
      <td>Accepts rebase and merge from features, issues, and hotfixes</td>
    </tr>
    <tr>
      <td>Issues</td>
      <td>issue-*</td>
      <td>Always branch off HEAD of developer stage</td>
    </tr>
    <tr>
      <td>Features</td>
      <td>feature-*</td>
      <td>Always branch off HEAD of developer stage</td>
    </tr>
    <tr>
      <td>Hotfixes</td>
      <td>hotfix-*</td>
      <td>Always branch off HEAD of developer stage</td>
    </tr>
  </tbody>
</table>

## Git Workflow

### Pull Requests

- `master` branch *always* merge commit from `dev`
- `dev` branch *always* merge commit from developer stage
- In developer stage, *always* accept *rebase & merge* from issue, hotfix, and feature branches

### Locally

These are the commands you will use in terminal or git bash:

Always run `git pull` in dev if that branch aren't updated in local. To say that you're dev wasn't up to date, check the *Network Graph* in Github.

For creating branch from developer stage, run this command:

- `git checkout -b <new-branch> <source-branch>`
  - This will create and switch to a new branch from source branch
    - Example: `git checkout -b hotfix-auth john-branch`
    - Example: `git checkout -b feature-message jam-branch`

In case of conflicts, run this command:

```
git rebase dev
```

Make sure that you run `git pull` in development stage. If not, your branch will not be fixed.

## Branch Hierarchy

![Branch Hierarchy](https://cloud.githubusercontent.com/assets/21231662/23155841/3734819c-f84f-11e6-888f-e25b550e38ab.png)

## Credits

[digitaljhelms](https://gist.github.com/digitaljhelms/4287848)

## LICENSE

This project is licensed under the MIT License - see the [LICENSE](https://github.com/TMJPEngineering/Standard-Workflow-Rules/blob/master/LICENSE) for details.

Copyright (c) 2017 [TMJ]() Philippines