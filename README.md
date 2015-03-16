# Geometryangle

[jQuery](http://jquery.com/) plugin that lets you create beautiful and responsive backgrounds to your site. **To get started, check out http://geometryangle.tritoncode.com/**

Please consider that the project is still in beta. The current status of the milestones can be found [here](https://github.com/TritonCode/Geometryangle/milestones).

## Quick start

Download the [latest release](https://github.com/TritonCode/Geometryangle/zipball/master).

Put the script at the [bottom](https://developer.yahoo.com/performance/rules.html#js_bottom) of your markup right after jQuery:

```html
<script src="jquery.min.js"></script>
<script src="Geometryangle/geometryangle.js"></script>
```

To create a fixed background, do the following:

```html
<body>
<div style="position: fixed; left: 0; right: 0; top: 0; bottom: 0;"></div>
<div>
Content...
</div>
</body>
```

Call the [plugin](http://learn.jquery.com/plugins/) function and your navigation widget is ready.

```javascript
$(document).ready(function(){
  $('body').Geometryangle({mesh:{}, lights: [{}], line: {}, vertex: {}});
});
```

## Documentation

The documentation is publicly available at http://geometryangle.tritoncode.com/

## Contributing

The [issue tracker](https://github.com/TritonCode/Geometryangle/issues) is the preferred channel for bug reports, features requests and submitting pull requests.

**Please do not use the issue tracker for personal support requests. Stack Overflow ([`Geometryangle`](http://stackoverflow.com/questions/tagged/Geometryangle)) is a better place to get help.**

### Bug reports

A bug is a **demonstrable problem** that is caused by the code in the repository. Good bug reports are extremely helpful, so thanks!

Guidelines for bug reports:

  1. Use the GitHub issue search — check if the issue has already been reported.

  2. Check if the issue has been fixed — try to reproduce it using the latest `develop` branch in the repository.

  3. Isolate the problem — ideally create a reduced test case and a live example. This [JSFiddle](http://jsfiddle.net/eqbL6vLb/) and this [JS Bin](http://jsbin.com/xuxozu/1) are helpful templates you can fork or clone.

Example:

> Short and descriptive example bug report title
> 
> A summary of the issue and the browser/OS environment in which it occurs. If suitable, include the steps required to reproduce the bug.
> 
>   1. This is the first step
>   2. This is the second step
>   3. Further steps, etc.
> 
> `<url>` - a link to the reduced test case
> 
> Any other information you want to share that is relevant to the issue being reported. This might include the lines of code that you have identified as causing the bug, and potential solutions (and your opinions on their merits).

### Feature requests

Feature requests are welcome. But take a moment to find out whether your idea fits with the scope and aims of the project. It's up to you to make a strong case to convince the project's developers of the merits of this feature. Please provide as much detail and context as possible.

### Pull requests

Good pull requests are a fantastic help. They should remain focused in scope and avoid containing unrelated commits.

**Please ask first** before embarking on any significant pull request (e.g. implementing features, refactoring code, porting to a different language), otherwise you risk spending a lot of time working on something that the project's developers might not want to merge into the project.

Adhering to the following process is the best way to get your work included in the project:

  1. [Fork](http://help.github.com/fork-a-repo/) the project, clone your fork, and configure the remotes:

    ```bash
    git clone https://github.com/<your-username>/Geometryangle.git
    cd Geometryangle
    git remote add upstream https://github.com/TritonCode/Geometryangle.git
    ```

  2. If you cloned a while ago, get the latest changes from upstream:

    ```bash
    git checkout develop
    git pull [--rebase] upstream develop
    ```

  3. Create a new topic branch (off the main project `develop` branch) to contain your feature, change, or fix:

    ```bash
    git checkout -b <topic-branch-name>
    ```

  4. Build the distribution before committing to ensure your changes follow the coding standards and all build files are up to date.

    ```bash
    grunt dist
    ```

  5. Commit your changes in logical chunks. Please adhere to these [guidelines](http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html). Use Git's [interactive rebase](https://help.github.com/articles/interactive-rebase) feature to tidy up your commits before making them public.

  6. Locally merge (or rebase) the upstream development branch into your topic branch:

    ```bash
    git pull [--rebase] upstream develop
    ```

  7. Push your topic branch up to your fork:

    ```bash
    git push origin <topic-branch-name>
    ```

  8. [Open a Pull Request](https://help.github.com/articles/using-pull-requests/) with a clear title and description against the `develop` branch.

**By submitting a patch, you agree to allow the project owner to
license your work under the terms of the [MIT License](LICENSE).**

## License

The code and the documentation are released under the [MIT License](LICENSE).
