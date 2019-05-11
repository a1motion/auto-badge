# auto-badge

## Usage

1. **[Configure the GitHub App](https://github.com/apps/auto-badge)**
2. Create `.github/badge.yml` based on the following template.
3. It will listen for pull request changes and auto-label them based on your configuration.

```yml
An object constisting on conventional commit types with either a string or a object based on scopes
types:
  fix:
    ui: 'My UI Fix Label'
    api: 'API Fixed!'
    default: 'There was no scope attached'
  feat: 'I cover all features'
```

> Auto Badge will preserve already existing labels, even if it was the one that created it. This may change in the future.
