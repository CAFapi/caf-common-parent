!not-ready-for-release!

#### Version Number
${version-number}

#### New Features
- **US361030**: Plugin versions updated  
  The Maven plugins have been updated to their latest versions.

#### Breaking Changes
- Java version update  
  Java 17 is now the default target.  This can be overridden by setting the
  `maven.compiler.release` property.

- Java EE banned  
  The Java EE artifacts have been added to the list of banned dependencies.
  It has been many years since the move to Jakarta EE so this is being added to
  the banned list to prevent any accidental reintroduction.

- Enforce correct dependencies  
  The `enforceCorrectDependencies` flag has been enabled by default.

- Enforce compatible dependencies  
  Conflicts between dependencies will now cause the build to fail.  These can be
  ignored by setting the `enforceCompatibleDependencies` flag to `false`.

- License header configuration changes  
  There have been a number of changes to the default license headers configuration.
  The new `<licenseSets>` option is being used for configuration so any overrides
  will also have to be similarly updated.

- Banned inapplicable test artifacts  
  The `hamcrest-all` and `mockito-all` artifacts have been banned since they are
  not meant to be used with dependency management systems like Maven.

#### Known Issues
