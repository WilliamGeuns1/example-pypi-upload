# Overview
Following tutorial from Udacity Nanodegree\
Additional resources
https://packaging.python.org/tutorials/packaging-projects/

## `setup.cfg`
1) The name must be unique;
2) packages is the name of the folder where your packages are located;
3) zip_safe = False, the package cannot be directly ran from a zip file.

## Uploading to test.pypi
First run: `python setup.py sdist` after this you will have a tar file. Next run `pip install twine`.

Next you can upload by running the following command `twine upload --repository-url https://test.pypi.org/legacy/ dist/*`

## Uploading to pypi
(You will need two separate accounts for test.pypi and pypi)\
You will need to have the tar file and twine installed from above.
Upload to pypi `twine upload dist/*`
