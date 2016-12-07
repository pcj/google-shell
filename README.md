# google-shell [![Build Status](https://travis-ci.org/pcj/google-shell.svg?branch=master)](https://travis-ci.org/pcj/google-shell)

<table><tr>
<td><img src="https://avatars0.githubusercontent.com/u/1342004?v=3&s=200" width="120"/></td>
<td><img src="http://cdn.osxdaily.com/wp-content/uploads/2014/08/terminal-icon-osx.png" width="120"/></td>
</tr><tr>
<td>Google</td>
<td>Shell</td>
</tr></table>

This is the command-line shell script runner from the
[Bazel Project](http://bazel.build).  The
`com.google.devtools.build.lib.shell` package has been split out into
a separate jar for general utility.

# Installation

Bazel

```python
git_repository(
  name = "com_github_pcj_google_shell",
  remote = "https://github.com/pcj/google-shell.git",
  commit = "HEAD", # replace with actual sha1
)

bind(
  name = "google_shell",
  actual = "@com_github_pcj_google_shell//src/main/java/com/google/devtools/build/lib/shell",
)
```

Maven/Gradle/...

> Note: *the maven artifact is not yet available*.

```markup
<dependency>
  <groupId>com.github.pcj</groupId>
  <artifactId>google-shell</artifactId>
  <version>1.0.0</version>
</dependency>
```

# Usage

Please consult the
[tests](src/test/java/com/google/devtools/build/lib/shell/) and
[source code](src/main/java/com/google/devtools/build/lib/shell/) for
more detailed information.
