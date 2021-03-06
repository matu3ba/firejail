---
name: Bug report
about: Create a report to help us improve
title: ''
labels: 'review'
assignees: ''

---
Write clear, concise and in textual form.

**Bug and expected behavior**
1. Describe the bug.
2. What did you expect to happen?

**Behavior change on disabling firejail**
3. What changed calling `firejail --noprofile PROGRAM` in a shell?
4. What changed calling the program *by path*=without firejail (check `whereis PROGRAM`, `firejail --list`, `stat $programpath`)?

**To Reproduce**
Steps to reproduce the behavior:
1. Run in bash `firejail PROGRAM`
2. See error `ERROR`
3. Click on '....'
4. Scroll down to '....'

**Desktop (please complete the following information):**
 - Linux distribution and version (ie output of `lsb_release -a`)
 - Firejail version (output of `firejail --version`) exclusive or used git commit (`git rev-parse HEAD`)
 - What other programs interact with the affected program for the functionality?
 - Are these listed in the profile? 

**Additional context**
Other context about the problem like related errors to understand the problem.

**Checklist**
 - [ ] The upstream profile (and redirect profile if exists) have no changes fixing it.
 - [ ] The upstream profile exists (`find / -name 'firejail' 2>/dev/null'/'fd firejail' to locate profiles ie in `/usr/local/etc/firejail/PROGRAM.profile`)
 - [ ] Programs needed for interaction are listed.
 - [ ] Error was checked in search engine and on issue list without success.


<details><summary> debug output </summary>

```
OUTPUT OF `firejail --debug PROGRAM`
```

</details>
