!not-ready-for-release!

#### Version Number
${version-number}

#### New Features
 - Dependency Analysis and Enforcement  
    The `maven-dependency-plugin` has been added to analyze the project's dependencies.  By default warnings are added to the build log if dependency issues are found.

    The `enforceCorrectDependencies` property can be set so that any dependency issues result in build failures:

        <properties>
            <enforceCorrectDependencies>true</enforceCorrectDependencies>
        </properties>

#### Breaking Changes
 - The `integration-test` profile has been removed.
 - The profiles that configured the `caf.integrationtests.fs.path` property have been removed.
 - Custom configuration of the `maven-surefire-plugin` and `maven-failsafe-plugin` have been removed.
 - The reference to the `sonar-maven-plugin` has been removed.
 - Most version control properties have been removed.

#### Known Issues
