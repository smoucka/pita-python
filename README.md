####pita-python
===========
Original notes file, setup_notes.txt.

Streamlined process followed this time was efficient and effective. Kenneth Reitz' hitchhiker's guide [Windows setup](http://docs.python-guide.org/en/latest/starting/install/win/) is the way to go.

The guide takes you through python download, setuptools and pip install. Use pip to install virtualenv.

  pip install virtualenv

Documentation for virtualenv [here](http://www.virtualenv.org/en/latest/).

In this case I also needed [BeautifulSoup](http://www.crummy.com/software/BeautifulSoup/). A particular script required the lxml parser library. For whatever reason "pip install lxml" did not work during this attempt nor previous ones. In previous attempts when not using virtualenv (there were many as Python continued to get messed up with each ArcGIS update) I downloaded the lxml_whateverversion.exe and ran the executable. The registry recognized python installation worked fine. In earlier cases these were ArcGIS installed flavors of Python. In this attempt I had both the ArcGIS flavor and the latest version, both showed up when running the .exe but I needed to install lxml in my virtual environment specific to the project. I found my answer [here](http://stackoverflow.com/questions/3271590/can-i-install-python-windows-packages-into-virtualenvs) with more detail in the [link](http://stackoverflow.com/questions/5382801/where-can-i-download-binary-eggs-with-psycopg2-for-windows) provided in the first answer by Piotr Dobrogost.

Ran "easy_install whatever.exe" while in the virtual environment.
