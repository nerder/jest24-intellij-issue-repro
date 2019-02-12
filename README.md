### Bug description

Running the test using the Intellij Idea interface not working properly when `jest` is on the version `24`.

```bash
/usr/local/bin/node --require "/Applications/IntelliJ IDEA.app/Contents/plugins/JavaScriptLanguage/helpers/jest-intellij/lib/jest-intellij-stdin-fix.js" /Users/`$USER`/Development/Tests/intellij-issue-repro/node_modules/jest/bin/jest.js --colors --reporters "/Applications/IntelliJ IDEA.app/Contents/plugins/JavaScriptLanguage/helpers/jest-intellij/lib/jest-intellij-reporter.js" --verbose --testPathPattern ^/Users/$USER/Development/Tests/intellij-issue-repro/test\.js$ "--testNamePattern=^thing "
```
Up to version `23.6` the bug is not present and tests run normally.


### Workaround

Adding `_JB_INTELLIJ_JASMINE_REPORTER_DISABLED=true` as Environmental
