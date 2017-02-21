# Git Branching Standards & Conventions

## Quick Legend

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
      <td>Name</td>
      <td>*-branch</td>
      <td>Accepts merges from features, issues, and hotfixes</td>
    </tr>
    <tr>
      <td>Issues</td>
      <td>issue-*</td>
      <td>Always branch off HEAD of *-branch</td>
    </tr>
    <tr>
      <td>Features</td>
      <td>feature-*</td>
      <td>Always branch off HEAD of *-branch</td>
    </tr>
    <tr>
      <td>Hotfixes</td>
      <td>hotfix-*</td>
      <td>Always branch off HEAD of *-branch</td>
    </tr>
  </tbody>
</table>

## Branch Hierarchy

![Branch Hierarchy](https://cloud.githubusercontent.com/assets/21231662/23155841/3734819c-f84f-11e6-888f-e25b550e38ab.png)

## Credits

[digitaljhelms](https://gist.github.com/digitaljhelms/4287848)