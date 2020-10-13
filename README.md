<!--
Event: [Angular Athens - 2nd workshop: Contriguting to Angular](https://www.meetup.com/Angular-Athens)
Date: 2020-10-13
Instructor: [George Kalpakas](https://twitter.com/gkalpakas)
-->

# <a name="top"></a> Angular Athens - 2nd workshop: Contributing to Angular

> [George Kalpakas](https://github.com/gkalpak) | Twitter: https://twitter.com/gkalpakas

Νotes for the "theoretical" part of the 2nd [Angular Athens](https://www.meetup.com/Angular-Athens) workshop on contributing to Angular (and OSS in general).

**Table of contents**

- [ ] [About open-source software (OSS) and contributing](#about-oss)
- [ ] [How to contribute](#how-to-contrib)
- [ ] [Where to contribute](#where-to-contrib)
- [ ] [Contribution process](#contrib-process)
  - [ ] [Non-PR-based contribution process](#non-pr-contrib-process)
  - [ ] [PR-based contribution process](#pr-contrib-process)
- [ ] [Contributing during the workshop](#workshop-contrib)
  - [ ] [Choosing an issue](#choose-issue)
  - [ ] [Working on the different issue types](#work-on-issue)


## <a name="about-oss"></a> About open-source software (OSS) and contributing

Good resources on OSS:

- [ ] On [all aspects](https://opensource.guide/).
- [ ] Specifically on [contributing](https://opensource.guide/how-to-contribute).

<p align="right"><sub><a href="#top">Back to top</a></sub></p>


## <a name="how-to-contrib"></a> How to contribute

There are many different ways to contribute to OSS (in general) and the Angular project (in particular), including (but not limited to):

- [ ] Helping others online/offline ([StackOverflow](https://stackoverflow.com/questions/tagged/angular), [Discord](https://discord.gg/angular), [Gitter](https://gitter.im/angular/angular), [Slack](https://angular-athens.slack.com/), colleagues, etc.).
- [ ] Creating educational resources (blog posts, presentations, courses, etc.).
- [ ] Responding to GitHub issues (if you know the answer or have additional information that might help).
- [ ] Creating reproductions for bug reports lacking them.
- [ ] Creating issues for docs problems, bug reports, feature requests.
- [ ] Reviewing pull requests (PRs) - esp. if you have expertise on the subject or framework area.
- [ ] Submitting PRs.

For PRs in particular, there can be several types (with varying degrees of complexity):

- [ ] Simple docs fixes (typos, punctuation, grammar, etc.).
- [ ] Docs improvements (re-wording, new content, etc.).
- [ ] Code refactoring (styling fixes, code simplification, etc.).
- [ ] Bug fixes (again, with varying degrees of complexity).
- [ ] New features.

> IMPORTANT:<br />
> Before spending significant time on a PR, coordinate with the team.

<p align="right"><sub><a href="#top">Back to top</a></sub></p>


## <a name="where-to-contrib"></a> Where to contribute

The Angular project comprises several repositories. Choose where to contribute based on your interests:

- [ ] [**Framework**](https://github.com/angular/angular): Most `@angular/*` packages (such as `core`, `forms`, `router`, `animations`, etc.).<br />
    _This is what we are focusing on in this workshop._
- [ ] [CLI](https://github.com/angular/angular-cli): The `@angular/cli` package and all `@angular-devkit/*` packages.
- [ ] [Universal](https://github.com/angular/universal): All `@nguniversal/*` packages.
- [ ] [Components (aka Material)](https://github.com/angular/components): The `@angular/cdk` and `@angular/material` packages (plus some other packages related to CDK/Material).
- [ ] [AngularJS material](https://github.com/angular/material): The `angular-material` package (i.e. Material design for AngularJS v1.x).<br />
    _It will enter LTS mode soon._

<p align="right"><sub><a href="#top">Back to top</a></sub></p>


## <a name="contrib-process"></a> Contribution process


### <a name="non-pr-contrib-process"></a> Non-PR-based contribution process

For contributions that do _not_ involve submitting a PR, the process is simple:

- [ ] Just navigate to the issue on GitHub in your browser.

If you want to create a reproduction for an issue, you have two options:

- [ ] Create a minimal app that reproduces the problem on [StackBlitz](https://stackblitz.com/).<br />
  (Use [this template](https://stackblitz.com/fork/angular-ivy) for creating an Angular app.)
- [ ] Create a minimal project that reproduces the problem and push it to a new GitHub repository.

> NOTE:<br />
> Generally, StackBlitz is preferable as a reproduction medium, but there are some issues that cannot be reproduced on StackBlitz.
> For example, issues involving ServiceWorkers, server-side rendering, custom build configurations, etc.

<p align="right"><sub><a href="#top">Back to top</a></sub></p>


### <a name="pr-contrib-process"></a> PR-based contribution process

Below is an overview of the process of creating and submitting a PR. For more details, check out [CONTRIBUTING.md](https://github.com/angular/angular/blob/b2342d4116d4a57b832628b878c467402581dbf4/CONTRIBUTING.md).

> NOTE:<br />
> For simple PRs that only affect a single file (and no tests), one can work directly in their browser and [submit a PR using the GitHub UI](https://docs.github.com/en/free-pro-team@latest/github/managing-files-in-a-repository/editing-files-in-another-users-repository) .

- [ ] **1.** Ensure the following tools are installed and available on the `PATH`:
  - [ ] [git](https://git-scm.com/) (any reasonably recent version) - [Download git](https://git-scm.com/downloads)
  - [ ] [Node.js](https://nodejs.org/en/) (a version in the range specified in [package.json > engines.node](https://github.com/angular/angular/blob/a84976fdfcde45adeba406be48ed979c2010ee57/package.json#L11)) - [Download Node.js](https://nodejs.org/en/download/)
  - [ ] [yarn](https://classic.yarnpkg.com/) (a version in the range specified in [package.json > engines.yarn](https://github.com/angular/angular/blob/a84976fdfcde45adeba406be48ed979c2010ee57/package.json#L12)) - [Install yarn](https://classic.yarnpkg.com/en/docs/install)

- [ ] **2.** Fork the [angular/angular](https://github.com/angular/angular) repo. ([instructions](https://docs.github.com/en/free-pro-team@latest/github/getting-started-with-github/fork-a-repo))

- [ ] **3.** Clone your fork locally. ([instructions](https://docs.github.com/en/free-pro-team@latest/github/creating-cloning-and-archiving-repositories/cloning-a-repository))

- [ ] **4.** Pick an issue to work on.<br />
    _For the workshop, you can pick from [our curated list](https://github.com/angularathens/2nd-workshop-angular-contrib/issues)._

- [ ] **5.** Write one or more failing tests (if applicable).

- [ ] **6.** Implement the fix or feature.

- [ ] **7.** Submit a PR. (Also [sign the CLA](https://github.com/angular/angular/blob/b2342d4116d4a57b832628b878c467402581dbf4/CONTRIBUTING.md#cla) if not already signed.)

- [ ] **8.** Address any review feedback.

- [ ] **9.** :tada:

<p align="right"><sub><a href="#top">Back to top</a></sub></p>


## <a name="workshop-contrib"></a> Contributing during the workshop


### <a name="choose-issue"></a> Choosing an issue

You can freely choose what kind of contribution you want to work on.<br />
_(For the workshop, we are sticking to the `angular/angular` repo.)_

Since there are currently over 2500 issues on `angular/angular` (:sweat_smile:), we have put together a [curated list of issues](https://github.com/angularathens/2nd-workshop-angular-contrib/issues) that we consider suitable for first-time contributors.

There are basically 4 types of issues on the list:

- [ ] [support](https://github.com/angularathens/2nd-workshop-angular-contrib/issues?q=is%3Aissue+is%3Aopen+label%3Asupport):
  - These are about interacting on GitHub issues and providing useful information.
  - They do _not_ involve submitting a PR.

- [ ] [documentation](https://github.com/angularathens/2nd-workshop-angular-contrib/issues?q=is%3Aissue+is%3Aopen+label%3Adocumentation):
  - These are about fixing issues in documentation content.
  - They involve submitting a PR, but not writing/building code or running tests.

- [ ] [docs-infra](https://github.com/angularathens/2nd-workshop-angular-contrib/issues?q=is%3Aissue+is%3Aopen+label%3Adocs-infra):
  - These are about fixing issues in the documentation infrastructure, i.e. the angular.io application and related tooling.
  - They may involve writing code and potentially building the app and/or running tests.

- [ ] [bug](https://github.com/angularathens/2nd-workshop-angular-contrib/issues?q=is%3Aissue+is%3Aopen+label%3Abug):
  - These are about fixing issues in the framework itself (i.e. one of the `@angular/*` packages).
  - They involve writing/building code and running tests.

  > NOTE:
  > There is currently only one issue of this type, because such issues tend to be more challenging (and thus not suitable for a first-time contributor).

<p align="right"><sub><a href="#top">Back to top</a></sub></p>


### <a name="work-on-issue"></a> Working on the different issue types

Depending on the type of issue, there are different commands one can run to prepare their environment before starting with the actual work.

- [ ] For issues labelled as `support`: N/A
- [ ] For issues labelled as `documentation` or `docs-infra`: `yarn --cwd=aio setup`<br />
  See also [aio/README.md](https://github.com/angular/angular/blob/a84976fdfcde45adeba406be48ed979c2010ee57/aio/README.md) for more info on working on the angular.io application and the documentation content.
- [ ] For issues labelled as `bug`: `yarn install`<br />
  See also [docs/DEVELOPER.md](https://github.com/angular/angular/blob/a84976fdfcde45adeba406be48ed979c2010ee57/docs/DEVELOPER.md) for more info on working on the Angular source code.

<p align="right"><sub><a href="#top">Back to top</a></sub></p>

---
<p align="center"><b>:computer: Happy hacking! :rocket:</b></p>
