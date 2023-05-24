```
Metadata TSV Errors:
  ? examples/dataset-examples/bad-codex-akoya-directory-v1-missing-dataset.json/upload/name-just-needs-to-end-with-metadata.tsv
    (as codex)
  : Internal:
    - On row 2, column "donor_id", value "ABC123" fails because constraint "pattern"
      is "[SNT]+\d{3}\.[A-Za-z]{4}\.\d{3}"
    - On row 2, column "tissue_id", value "ABC123-RK-1_1" fails because constraint
      "pattern" is "[SNT]+\d{3}\.[A-Za-z]{4}\.\d{3}"
    External:
      row 2, data examples/dataset-examples/bad-codex-akoya-directory-v1-missing-dataset.json/upload/dataset-1:
        Required but missing:
        - (raw|src_[^/]*)/dataset\.json
Hint: 'If validation fails because of extra whitespace in the TSV, try:

  src/cleanup_whitespace.py --tsv_in original.tsv --tsv_out clean.tsv'
```
