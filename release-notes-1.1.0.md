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

#### Known Issues
