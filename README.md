# test

A scratch repository used to exercise the **dsh-superagent** GitHub integration: issues
and comments that mention the agent account become work items, and the agent answers
in the same thread with a pull request.

## How a request starts

Comment on an issue or pull request and mention the agent account:

```
@kafeim Please fix the typo in the first paragraph.
```

The agent picks the request up on its next poll, records a ticket, and reports back in
the same conversation. Work it decides to do lands on a branch named `agent/<name>` and
a pull request opened against `main`.

## Scope

Everything here is disposable: the repository exists so the integration can be tried on
a small, safe surface before it touches a real project.
