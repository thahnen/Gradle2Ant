# Gradle2Ant

Simple Ant libraries to enable running Gradle tasks from within Ant build scripts. Ant macros used
to enable user to directly use them in simple Ant targets using really simple parameters!

For more information take a look [here](https://github.com/thahnen/Gradle2Ant)!

## Gradle2Ant.xml

Defines the basic *gradle* macro used in all other macros througout this Ant library and the ones below!

Abstract macros based on the tasks provided by the Gradle Java plugin:

- classes (macro *gradle.classes*)
- testClasses (macro *gradle.testClasses*)
- jar (macro *gradle.jar*)
- test (macro *gradle.test*)
- clean (macro *gradle.clean*)
- javadoc (macro *gradle.javadoc*)

Can be imported into any Ant build script using:
```xml
<import file="${path.to.libraries}/Gradle2Ant.xml" />
```

## ide/Gradle2Ant-Eclipse.xml

Abstract macros based on the tasks provided by the Gradle Eclipse plugin for generating Eclipse
configuration files:

- eclipse (macro *gradle.eclipse*)
- cleanEclipse (macro *gradle.cleanEclipse*)

Can be imported into any Ant build script using:
```xml
<import file="${path.to.libraries}/ide/Gradle2Ant-Eclipse.xml" />
```

## ide/Gradle2Ant-IDEA.xml

Abstract macros based on the tasks provided by the Gradle IDEA plugin for generating IntelliJ IDEA
configuration files:

- idea (macro *gradle.idea*)
- openIdea (macro *gradle.openIdea*)
- cleanIdea (macro *gradle.cleanIdea*)

Can be imported into any Ant build script using:
```xml
<import file="${path.to.libraries}/ide/Gradle2Ant-IDEA.xml" />
```

## ide/Gradle2Ant-VisualStudio.xml

Abstract macros based on the tasks provided by the Gradle Visual Studio plugin for generating
Visual Studio configuration files:

- visualStudio (macro *gradle.visualStudio*)
- openVisualStudio (macro *gradle.openVisualStudio*)
- cleanVisualStudio (macro *gradle.cleanVisualStudio*)

Can be imported into any Ant build script using:
```xml
<import file="${path.to.libraries}/ide/Gradle2Ant-VisualStudio.xml" />
```

## ide/Gradle2Ant-XCode.xml

Abstract macros based on the tasks provided by the Gradle XCode plugin for generating XCode
configuration files:

- xcode (macro *gradle.xcode*)
- openXcode (macro *gradle.openXcode*)
- cleanXcode (macro *gradle.cleanXcode*)

Can be imported into any Ant build script using:
```xml
<import file="${path.to.libraries}/ide/Gradle2Ant-XCode.xml" />
```

## plugins/official/Gradle2Ant-WAR.xml

Abstract macro based on the task provided by the Gradle WAR plugin for creating web archives:

- war (macro *gradle.war*)

Can be imported into any Ant build script using:
```xml
<import file="${path.to.libraries}/plugins/official/Gradle2Ant-WAR.xml" />
```

## plugins/official/Gradle2Ant-EAR.xml

Abstract macro based on the task provided by the Gradle EAR plugin for creating enterprise archives:

- ear (macro *gradle.ear*)

Can be imported into any Ant build script using:
```xml
<import file="${path.to.libraries}/plugins/official/Gradle2Ant-EAR.xml" />
```

## plugins/official/Gradle2Ant-Groovy.xml

Abstract macros based on the tasks provided by the Gradle Groovy plugin when using Groovy when developing:

- compileGroovy (macro *gradle.compileGroovy*)
- compileTestGroovy (macro *gradle.compileTestGroovy*)
- groovydoc (macro *gradle.groovydoc*)

Can be imported into any Ant build script using:
```xml
<import file="${path.to.libraries}/plugins/official/Gradle2Ant-Groovy.xml" />
```

## plugins/official/Gradle2Ant-Scala.xml

Abstract macros based on the tasks provided by the Gradle Scala plugin when using Scala when developing:

- compileScala (macro *gradle.compileScala*)
- compileTestScala (macro *gradle.compileTestScala*)
- scaladoc (macro *gradle.scaladoc*)

Can be imported into any Ant build script using:
```xml
<import file="${path.to.libraries}/plugins/official/Gradle2Ant-Scala.xml" />
```

## plugins/official/Gradle2Ant-Application.xml

Abstract macros based on the tasks provided by the Gradle Application for running and creating
(distributable) applications:

- run (macro *gradle.run*)
- startScripts (macro *gradle.startScripts*)
- installDist (macro *gradle.installDist*)
- distZip (macro *gradle.distZip*)
- distTar (macro *gradle.distTar*)

Can be imported into any Ant build script using:
```xml
<import file="${path.to.libraries}/plugins/official/Gradle2Ant-Application.xml" />
```

## plugins/official/Gradle2Ant-JaCoCo.xml

Abstract macros based on the tasks provided by the Gradle JaCoCo plugin when checking code for
coverage based on the results of the Gradle tasks of type *Test*:

- jacocoTestReport (macro *gradle.jacocoTestReport*)
- jacocoTestCoverageVerification (macro *gradle.jacocoTestCoverageVerification*)

Can be imported into any Ant build script using:
```xml
<import file="${path.to.libraries}/plugins/official/Gradle2Ant-JaCoCo.xml" />
```

## plugins/inofficial/Gradle2Ant-SonarQube.xml

Abstract macro based on the task provided by the unofficial Gradle SonarQube plugin when running a
static code analysis on the given source code:

- sonarqube (macro *gradle.sonarqube*)

Can be imported into any Ant build script using:
```xml
<import file="${path.to.libraries}/plugins/inofficial/Gradle2Ant-SonarQube.xml" />
```

## plugins/inofficial/Gradle2Ant-RunTestsSeparateJVM.xml

Abstract macros based on the tasks provided by the unofficial Gradle RunTestsSeparateJVMPlugin
plugin when running jUnit tests eather in separate JVM sequentially or in parallel

- testSeparateJVMSequentially (macro *gradle.testSeparateJVMSequentially*)
- testSeparateJVMInParallel (macro *gradle.testSeparateJVMInParallel*)

Can be imported into any Ant build script using:
```xml
<import file="${path.to.libraries}/plugins/inofficial/Gradle2Ant-RunTestsSeparateJVM.xml" />
```
