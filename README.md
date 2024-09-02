# Process resource limit checker

usage: prlcheck.py [-h] [--verbose] [--threshold THRESHOLD]

```
Process resource limit checker

optional arguments:
  -h, --help            show this help message and exit
  --verbose             Be verbose (default: False)
  --threshold THRESHOLD
                        Specify threshold % (default: 80)
  --ignore IGNORE       Specify process names to ignore, csv (default: )
```

Example:

      PID |                           NAME |        Resource |           Usage |                Limit |  Use%
      ...
	15684 |                           java |       processes |           21347 |               402808 |  5.30
	15684 |                           java |       openfiles |           24827 |               100000 | 24.83
	15684 |                           java |        mapcount |           43719 |                65530 | 66.72
	15684 |                           java |    lockedmemory |               0 |                65536 |  0.00
	15684 |                           java |       stacksize |          135168 |  9223372036854775807 |  0.00
	26123 |                        wrapper |       processes |               2 |               402808 |  0.00
	26123 |                        wrapper |       openfiles |               5 |               100000 |  0.01
	26123 |                        wrapper |        mapcount |              33 |                65530 |  0.05
	26123 |                        wrapper |    lockedmemory |               0 |                65536 |  0.00
	26123 |                        wrapper |       stacksize |          176128 |  9223372036854775807 |  0.00
	 1051 |                          tuned |       processes |               5 |               402808 |  0.00
	 1051 |                          tuned |       openfiles |              13 |                 4096 |  0.32
	 1051 |                          tuned |        mapcount |             319 |                65530 |  0.49
	 1051 |                          tuned |    lockedmemory |               0 |                65536 |  0.00
	 1051 |                          tuned |       stacksize |          135168 |  9223372036854775807 |  0.00
	 1053 |                           java |       processes |             180 |               402808 |  0.04
	 1053 |                           java |       openfiles |              98 |                 4096 |  2.39
	 1053 |                           java |        mapcount |             893 |                65530 |  1.36
	 1053 |                           java |    lockedmemory |               0 |                65536 |  0.00
	 1053 |                           java |       stacksize |          135168 |  9223372036854775807 |  0.00
