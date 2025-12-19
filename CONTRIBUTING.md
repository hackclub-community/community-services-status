# Contributing to the repo

## IMPORTANT: Before you start

* Request for an org invite from either @3kho or @radioblahaj via HC Slack
(either DMs or in the #community channel should work) for issue assignments to
work reliably as well as to create/move repositories in the @hackclub-community
organization.
  * Alternatively, you can open an issue for a repo invite as a outside collaborator in the meanwhile [using this issue form][form]. If you do,
  you'll be granted with write access within 24 hours or so by @ajhalili2006.
* This Upptime-powered infra monitoring is available for Hack Clubbers running
community services, mostly hosted on [Nest](https://hackclub.app). Although we
have some HQ-sanctioned services hooked up (like [HC Accounts][hca]), if you
want to set up one for your own apps, [visit the official template for details][repo].

## Adding your service

In the [Upptime config file](./.upptimerc.yml), add your service at the end of
the `sites` list, using the following format:

```yaml
# Remember to replace the placeholder values below with your own.

sites:
  # ...other services here

  # Service Repo/Website: https://github.com/your-username/repo or https://project.website.tld
  # Primary maintainer: https://github.com/your-username / https://hackclub.enterprise.slack.com/team/U<SLACK_UID>
  - name: Your Service Here
    url: https://service.host.tld
    slug: slugified-name-here
    assignees:
    - your-username
```

Since the default branch is protected through branch rulesets (only org admins
as well as those with admin or maintain access can push directly), you will
need to submit your changes as a pull request. In most cases, @ajhalili2006
will review and merge your PR within a day or two for you and expect your
service to be monitored right after merging.

[form]: https://github.com/hackclub-community/community-services-status/issues/new?template=request-repo-access.yml
[hca]: https://github.com/hackclub/auth
[repo]: https://github.com/upptime/upptime
