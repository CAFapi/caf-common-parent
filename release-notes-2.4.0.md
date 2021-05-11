#### Version Number
${version-number}

#### New Features
- **SCMOD-12630**: Add **_BanDuplicatePomDependencyVersions_**  
This has been included as part of the `maven-enforcer-plugin` within `enforceBannedDependencies` and will check for dependency duplicates, failing the build if `enforceBannedDependencies` property is set to true.

#### Known Issues
- None
