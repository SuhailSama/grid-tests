# A few SWIG examples adapted from the official documentation:
# http://swig.org/Doc3.0/Introduction.html
# These are just a few of the languages SWIG can support; see "swig --help"
# for a list.

queue = bme.q

all: swig-python

swig-tcl:
	qsub -q "$(queue)" swig-tcl.sh

swig-python:
	qsub -q "$(queue)" swig-python.sh

clean:
	rm -f swig-{python,tcl}.{o,e}*
	rm -f example_python_wrap.*
	rm -f example_wrap.*
	rm -f *.{o,so}
	rm -f example_python.py
	rm -f *.pyc
