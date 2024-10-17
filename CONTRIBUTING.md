# Contributing to the Defender Docs
Thank you for your interest in contributing to the Defender Docs!

Please take a moment to review this document in order to make the contribution process easy and effective for everyone involved.

## Using the issue tracker

The [issue tracker](https://github.com/Openzeppelin/defender-docs/issues) is
the preferred channel for [submitting pull requests](#pull-requests), but please respect the following
restrictions:

- Please **do not** use the issue tracker for personal support requests (reach out to [defender-support@openzeppelin.com](mailto:defender-support@openzeppelin.com) or submit a post to the [Defender Forum](https://forum.openzeppelin.com/)).

- Please **do not** derail or troll issues. Keep the discussion on topic and
  respect the opinions of others.

## Pull requests

Good pull requests are a fantastic help. They should remain focused in scope and avoid containing unrelated commits.

**Please ask first** before embarking on any significant pull request (e.g.
implementing features, refactoring code, porting to a different language),
otherwise you risk spending a lot of time working on something that the
project's developers might not want to merge into the project.

Please adhere to the coding conventions used throughout a project (indentation,
accurate comments, etc.) and any other requirements (such as test coverage).

Adhering to the following process is the best way to get your work
included in the project:

1. [Fork](https://help.github.com/articles/fork-a-repo/) the project, clone your
   fork, and configure the remotes:

   ```bash
   # Clone your fork of the repo into the current directory
   git clone https://github.com/<your-username>/defender-docs.git
   # Navigate to the newly cloned directory
   cd defender-docs
   # Assign the original repo to a remote called "upstream"
   git remote add upstream https://github.com/OpenZeppelin/defender-docs.git
   ```

2. If you cloned a while ago, get the latest changes from upstream:

   ```bash
   git checkout main
   git pull upstream main
   ```

3. Create a new topic branch (off the main project development branch) to
   contain your feature, change, or fix:

   ```bash
   git checkout -b <me>
   ```

4. Install locked dependencies:

   ```bash
   npm install
   ```

   Ensure that your `node` and `npm` versions are compatible with the `engines`
   specification in `package.json`.

5. Commit your changes in logical chunks. Please adhere to these [git commit
   message guidelines](https://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html)
   or your code is unlikely be merged into the main project. Use Git's
   [interactive rebase](https://help.github.com/articles/about-git-rebase/)
   feature to tidy up your commits before making them public.

6. Locally merge (or rebase) the upstream development branch into your topic branch:

   ```bash
   git pull [--rebase] upstream main
   ```

7. Preview changes:

   ```bash
   npm run docs:watch
   ```

8. Push your topic branch up to your fork:

   ```bash
   git push origin <topic-branch-name>
   ```

9. [Open a Pull Request](https://help.github.com/articles/using-pull-requests/)
    with a clear title and description.

**IMPORTANT**: By submitting a patch, you agree to allow the project
owners to license your work under the terms of the [MIT License](LICENSE.txt).
