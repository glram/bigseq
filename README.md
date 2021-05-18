# bigseq
A port of the BIGSI database to the Seq language.

COVID sequence for benchmarking comes from https://www.ncbi.nlm.nih.gov/sra/ERX5420434[accn]

Team Members: Gabe Ramirez, Kaveri Nadhamuni, Charvi Gopal

## Installation
1. Clone the repo.
2. Install Seq, ensuring that it is in your `$PATH` and that `$LD_LIBRARY_PATH` contains `{seq_installation_directory}/lib/seq`
```bash
/bin/bash -c "$(curl -fsSL https://seq-lang.org/install.sh)"
```
3. Install BIGSI's required libraries. See [their docs](https://bigsi.readme.io/docs).
4. Compile the `bigseq` binary.
```bash
cd bigseq
seqc build -release bigseq.seq -o=bigseq
```
5. Set `SEQ_PYTHON` to the output of `python3 find.py`.
6. Run `bigseq`.

## Commands
- `bloom <ctx_file> <out_file>`: constructs a bloom filter
- `build -b <bloom_file> -s <sample_name> ...`: builds an index
- `search <seq>`: searches for a matching sample

## Licenses
See `licenses` directory and report.
