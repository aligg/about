---
title: Sourcegraph for GitLab
description: Sourcegraph features on GitLab
authors:
  - github.com/ijsnow
startdate: 2018-09-18
enddate: 2018-10-01
releasedate: 2018-10-01
publishdate: 2018-10-01
published: false
---

You can now get code intelligence on GitLab with the Sourcegraph browser
extension, just as 10,000s of developers get on GitHub now.

<!-- Gif -->

To start using this:

1. Install [Sourcegraph for Chrome](...) or [Sourcegraph for Firefox](...)
2. Visit [common/executor.go](https://gitlab.com/gitlab-org/gitlab-runner/blob/master/common/executor.go) in [gitlab-org/gitlab-runner](https://gitlab.com/gitlab-org/gitlab-runner) on GitLab (or any other file in a public repository)
3. To enable Sourcegraph on your own GitLab instance on Chrome, right click the Sourcegraph logo in your browser's
   toolbar and click "Enable Sourcegraph on this domain"
4. Hover over any token in the file to see tooltips

To use this on your company's private code, run a [Sourcegraph instance](https://about.sourcegraph.com/docs).

GitLab is the first of many more code hosts Sourcegraph will support in [the open
source Sourcegraph browser extension](https://github.com/sourcegraph/browser-extensions). Check out the code it took to add
GitLab support: https://sourcegraph.com/github.com/sourcegraph/browser-extensions/-/blob/src/libs/gitlab/code_intelligence.ts

## Implementation Notes

- I want to give GitLab a shoutout for making a really clean DOM. We extend
  several products via the DOM and GitLab's is by far the cleanest. Thanks for
  minding your class names GitLabbers!