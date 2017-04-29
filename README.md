# README #

This is a simple Python script to remove the last revision of every file encrypted by Spora Ransomware and rename them to what they were before infection.

This script will revert all files on your Google Drive back one revision if they were altered after a certain date. Use at your own risk.

## Setup

Install Python 3.x or greater and pip (package manager).

- Install Python and Pip on MacOS using Homebrew (http://docs.brew.sh/Homebrew-and-Python.html);
- Install Python and Pip on Windows (https://github.com/BurntSushi/nfldb/wiki/Python-&-pip-Windows-installation);
- Install Python and Pip on Linux (just the package manager of your favorite Distro. For ubuntu `sudo apt-get install python-pip`);

Import the required python libs :

	pip install --upgrade google-api-python-client requests httplib2

Turn on the Drive API and generate a OAuth client ID (step 1 will guid through enabling the API Key and downloading client_secret.json) : https://developers.google.com/drive/v3/web/quickstart/python

## Run the Script

Execute the following commands in a terminal

	python cleanup.py
