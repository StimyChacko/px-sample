# Contributing to Predix UI

Hi,

Want to contribute your suggestions to Predix UI? **Here's how you can help.**

Please follow the below steps carefully, so your suggestions will be clear and developers can make effective fixes.

## Using the GitHub issue tracker

The GitHub issue tracker is the preferred channel for [bug reports](#bug-reports), [features requests](#feature-requests)
and [submitting pull requests](#pull-requests), so please respect the following
restrictions:

* Please **do not** use the GitHub issue tracker for personal support requests. Stack
  Overflow ([`predix ui`](https://stackoverflow.com/questions/tagged/predix-ui) tag), or [Predix.io](https://predix.io) are better places to get help.

* Please **do not** derail or troll issues. Keep the discussion on topic and
  respect the opinions of others.

* Please **do not** post vague comments like "+1" or ":thumbsup:".
  Use [GitHub's "reactions" feature](https://github.com/blog/2119-add-reactions-to-pull-requests-issues-and-comments). We reserve the right to delete comments.

## Issues and labels

Our bug tracker utilizes several labels to help organize and identify issues. Here's what they represent and how we use them:

- `browser bug` - Issues that are reported to us, but are actually the result of a browser-specific bug. These issues are diagnosed with reduced test cases and result in an issue opened on that browser's own bug tracker.
- `confirmed` - Issues that have been confirmed with a reduced test case and identify a bug in a Predix UI component.
- `css` - Issues stemming from our compiled CSS or source Sass files.
- `docs` - Issues for improving or updating our documentation.
- `examples` - Issues involving the example templates included in our docs.
- `feature` - Issues asking for a new feature to be added, or an existing one to be extended or modified. New features require a minor version bump (e.g., `v3.0.0` to `v3.1.0`).
- `gulp` - Issues with our included JavaScript-based gulpfile, which is used to run all our tests, concatenate and compile source files, and more.
- `help wanted` - Issues that we need or would like the community to help us resolve.
- `js` - Issues stemming from our compiled or source JavaScript files.
- `meta` - Issues with the project itself or our GitHub repository.


## Bug reports

A bug is a _demonstrable problem_ caused by the code in the repository.
Good bug reports are extremely helpful.

Guidelines for bug reports:

0. **Validate and lint your code**; [validate your HTML](http://html5.validator.nu)
   and [lint your HTML](http://www.dirtymarkup.com/) to ensure your
   problem isn't caused by a simple error in your own code.

1. **Use the GitHub issue search**; check if the issue has already been
   reported.

2. **Check if the issue has been fixed**; try to reproduce the issue by using the
   latest `master` or development branch in the repository.

3. **Isolate the problem**; ideally create a [reduced test
   case](https://css-tricks.com/reduced-test-cases/) and a live example using [CodePen](http://codepen.io/mdwragg/pen/LNwmpB) or [jsfiddle](https://jsfiddle.net/Lqmcwhw0/3/).


A good bug report shouldn't require others to get more information. Please be as detailed as possible in your report. What is your environment? What steps will reproduce the issue? What browser(s) and OS experience the problem? Do other browsers show the bug differently? What would you expect for the outcome? Such details will help people fix potential bugs.

Example:

> Short and descriptive example bug report title
>
> A summary of the issue and the browser/OS environment in which it occurs. If
> suitable, include the steps required to reproduce the bug.
>
> 1. This is the first step
> 2. This is the second step
> 3. Further steps, etc.
>
> `<url>` - a link to the reduced test case
>
> Any other information relevant to the bug report. This might include the lines of code that you have identified as
> causing the bug, and potential solutions (and your opinions on their
> merits).

## Feature Requests

Feature requests are welcome, but before opening one, determine if your idea suits the scope and aims of Predix UI. *You* need to make a strong case and convince the Predix UI team to adopt your feature. Please provide as much detail and context as possible.


## Pull Requests

Your pull requests???patches, improvements, and new features???are a big help. The requests should be focused and avoid unrelated commits.

**Please ask** before making a significant pull request (e.g., implementing features, refactoring code, or porting to a different language) that Predix UI developers might not merge into the component.

Please follow the [coding guidelines](#code-guidelines) used throughout the project (indentation, accurate comments, etc.) and any other requirements (such as test coverage).

**Do not edit any of the CSS files directly!** The files are automatically generated. You should edit the source files in [`sass/`] instead.

**Do not edit the `gh-pages` branch.** That branch is generated from the documentation source files and is managed separately by the Predix UI team.

Please use the following process to have your work considered for the project:

1. [Fork](https://help.github.com/fork-a-repo/) the component.

2. Create a new topic branch (off the main project development branch) to
   contain your feature, change, or fix:

   ```
   bash
   git checkout -b <topic-branch-name>
   ```

3. Commit your changes in logical chunks. Please adhere to these [git commit message guidelines](http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html) or your code is unlikely to be merged into the main project. Use Git's [interactive rebase](https://help.github.com/articles/interactive-rebase) feature to tidy up your commits before making them public.

4. Locally merge (or rebase) the latest commits into your branch:

   ```
   bash
   git pull [--rebase] origin master
   ```

5. Push your topic branch up to your fork:

   ```
   bash
   git push origin <topic-branch-name>
   ```

6. [Open a Pull Request](https://help.github.com/articles/using-pull-requests/) with a clear title and description against the `master` branch.

## Code guidelines

### HTML

[Adhere to the Code Guide.](http://codeguide.co/#html)

- Use tags and elements appropriate for an HTML5 doctype (e.g., self-closing tags).
- Use [WAI-ARIA](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA) attributes in documentation examples to promote accessibility.

### CSS

[Adhere to the Code Guide.](http://codeguide.co/#css)

- When feasible, default color palettes should comply with [WCAG color contrast guidelines](http://www.w3.org/TR/WCAG20/#visual-audio-contrast).
- Except in rare cases, don't remove default `:focus` styles (via e.g. `outline: none;`) without providing alternative styles. See [this A11Y Project post](http://a11yproject.com/posts/never-remove-css-outlines/) for more details.

### JS

- 2 spaces (no tabs)
- "Attractive"
- no errors / warnings
