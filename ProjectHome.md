This is a program which allow to graph GNU make projects. This program is used to generate a DOT file that represent the dependencies between GNU makefile's targets. It uses as input a makefile database.

The typical usage is:
```
  make -npr > Makefile.complete
  python ~jpbarrette/Projects/MakeGrapher/make_grapher.py -T Makefile.complete -s "../tmp/build" -o test.dot
  dot -Tps test.dot > test.ps; ps2pdf test.ps; acroread test.pdf
```
Currently, the only way to get the code is from the repository located here: http://bitbucket.org/jpbarrette/makegrapher/overview/