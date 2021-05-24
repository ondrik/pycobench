# pycobench
A small Python framework for running benchmarks.

Contents:
* `bin/pycobench`: The main script for running benchmarks
* `bin/pyco_proc`: The script for processing the output of `pycobench` into a table
* `examples/ba-compl.yaml`: Example of a YAML file for configuring what to run
* `examples/ba-all.input`: Example of a file with input benchmarks

How to run:
```
cat benchmarks.input | ./pycobench -c config.yaml -j JOBS -t TIMEOUT -o OUTPUT_FILE
```
When the benchmarks finish, you can process the results by
```
cat OUTPUT_FILE | ./pyco_proc --csv > OUTPUT_CSV
```
