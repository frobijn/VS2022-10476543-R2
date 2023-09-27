This is a demo for a [VS2022 issue](https://developercommunity.visualstudio.com/t/Solution-without-projectsfolder-view-af/10476543).


How to set up the demo:

- Create a demo directory, e.g., `C:\....\demo`
- Clone [repository #1](https://github.com/frobijn/VS2022-10476543-R1) in `C:\....\demo\Repository1`
- Clone [repository #2](https://github.com/frobijn/VS2022-10476543-R2) in `C:\....\demo\Repository2`
- Move the files `SolutionProjects-NotInGit.sln` and `SolutionWithoutProjects-NotInGit.sln` from `C:\....\demo\Repository1` to `C:\....\demo`
- Start VS2022 and open the local directory `C:\....\demo`

Demo of the issues:

# Solution outside of git, no projects, items from both repositories
- Use the _Solution explorer_’s _Switch between solutions and available views_ button to open `SolutionWithProject-Repository1.sln`
- Use the same button to open `SolutionWithoutProjects-NotInGit.sln`

The `Git changes` window does not show any repositories

# Solution in one repository, no projects, items from both repositories
- Use the _Solution explorer_’s _Switch between solutions and available views_ button to open `SolutionWithProject-Repository1.sln`
- Use the same button to open `SolutionWithoutProjects-Repository2.sln`

The `Git changes` window shows _Repository 2_, not _Repository 1_
