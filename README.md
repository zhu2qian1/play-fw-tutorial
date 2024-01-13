# Play Framework Tutorial

Reference: [Introduction to the Play](https://www.baeldung.com/scala/play-framework-intro)

## Prerequisites

- scala (2.13.12)
- scala-cli
- coursier
- sbt
- SDKMAN!

## Environment setup

On installation, an error occured:

```bash
$ sbt new playframework/play-scala-seed.g8
java.lang.RuntimeException: Retrieval of org.scala-sbt.sbt-giter8-resolver:sbt-giter8-resolver:0.16.2 failed.
        at scala.sys.package$.error(package.scala:30)
        at sbt.TemplateCommandUtil$.classpathForInfo(TemplateCommandUtil.scala:158)
        at sbt.TemplateCommandUtil$.infoLoader(TemplateCommandUtil.scala:118)
        at sbt.TemplateCommandUtil$.$anonfun$run$1(TemplateCommandUtil.scala:79)
        at sbt.TemplateCommandUtil$.$anonfun$run$1$adapted(TemplateCommandUtil.scala:78)
        at scala.collection.LinearSeqOptimized.find(LinearSeqOptimized.scala:115)
        at scala.collection.LinearSeqOptimized.find$(LinearSeqOptimized.scala:112)
        at scala.collection.immutable.List.find(List.scala:91)
        at sbt.TemplateCommandUtil$.run(TemplateCommandUtil.scala:78)
        at sbt.TemplateCommandUtil$.runTemplate(TemplateCommandUtil.scala:54)
        at sbt.TemplateCommandUtil$.$anonfun$templateCommand0$2(TemplateCommandUtil.scala:31)
        at sbt.Command$.$anonfun$applyEffect$4(Command.scala:151)
        at sbt.Command$.$anonfun$applyEffect$2(Command.scala:146)
        at sbt.Command$.process(Command.scala:190)
        at sbt.MainLoop$.$anonfun$processCommand$5(MainLoop.scala:246)
        at scala.Option.getOrElse(Option.scala:189)
        at sbt.MainLoop$.process$1(MainLoop.scala:246)
        at sbt.MainLoop$.processCommand(MainLoop.scala:277)
        at sbt.MainLoop$.$anonfun$next$5(MainLoop.scala:164)
        at sbt.State$StateOpsImpl$.runCmd$1(State.scala:290)
        at sbt.State$StateOpsImpl$.process$extension(State.scala:326)
        at sbt.MainLoop$.$anonfun$next$4(MainLoop.scala:164)
        at sbt.internal.util.ErrorHandling$.wideConvert(ErrorHandling.scala:24)
        at sbt.MainLoop$.next(MainLoop.scala:164)
        at sbt.MainLoop$.run(MainLoop.scala:145)
        at sbt.MainLoop$.$anonfun$runWithNewLog$1(MainLoop.scala:120)
        at sbt.io.Using.apply(Using.scala:28)
        at sbt.MainLoop$.runWithNewLog(MainLoop.scala:113)
        at sbt.MainLoop$.runAndClearLast(MainLoop.scala:67)
        at sbt.MainLoop$.runLoggedLoop(MainLoop.scala:52)
        at sbt.MainLoop$.runLogged(MainLoop.scala:43)
        at sbt.StandardMain$.runManaged(Main.scala:225)
        at sbt.xMain$.$anonfun$run$9(Main.scala:115)
        at sbt.io.IO$.withTemporaryDirectory(IO.scala:496)
        at sbt.io.IO$.withTemporaryDirectory(IO.scala:506)
        at sbt.xMain$.run(Main.scala:102)
        at java.base/jdk.internal.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
        at java.base/jdk.internal.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:77)
        at java.base/jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
        at java.base/java.lang.reflect.Method.invoke(Method.java:568)
        at sbt.internal.XMainConfiguration.run(XMainConfiguration.java:59)
        at sbt.xMain.run(Main.scala:47)
        at xsbt.boot.Launch$.$anonfun$run$1(Launch.scala:149)
        at xsbt.boot.Launch$.withContextLoader(Launch.scala:176)
        at xsbt.boot.Launch$.run(Launch.scala:149)
        at xsbt.boot.Launch$.$anonfun$apply$1(Launch.scala:44)
        at xsbt.boot.Launch$.launch(Launch.scala:159)
        at xsbt.boot.Launch$.apply(Launch.scala:44)
        at xsbt.boot.Launch$.apply(Launch.scala:21)
        at xsbt.boot.Boot$.runImpl(Boot.scala:78)
        at xsbt.boot.Boot$.run(Boot.scala:73)
        at xsbt.boot.Boot$.main(Boot.scala:21)
        at xsbt.boot.Boot.main(Boot.scala)
```

installed scala-cli and courseir setup, the problem fixed.
