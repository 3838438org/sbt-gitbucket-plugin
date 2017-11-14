sbt-gitbucket-plugin
========

This sbt plugin supports GitBucket plugin development.

Add a following line to your GitBucket plugin's `project/plugin.sbt`:

```scala
addSbtPlugin("io.github.gitbucket" % "sbt-gitbucket-plugin" % "0.1-SNAPSHOT")
```

and define the target GitBucket version in `build.sbt`:

```scala
gitbucketVersion := "4.18.0"
```

This plugin provides following functionality in your GitBucket plugin project: 

- Add GitBucket core library dependency to the project as "provided" scope
- Enable [sbt-assembly](https://github.com/sbt/sbt-assembly) plugin to package your GitBucket plugin
- Enable `sbt install` task to build and install the GitBucket plugin to the local GitBucket instance

### TODO

- Enable sbt-twirl plugin automatically
- Generate a plugin manifest file for network installation
