---
title: "About"
date: 2019-06-28
draft: false
disableToc: false
---

# Packit

Packit provides tooling and automation to integrate upstream open source
projects into Fedora operating system. Packit project is composed of two main
components:

1. `packit`, a CLI tool, which you can install locally and start using right away.

2. [Packit-as-a-Service](https://github.com/marketplace/packit-as-a-service), a
   GitHub app — it can provide you feedback on how is your project integrated
   with Fedora Operating System.

Feel free to jump into [the guide]({{< ref "/docs/guide" >}}) for using packit.

### Upstream repository

https://github.com/packit-service/packit


### Contact

You can find us at Freenode IRC channel #packit, or feel free to create an
issue in any of our GitHub projects.

We are also available on this e-mail: user-cont-team@redhat.com.


### The key principles of packit

* Packit aims to make things easy and right. But if the default behavior is not
  the right for you, there is still a way around, but may not be that simple.
  For example you can use
  [actions](/docs/actions/)
  to replace default packit's behavior with a script of yours.

* Reuse existing tools and services where it makes sense: don't reinvent the
  wheel.

* You can consume packit in two forms:
  * Packit tool can run on your laptop and you run commands you want.
  * Packit service reacts to events and performs actions which you
    defined in your `packit.yaml`.

* We don't break backwards compatibility just like that.

* Packit has a deprecation policy:
  * We can mark a behaviour as deprecated.
  * Deprecated content can be removed or changed after at least 3 minor
    releases.
  * Deprecated content is advertised in our
    [changelog](https://github.com/packit-service/packit/blob/master/CHANGELOG.md),
    printed in terminal or tracked in your issue tracker.

* We care about artifacts which Fedora supports: at the moment it's RPMs,
  modules and container images.
  * Our initial focus is solely on RPMs.

* Packit respects Fedora guidelines.

* We want latest content in Fedora Rawhide, but only if it works (the new
  content can be built and tests are passing).

* Any task done by the automation system must be able to be performed by a
  human when that is required. Packit service must be capable of recovering
  from such situation.

* Packit developers must be able to iterate on all parts packit (testing a
  change, merging a change, deploying to production) at a pace of at least
  every two weeks. To accomplish this, the release and validation processes are
  completely automated.

* Contributions to packit must be possible by any developer, maintainer,
  tester, or other engineer. Any Fedora developer or tester should be able to
  reproduce a bot locally on their machine, given appropriate credentials.

<!--more-->


### Why packit?

 * Our intent is to bring downstream and upstream communities closer: provide
   feedback from downstream to upstream. (e.g. *"Hello \<upstream project Y>,
   your newest release doesn't work in Fedora Rawhide, it breaks \<Z>, here is
   a link to logs."*)

 * We want to only merge, build and compose components which integrate well
   with the rest of the operating system. The biggest impact of such behavior
   will be on Fedora Rawhide and when working on a new Fedora release.

 * Automatically pull and validate new upstream releases. This can be a trivial
   thing to do, why should maintainers waste their times on work which can be
   automated.

 * Developing in dist-git is cumbersome. Editing patch files and moving
   tarballs around is not fun. Why not working with the source code itself?
   With [source-git](/source-git/), you'll have upstream git history and the
   dist-git content combined in a single repository.

 * Let's use modern development techniques such as pull requests, code review,
   modern git forges, automation and continuous integration. We have computers
   to do all the mundane tasks. Why we, as humans, should do such work?

 * We want dist-git to be "a database of content in a release" rather a place
   to do actual work. On the other hand, you'll still be able to interact with
   dist-git the same way. We are not taking that away.
   [Source-git](/source-git/) is meant to be the modern, better alternative.

DevConf.cz ["Auto-maintain your package" talk](https://www.youtube.com/watch?v=KpF27v6K4Oc).
