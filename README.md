# Gradle2Ant

Simple Ant libraries to enable running Gradle tasks from within Ant build scripts. Ant macros used to enable user to
directly use them in simple Ant targets using really simple parameters!

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

## plugins/Gradle2Ant-WAR.xml

Abstract macro based on the task provided by the Gradle WAR plugin for creating web archives:

- war (macro *gradle.war*)

Can be imported into any Ant build script using:
```xml
<import file="${path.to.libraries}/plugins/Gradle2Ant-WAR.xml" />
```

## plugins/Gradle2Ant-EAR.xml

Abstract macro based on the task provided by the Gradle EAR plugin for creating enterprise archives:

- ear (macro *gradle.ear*)

Can be imported into any Ant build script using:
```xml
<import file="${path.to.libraries}/plugins/Gradle2Ant-EAR.xml" />
```

## plugins/Gradle2Ant-Groovy.xml

Abstract macros based on the tasks provided by the Gradle Groovy plugin when using Groovy when developing:

- compileGroovy (macro *gradle.compileGroovy*)
- compileTestGroovy (macro *gradle.compileTestGroovy*)

Can be imported into any Ant build script using:
```xml
<import file="${path.to.libraries}/plugins/Gradle2Ant-Groovy.xml" />
```

## plugins/Gradle2Ant-JaCoCo.xml

Abstract macros based on the tasks provided by the Gradle JaCoCo plugin when checking code for coverage based on the
results of the Gradle tasks of type *Test*:

- jacocoTestReport (macro *gradle.jacocoTestReport*)
- jacocoTestCoverageVerification (macro *gradle.jacocoTestCoverageVerification*)

Can be imported into any Ant build script using:
```xml
<import file="${path.to.libraries}/plugins/Gradle2Ant-JaCoCo.xml" />
```

## plugins/Gradle2Ant-SonarQube.xml

Abstract macro based on the task provided by the unofficial Gradle SonarQube plugin when running a static code analysis
on the given source code:

- sonarqube (macro *gradle.sonarqube*)

Can be imported into any Ant build script using:
```xml
<import file="${path.to.libraries}/plugins/Gradle2Ant-SonarQube.xml" />
```

## plugins/Gradle2Ant-RunTestsSeparateJVM.xml

Abstract macros based on the tasks provided by the unofficial Gradle RunTestsSeparateJVMPlugin plugin when running
jUnit tests eather in separate JVM sequentially or in parallel

- testSeparateJVMSequentially (macro *gradle.testSeparateJVMSequentially*)
- testSeparateJVMInParallel (macro *gradle.testSeparateJVMInParallel*)

Can be imported into any Ant build script using:
```xml
<import file="${path.to.libraries}/plugins/Gradle2Ant-RunTestsSeparateJVM.xml" />
```
