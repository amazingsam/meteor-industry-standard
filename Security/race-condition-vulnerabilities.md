#Race Condition Vulnerabilities

**Affected Versions**

Meteor on current NodeJS versions

**Expected Solutions**

Future NodeJS will deprecate the fs.exists family/

**Workarounds**

Do not use fs.exists(), fs.existsSync() from the NodeJS fs module. Instead, use fs.open.

##Description
The methods fs.exists() and fs.existsSync are anachronisms and exists only for historical reasons. There should be no reason to use it in your code. Checking if a file exists before opening it is an anti-pattern that leaves you vulnerable to race conditions: another process may remove the file between the calls to fs.exists() and fs.open()

##Related Sources
[Node.js v0.12.7 Manual & Documentation](https://nodejs.org/api/fs.html#fs_fs_existssync_path) from NodeJS
