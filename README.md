# Arithmetic Benchmark

This is a simple benchmark to compare simple operations:

* Addition
* Subtraction
* Multiplication
* Division
* Modulo

The idea is to have a proper [JMH benchmark](https://openjdk.java.net/projects/code-tools/jmh/) to compare them.

## How to run

    git clone git@github.com:bram-inniger/arithmetic.git
    cd arithmetic
    mvn clean package
    java -jar target/benchmarks.jar -rf text

## Sample result

    Benchmark                           Mode  Cnt   Score   Error  Units
    ArithmeticBenchmark.addition        avgt   25   3.734 ± 0.120  ns/op
    ArithmeticBenchmark.division        avgt   25  16.738 ± 0.141  ns/op
    ArithmeticBenchmark.modulus         avgt   25  16.248 ± 0.075  ns/op
    ArithmeticBenchmark.multiplication  avgt   25   3.702 ± 0.075  ns/op
    ArithmeticBenchmark.subtraction     avgt   25   3.645 ± 0.035  ns/op
