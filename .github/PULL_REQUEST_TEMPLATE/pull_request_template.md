## JIRA Reference
[comment]: <> (Jira ticket reference)

## Change Summary

[comment]: <> (What's changed and why - reference the jira ticket where appropriate.)

## Code Review 

### Concerns

[comment]: <> (Add any specific areas of concern where you would like review input.)

### Checklist

[comment]: <> (Delete Sections that don't apply.)

#### General
- [ ] Does the implementation satisfy the requirements?
- [ ] Beyond linting, is the code easy to read and understand? Are naming choices appropriate, descriptive and consistent with other parts of the system?
- [ ] Is the code tested, and do the tests adequately cover the requirements?
- [ ] Is the code documented? 
- [ ] Are there any hard coded configuration items?
- [ ] Is the code tightly coupled to other systems, in a way that would make it difficult to maintain?
- [ ] Is the code using new external libraries, that have not been captured and assessed as part of the SOUP management process?
- [ ] Are there obvious security vulnerabilities; eg: use of free text passwords/keys
- [ ] Is there any unnecessary duplication, either within the change, or of an existing module or standard library?
- [ ] Is the data structure choice appropriate?
- [ ] Does the code have any memory leaks? e.g. data structures that are continually added to, but never removed from?
- [ ] Has thought been given to handling of exceptions?
- [ ] Is the logging adequate for debugging in production?

#### Bugfix
- [ ] Does the change contain a test that would fail, if the bug was reintroduced?
- [ ] Does the change address potentially related bugs? e.g. if the bug was caused by some user input error, does the fix address other possible invalid input?
- [ ] Has the bug been fixed system wide? e.g. are there other parts of the code base with the same issue? Does the fix push the problem to another part of the system by mistake?


#### Performance
- [ ] Is the difference in performance well understood; i.e. before and after performance improvement? 
- [ ] Is the optimization worth the additional complexity?

See the [Pull Requests](https://github.com/franklin-ai/engineering-handbook/blob/main/process/source_control.md#pull-requests) for more info.
