## R CMD check results

0 errors | 0 warnings | 3 notes

* This is a new release.

* The second note is found only on Windows (Windows Server 2022, R-devel, 64 bit)

```
* checking for detritus in the temp directory ... NOTE
Found the following files/directories:
  'lastMiKTeXException'
```
As noted in [R-hub issue #503](https://github.com/r-hub/rhub/issues/503), this could be due to a bug/crash in MiKTeX and can likely be ignored.

* The third note is found only on Linux (Fedora Linux, R-devel, clang, gfortran)

```
* checking examples ... NOTE
Examples with CPU (user + system) or elapsed time > 5s
                    user system elapsed
crescent_kf        5.708  0.427   3.949
generate_filaments 5.431  0.056   5.487
```
The time limit on the examples was surpassed, however these functions often take variable length of time, and the random element may cause slight variation.
