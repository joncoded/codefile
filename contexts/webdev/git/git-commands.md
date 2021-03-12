# Git commands

Type `git` plus any of the following on Terminal \(assuming that we have already run `git init` on the current folder\):

<table>
  <thead>
    <tr>
      <th style="text-align:left">Command</th>
      <th style="text-align:left">What it does</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left"><code>init</code>
      </td>
      <td style="text-align:left"><b>creates </b>or <b>initializes</b> a new local repository</td>
    </tr>
    <tr>
      <td style="text-align:left"><code>add -A</code>
      </td>
      <td style="text-align:left"><b>adds</b> all the changes to the Git repository to &quot;staging&quot;</td>
    </tr>
    <tr>
      <td style="text-align:left"><code>add [file]</code>
      </td>
      <td style="text-align:left"><b>adds</b> all the chances to a file to &quot;staging&quot;</td>
    </tr>
    <tr>
      <td style="text-align:left"><code>commit -m <br />&quot;[message]&quot;</code>
      </td>
      <td style="text-align:left"><b>updates</b> the local repository with all the changes previously added
        to &quot;staging&quot; (tagged with a message summarizing the changes made)</td>
    </tr>
    <tr>
      <td style="text-align:left"><code>remote add origin [repourl]</code>
      </td>
      <td style="text-align:left"><b>connects</b> the local repository with a remote repository (usually
        on GitHub.com)</td>
    </tr>
    <tr>
      <td style="text-align:left"><code>push [origin] [branch]</code>
      </td>
      <td style="text-align:left">
        <p><b>uploads</b> the most recently committed changes</p>
        <p>(from the local repository to the remote repository)</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><code>clone [repourl]</code>
      </td>
      <td style="text-align:left"><b>downloads</b> a remote repository to one&apos;s own computer</td>
    </tr>
    <tr>
      <td style="text-align:left"><code>checkout [branchname]</code>
      </td>
      <td style="text-align:left"><b>switches</b> to a branch in the local repository (assuming it exists)</td>
    </tr>
    <tr>
      <td style="text-align:left"><code>checkout -b [newbranchname]</code>
      </td>
      <td style="text-align:left"><b>creates</b> a new branch in the local repository</td>
    </tr>
    <tr>
      <td style="text-align:left"><code>branch -a</code>
      </td>
      <td style="text-align:left"><b>displays</b> a list of all branches</td>
    </tr>
    <tr>
      <td style="text-align:left"><code>status</code>
      </td>
      <td style="text-align:left">
        <p><b>displays</b> the current status of the local repository, i.e.:</p>
        <ul>
          <li>current branch name</li>
          <li>any files on staging</li>
          <li>any files with changes but not on staging</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><code>log</code>
      </td>
      <td style="text-align:left"><b>displays</b> a list of commits made by the current user</td>
    </tr>
    <tr>
      <td style="text-align:left"><code>pull [branch]</code>
      </td>
      <td style="text-align:left"><b>retrieves</b> the latest changes of a working version from the remote
        to the local</td>
    </tr>
    <tr>
      <td style="text-align:left"><code>diff</code>
      </td>
      <td style="text-align:left"><b>displays</b> a list of code changes since the last <code>add</code>
      </td>
    </tr>
  </tbody>
</table>

### Further reading

* [GitHub's Git cheat sheet](https://education.github.com/git-cheat-sheet-education.pdf)

