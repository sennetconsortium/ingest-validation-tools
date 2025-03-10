## Manual Testing for Next-Gen Templates

Currently, testing for metatdata templates hosted by CEDAR needs to be run manually. Automated testing does not hit the CEDAR API.

To test CEDAR validation including API calls, run the following from the top-level directory:

# ./tests-manual/test-dataset-examples-cedar.sh <globus_token> <start_index>

- $1 = globus_token: you can find your personal Globus token by logging in to a site that requires Globus authentication (e.g. https://ingest.hubmapconsortium.org/) and looking at the Authorization header for your request in the Network tab of your browser. Omit the "Bearer " prefix.
- $2 = start_index (optional): to avoid hitting APIs continuously when re-running tests, you can provide an index (starting at 1) (# TODO: should probably be 0) to start at a specific test.

## Manual Testing for Plugins

Plugins live in [https://github.com/hubmapconsortium/ingest-validation-tests](https://github.com/hubmapconsortium/ingest-validation-tests), requiring them to be tested manually rather than being added to automatic testing suite. To test plugins, first make sure you have [ingest-validation-tests properly installed](https://github.com/hubmapconsortium/ingest-validation-tools#running-plugin-tests).

Then, run the following from the top-level directory:

# ./tests-manual/test-plugins.sh

## Creating Tests

All examples with CEDAR API validation will need a README_ONLINE.md file. The test script will try to detect whether this file is missing based on example names including the string "cedar," but may not be 100% reliable.
