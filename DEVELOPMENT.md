# Release Procedure

* `git switch main && git pull`
* `npm version [major|minor|patch]`
    * This generates a new tag.
* `git push origin main`
* `git push origin [tag]`
* `npm login`
* `npm publish --dry-run`
* `npm publish`
* `npm logout`
* Create a release in Github.
    * Push `Draft a new release` button in https://github.com/mmktomato/parcel-reporter-web-ext/releases
