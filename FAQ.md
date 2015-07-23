Q: Meteor's build takes a really long time once you reach a project of any reasonable size.

A: ...

Q: Is it possible to create a package that serves to exclude a whole folder from becoming part of production builds? Could be a folder with a specific name or containing a specific config file, but the contents of which are only relevant during development.

A: You can start any file or directory with dot ('.') and they won't include in the build.
