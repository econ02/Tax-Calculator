## Cross-Checking Results from Tax-Calculator

The contents of this directory are for use by the core development
team only.

The purpose of the cross-checking is to test that Tax-Calculator
produces essentially the same results when accessed in two different
ways: (1) via the [TaxBrain file-upload web
page](http://www.ospc.org/taxbrain/file/) and (2) via the
Tax-Calculator command-line interface (CLI) `tc` running on a local
computer.  The CLI is part of the the taxcalc conda package, which
is installed using this command `conda install -c ospc taxcalc`.

The contents of this directory include JSON reform and assumption
files used in the cross-checking.  The local-computer results are
generated by the `cli-results` bash script in this directory.

The TaxBrain results are located at `http://www.ospc.org/taxbrain/RUN/`
where `RUN` is the number of the TaxBrain run.

### Results for version 0.8.2 are as follows:

#### Reform `r1.json` with assumptions `a0.json`
```
              Tax-Calculator CLI   TaxBrain RUN 12224
2022 INCOME TAX ($B)     1817.36   1817.4  <---- same ----
2022 PAYROLL TAX ($B)    1474.76   1474.8  <---- same ----
```

#### Reform `r1.json` with assumptions `a1.json`
```
              Tax-Calculator CLI   TaxBrain RUN 12225
2022 INCOME TAX ($B)     1770.35   1770.4  <---- same ----
2022 PAYROLL TAX ($B)    1447.90   1447.9  <---- same ----
```

#### Reform `r1.json` with assumptions `a2.json`
```
              Tax-Calculator CLI   TaxBrain RUN 12226
2022 INCOME TAX ($B)     1791.99   1792.0  <---- same ----
2022 PAYROLL TAX ($B)    1461.56   1461.6  <---- same ----
```
