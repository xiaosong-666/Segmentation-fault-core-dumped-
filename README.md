# Segmentation-fault-core-dumped-
try to run python but got the error: Segmentation fault (core dumped)
the main reason is that you have installed many things in your home version python, try to keep your ~/.local/lib/python*/site-packages clean: python -sm pip or export PYTHONNOUSERSITE=1
otherwise when you will use the libraries from home instead of conda_env even though you run your software in the build conda env, which will cause conflicts and so on...(mess/chiaos)

the way to solve this is put PYTHONNOUSERSITE=1 python xxx.py -h to aviod the library or anything from your home


https://pypi.org/project/pip-utils/ reads:

By default, pip-utils will interact with packages installed to the user site (assuming the user site is available). To disable this behavior, call pip-utils with Python’s -s option (i.e. python -sm pip_utils) or PYTHONNOUSERSITE environment variable (i.e. PYTHONNOUSERSITE=1 python -m pip_utils).


see also:

https://snarky.ca/why-you-should-use-python-m-pip/ (using module and virtualenv/conda properly can avoid most of the mess, imho)

