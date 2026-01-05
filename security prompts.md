##Security:

```
Perform a full audit of authentication, authorization, and secrets. Document findings in security[.]md


```
Reverse-engineer the permission model. List roles, objects, and allowed actions in permissions[.]md'''

```
Check for unauthorized data access. Compare actual behavior vs permissions[.]md'''

```
Reverse-engineer the codebase vs, OWASP Top 10. Document risks, priorities, fixes, and why in owasp10[.]md'''

Performance:

```
Identify routes that fetch unnecessary data or block on sequential queries. Can we cache, prefetch, or parallelize?
'''


```
Review edge functions and related tables. Where can indexes, parallel queries, or denormalization improve performance? Document priorities in performance[.]md'''

```
Why does [view] take 2-3 seconds to load? Analyze code, network, logs, and queries. Propose fixes with why and priority.'''

source: https://substack.com/@huryn/note/c-195448364?r=6xt014&utm_medium=ios&utm_source=notes-share-action