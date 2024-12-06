<!---
 Licensed to the Apache Software Foundation (ASF) under one or more
 contributor license agreements.  See the NOTICE file distributed with
 this work for additional information regarding copyright ownership.
 The ASF licenses this file to You under the Apache License, Version 2.0
 (the "License"); you may not use this file except in compliance with
 the License.  You may obtain a copy of the License at

      http://www.apache.org/licenses/LICENSE-2.0

 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
-->
Contributing to [Apache Software Foundation Parent POM](https://maven.apache.org/pom/asf/)
======================

[![Apache License, Version 2.0, January 2004](https://img.shields.io/github/license/apache/maven.svg?label=License)][license]
[![Maven Central](https://img.shields.io/maven-central/v/org.apache/apache.svg?label=Maven%20Central)](https://search.maven.org/artifact/org.apache/apache)
[![Jenkins Status](https://img.shields.io/jenkins/s/https/ci-maven.apache.org/job/Maven/job/maven-box/job/maven-apache-parent/job/master.svg)][build]
[![Verify](https://github.com/apache/maven-apache-parent/actions/workflows/maven-verify.yml/badge.svg)](https://github.com/apache/maven-apache-parent/actions/workflows/maven-verify.yml)

Have you found a bug or have an idea for a cool new feature? Contributing
code is a great way to give something back to the open source community. Before
you dig right into the code, there are a few guidelines that we need
contributors to follow so that we can have a chance of keeping on top of
things.

Getting Started
---------------

+ Make sure you have a [GitHub account](https://github.com/signup).
+ If you're planning to implement a new feature, please discuss your changes 
  on the [developer mailing list][ml-list] first. 
  This way you can make sure you're not wasting your time on something that isn't 
  considered to be in Apache Maven's scope.
+ Submit a ticket for your issue, assuming one does not already exist.
  + Clearly describe the issue, including steps to reproduce when it is a bug.
  + Make sure you fill in the earliest version that you know has the issue.
+ Fork the repository on GitHub.

Making and Submitting Changes
--------------

We accept Pull Requests via GitHub. The [developer mailing list][ml-list] is the
main channel of communication for contributors.  
There are some guidelines which will make applying PRs easier for us:
+ Create a topic branch from where you want to base your work (this is usually the master branch).
  Push your changes to a topic branch in your fork of the repository.
+ Make commits of logical units.
+ Respect the original code style: by using the same [codestyle][code-style],
  patches should only highlight the actual difference, not being disturbed by any formatting issues:
  + Only use spaces for indentation.
  + Create minimal diffs - disable on save actions like reformat source code or organize imports. 
    If you feel the source code should be reformatted, create a separate PR for this change.
  + Check for unnecessary whitespace with `git diff --check` before committing.
+ Make sure your commit messages are in the proper format. Your commit message should contain the key of the issue.
```
[#issue-number] - Subject of the issue
 Optional supplemental description.
```
+ Update the [site documentation](https://maven.apache.org/pom/asf/) accordingly in `docs/src/site` and build it via `mvn site -f docs`
+ Submit a pull request to the repository in the Apache organization.

If you plan to contribute on a regular basis, please consider filing a [contributor license agreement][cla].

Making Trivial Changes
----------------------

For changes of a trivial nature to comments and documentation, or other simple changes
it is not always necessary to create a new issue.  
In this case, it is appropriate to skip the issue from a commit message.

Additional Resources
--------------------

+ [Contributing patches](https://maven.apache.org/guides/development/guide-maven-development.html#Creating_and_submitting_a_patch)
+ [Contributor License Agreement][cla]
+ [General GitHub documentation](https://docs.github.com/)
+ [GitHub pull request documentation](https://docs.github.com/pull-requests)
+ [Apache Maven Twitter Account](https://twitter.com/ASFMavenProject)

[license]: https://www.apache.org/licenses/LICENSE-2.0
[ml-list]: https://maven.apache.org/mailing-lists.html
[code-style]: https://maven.apache.org/developers/conventions/code.html
[cla]: https://www.apache.org/licenses/#clas
[build]: https://ci-maven.apache.org/job/Maven/job/maven-box/job/maven-apache-parent/job/master/
