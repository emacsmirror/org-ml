# Changelog

## 5.0.1

- rearrange reference files
- use buttercup for testing

## 5.0.0

- add robust headline logbook and contents function
- rename indent/unindent functions to better reflect native org function naming
  conventions
- add `org-ml-from-string`
- improve subtree parsing performance
- fix whitespace errors for
  `org-ml-headline-set-planning/node-properties/supercontents` functions

## 4.0.1

- fix `org-ml-parse-this-table-row` and `org-ml-parse-table-row-at`
  beyond first row of table

## 4.0.0

- add `org-ml-get-parents`
- add `org-ml-headline-get-logbook-loose` and `org-ml-headline-get-contents`
- removed old `org-ml-headline-X-logbook` functions and replaced them with
  `org-ml-headline-X-logbook-drawer` which can be made aware of other drawers
  other than "LOGBOOK" or nothing
- add `org-ml-clone-n`

## 3.0.2

- Update dependencies
- Fix bugs

## 3.0.1

- Fix bugs
  - Don't use `nreverse` unless needed
  - Don't crash when `org-ml-headline-get-node-property` should return nil

## 3.0.0

- Update for org-mode 9.3

## 2.0.1

- Fixed byte compile
- Clean up docstrings

## 2.0.0 

- Renamed from `om.el` to `org-ml` (org-metalanguage)
- Renamed functions to be more consistent
  - `org-ml-get-headlines` and friends to `org-ml-parse-headlines`
  - `org-ml-do-headlines` and friends to `org-ml-update-headlines`
- Add POSIX ERE-like regexp syntax to `org-ml-match` and friends
- Add affiliated keyword support
- Numerous bug fixes