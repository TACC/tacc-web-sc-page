# TACC Website Jobs Page

This project creates markup for the body of TACC's SC pages:
- [SC2019](https://www.tacc.utexas.edu/sc19 "TACC: Super Computing 2019")
- [SC2020](https://www.tacc.utexas.edu/sc20 "TACC: Super Computing 2020")
- (coming soon) [SC2021](https://www.tacc.utexas.edu/sc21 "TACC: Super Computing 2021")

<details>It compiles data and templates to create markup to which raw markup is also appended.</details>

## Usage

1. Edit templates and data in:
    - `*.mustache/`
    - `events.*.json`
2. Run build script:
    - __either__ `npm run build` to build everything
    - __or__ `npm run start …` to get a list of commands to build pieces

        <details><summary>Examples</summary>

        - `npm run start build:2021`

            would build all the 2021 page markup (to `dist/`)

        - `npm run start build:2020:partials`

            would build some of the 2020 markup (__not__ to `dist/`)

        - `npm run start build:2019:partials:styles`

            would build only the 2019 `<style />` markup (__not__ to `dist/`)

        </details>
3. Confirm output in:
    - `dist/`
4. Use output.

## Reference

- [How To - Legacy TACC - Markup Generation Utility](https://confluence.tacc.utexas.edu/x/AYGDC)

## Repository History

The first 300 commits of this repository are from a prior BitBucket repo that contained what is now multiple repositories imported from that original repository:

- [tacc-web-content](https://github.com/tacc-wbomar/tacc-web-content)
- [tacc-web-staff-dir](https://github.com/tacc-wbomar/tacc-web-staff-dir)
- [tacc-web-jobs-page](https://github.com/tacc-wbomar/tacc-web-jobs-page)
- [tacc-web-sc19-page](https://github.com/tacc-wbomar/tacc-web-sc19-page)
