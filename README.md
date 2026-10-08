# lib.apache-commons-compress

Apache Commons Compress 1.12 (Apache License 2.0, https://commons.apache.org/proper/commons-compress/),
vendored as a Java library.

Provides `lib.apache-commons-compress`, `apache-commons-compress` and the AE3 package
`ae3.pkg.lib.util.apache-commons-compress` (`export-classpath:java`). Requires `lib.tukaani-xz-java`
for XZ support.

## Layout

- `jars/` - the upstream jar, unmodified.
- `ae3-packages/ae3.pkg.lib.util.apache-commons-compress/` - the AE3 package: `package.json` and its own copy of the jar.
- `incoming/` - the upstream release as downloaded: sources, licence, notices, javadoc.
- `project.inf` - project metadata consumed by distro tooling.

## Updating

Unpack the new upstream release under `incoming/`, replace the jar in both `jars/` folders,
and update the version in the `package.json` title.
