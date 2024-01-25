```
Upload Errors:
  Directory Errors:
    ? examples/dataset-examples/bad-codex-akoya-directory-v1-missing-dataset.json/upload/name-just-needs-to-end-with-metadata.tsv,
      column 'data_path', value 'dataset-1'
    : ? examples/dataset-examples/bad-codex-akoya-directory-v1-missing-dataset.json/upload/dataset-1
        (as codex-v1-with-dataset-json)
      : Required but missing:
        - (raw|src_[^/]*)/dataset\.json.
Metadata TSV Validation Errors:
  Local Validation Errors:
    ? examples/dataset-examples/bad-codex-akoya-directory-v1-missing-dataset.json/upload/name-just-needs-to-end-with-metadata.tsv
      (as codex-v1)
    : - 'On row 2, column "donor_id", value "ABC123" fails because it does not match
        the expected pattern. Example: SNT123.ABCD.567'
      - 'On row 2, column "tissue_id", value "ABC123-RK-1_1" fails because it does
        not match the expected pattern. Example: SNT890.EFGH.321'
Hint: 'If validation fails because of extra whitespace in the TSV, try:

  src/cleanup_whitespace.py --tsv_in original.tsv --tsv_out clean.tsv.'
```
