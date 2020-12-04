FAQs
====

How Do I Create PRs at the Same Time If Multiple Code Repositories Have Compilation Dependencies?
-------------------------------------------------------------------------------------------------

During the development of the operating system (OS), it is common that
multiple code repositories have compilation dependencies. Therefore, the
PRs need to be created and merged at the same time. For this reason,
Gitee uses issues as the association identifiers for code repositories
with dependency dependencies to commit the PRs. Follow the operations
below:

1. Create an issue in any of the code repositories.

2. Associate PRs that need to be built and merged at the same time with
   the issue. For details, visit https://gitee.com/help/articles/4142.

3. After the build is triggered, the build center identifies the PRs
   associated with the same issue, downloads the build, and merges the
   PRs into the code library after the code is approved.

Rollback
--------

Visit https://gitee.com/help/articles/4195.

Resolving Merge Conflicts
-------------------------

Visit https://gitee.com/help/articles/4194.
