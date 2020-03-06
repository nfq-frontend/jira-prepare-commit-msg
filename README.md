# jira-prepare-commit-msg

Husky command to add JIRA ticket ID into the commit message if it is missed.

The JIRA ticket ID is taken from a git branch name.

## Installation

Install the package using NPM

```bash
npm i -D husky nfq-jira-prepare-commit-msg
```

## Configuration

Inside your package.json add a standard husky npm script for the git hook:

```json
{
  "husky": {
    "hooks": {
      "prepare-commit-msg": "nfq-jira-prepare-commit-msg"
    }
  }
}
```

## Supported pattern

The following patterns are currently supported:

* /([A-Z]+-\d+)/i

## TODO

- [ ] Support user patterns
- [ ] Support configuration (package.json)
- [x] Lint
- [x] Tests

## License

MIT
