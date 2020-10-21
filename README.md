# simple-semver

A github action to increment a semver string consisting of MAJOR, MINOR and PATCH numbers.

## Usage

```yaml
- name: Simple Semver
  id: semver
  uses: matt-FFFFFF/simple-semver@v0.0.1
  with:
    semver-input: '1.2.2344234'
    increment: p

- name: Use new semver
  run: echo ${{ steps.semver.outputs.semver }}
```
