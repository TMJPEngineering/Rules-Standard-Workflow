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

## Credits

[digitaljhelms](https://gist.github.com/digitaljhelms/4287848)