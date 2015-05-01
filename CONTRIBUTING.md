# Contributing Guidelines

Skim is open source. It's hosted, developed, and maintained only on GitHub.

Skim follows the <a href="http://help.github.com/articles/using-pull-requests" target="_blank">fork-pull model</a> and leverages <a href="http://github.com/caleorourke/skim/issues" target="_blank">issues</a> and <a href="http://github.com/caleorourke/skim/pulls" target="_blank">pull requests</a> for source control, bug fixes, and new features. Anyone is welcome to submit a request, but I ask that you follow a few simple guidelines in regards to:

* [Code Standards](#code-standards)
* [Pull Requests](#pull-requests)
* [Feature Requests](#feature-requests)
* [Issue Reporting](#issue-reporting)

## Code Standards

All submissions should follow, but not strictly adhering to, the <a href="http://codeguide.co" target="_blank">Code Guide by @mdo</a>. Also, as a suggestion, you can configure these settings in your editor to follow this coding style.

~~~
"translate_tabs_to_spaces": true,
"tab_size": 2,
"ensure_newline_at_eof_on_save": false,
"default_encoding": "UTF-8",
"default_line_ending": "lf",
"trim_trailing_white_space_on_save": true
~~~

> Names and formatting vary across different editors.

## Pull Requests

I accept all types of pull requests, just as long as they stay within scope and don't break compatibility downstream. If you're unsure about what impact your request might have, send me a [New Feature request](#feature-requests) first. This gives me a chance to vet it before you start working on something that I may decide not to merge.

Create a pull request by following the instructions below.

1. Fork Skim from GitHub: `http://github.com/caleorourke/skim/fork`
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am "add some sweet features"`
4. Push to the branch: `git push origin my-new-feature`
5. Create new Pull Request in GitHub

## Feature Requests

When submitting a new request, please provide as much context as possible to justify how it fits in with Skim's scope. Click <a href="http://github.com/caleorourke/skim/issues" target="_blank">Search</a> to browse current requests or <a href="http://github.com/caleorourke/skim/issues/new" target="_blank">Request</a> to submit a new one.

## Issue Reporting

Got issues? Here are some suggestions to help guide you through escalating it to me.

#### Search issues already in GitHub

All issues are bagged and tagged in GitHub. Click <a href="http://github.com/caleorourke/skim/issues" target="_blank">Search</a> and make sure your issue hasn't already been reported.

#### Provide information about your setup

This includes versions, when was it installed, what you're trying to do, and so on.

#### Gauge its severity, impact, and occurrences

Help me understand how serious the issue is and what priority I need to triage it in.

#### Share code pastes in Gist

Paste any code, logs, or errors into a page on <a href="http://gist.github.com" target="_blank">Gist</a> and drop the link to it in the report.

#### Use this template to write-up your report

A good report should not require anyone to pine for more information. That's why I suggest using this template. It's sufficient for the majority of reports, albeit some issues may require me to ask for more details.

~~~
A summary of the issue and what problem it's causing.

Severity: (e.g. low, medium, high)
Impact: (e.g. minimal, nuisance, show-stopper)
Frequency: (e.g. daily, on shut down, random)

Steps to Reproduce
1. This is the first step
2. This is the second step
3. Additional steps, etc.

[url] (link to your Gist page)

Include any other comments, such as how you worked around it, suggestions you have for fixing it, and so on.
~~~

#### Submit the issue in GitHub

When you're ready, <a href="http://github.com/caleorourke/skim/issues/new" target="_blank">open a new issue</a> and send it over to me.
