# Segmentation-fault-core-dumped-
try to run python but got the error: Segmentation fault (core dumped)


https://pypi.org/project/pip-utils/ reads:

By default, pip-utils will interact with packages installed to the user site (assuming the user site is available). To disable this behavior, call pip-utils with Python’s -s option (i.e. python -sm pip_utils) or PYTHONNOUSERSITE environment variable (i.e. PYTHONNOUSERSITE=1 python -m pip_utils).


see also:

https://snarky.ca/why-you-should-use-python-m-pip/ (using module and virtualenv/conda properly can avoid most of the mess, imho)

