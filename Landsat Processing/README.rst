To get started with this project, ensure that you have the latest version of Python 3.9 installed.
    - https://www.python.org/downloads/release/python-3912/
You will also need to have Poetry, a Python package and dependency manager, installed.
    - https://python-poetry.org/docs/#windows-powershell-install-instructions

To deploy the landsat-processing project, unzip the project package.  In command prompt, navigate to the root folder of this project and run the command "poetry Install".
    - https://python-poetry.org/docs/basic-usage/#installing-dependencies

A virtual environment will be installed that is isolated from your main python installation.

Installing the python libraries GDAL and Cartopy (GDAL has a dependency on Cartopy) will not work through the typical "pip install" command.  They will need to be manually installed from the wheel file.
I've downloaded the wheel files and placed them in the resources/wheels folder. The files have been referenced in the TOML file and will be installed when you run the "poetry install" command.

pip install <path to wheel file> ex: pip install "C:\ai-la\landsat-processing\resources\wheels\Cartopy-0.20.2-cp39-cp39-win_amd64.whl"
    - Note you must have the virtual env that resides within this poetry project active.

To start up jupyter notebook, run the following command: python -m notebook
    - Note you must have the virtual env that resides within this poetry project active.