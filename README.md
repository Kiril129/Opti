# Opti
Opti
#!/bin/sh
. "$(dirname "$0")/_/husky.sh"

yarn lerna run --concurrency 1 --stream pre-commit --since HEAD --exclude-dependents
