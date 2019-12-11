Requirements: This tool requires that python3 be installed on your system with
the requests, json, time, sys, os, base64, datetime, hashlib, hmac, urllib,
argparse, logging, and configparser python libs available. You will also need
network access to both your Absolute and Snipe-IT environments. You will also
need a Absolute token and secret key from an account that access to the API for
computer assets (a guest or admin account). You will need a snipe api key for a
user that has edit/create permissions for assets and models.

Overview: What does it do? This tool will sync assets between a Absolute
instance and a snipe-it instance. The tool searches for assets based of of the
serial number, and not the existing asset tag. In future versions the tool will
be able to create

Installation: Copy the files to your system (recommend installing to
/opt/absolute2snipe/* ). Make sure you meet all the system requirement. Edit
the settings.conf to match your current environment. The script will look for
a valid settings.conf in /opt/absolute2snipe/settings.conf,
/etc/absolute2snipe/settings.conf, or in the current folder (in that order):
so either copy the file to one of those locations, or be sure that the user 
running the program is in the same folder as the settings.conf.

Configuration: All of the settings that are listed in the settings.conf are
required except for the api-mapping section. It's recommended that you install
these files to /opt/Absolute2snipe/ and run them from there. You will need
valid subsets of from Absolute's api to associate fields into snipe. More
information can be found in the ./Absolute2snipe file about associations and
valid subsets. For more ingormation about API credential generation, please see
the project documentation:
https://www.absolute.com/api - https://snipe-it.readme.io/reference
