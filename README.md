# bigseq
A port of the BIGSI database to the Seq language.

COVID sequence for benchmarking comes from https://www.ncbi.nlm.nih.gov/sra/ERX5420434[accn]

Benchmarking Procedure for BIGSI:
- Running BIGSI tutorial (https://bigsi.readme.io/docs/your-first-bigsi) with the FASTA of the COVID sequence

Benchmarking Procedure for BIGSeq:

how to run:
- download seq 
- pythonpath??? seqpath??
- commands to run:

    - seqc run bigseq/bigseq.seq bloom example-data/test1.ctx example-data/test1.bloom
    - seqc run bigseq/bigseq.seq bloom example-data/test2.ctx example-data/test2.bloom
    - seqc run bigseq/bigseq.seq build -b example-data/test1.bloom -b example-data/test2.bloom -s s1 -s s2
    - seqc run bigseq/bigseq.seq search CGGCGAGGAAGCGTTAAATCTCTTTCTGACG

Team Members: Gabe Ramirez, Kaveri Nadhamuni, Charvi Gopal
