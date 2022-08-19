# Nello-Subdomain-Finder


Basic python script that looks into a subdomain text list and compares it with a given link



![imagen](https://user-images.githubusercontent.com/80414186/185537564-1007df05-a247-47f9-867c-073fac8b958a.png)

🔧 Installation

# Clone the repository
$ git clone https://github.com/valentinello/Nello-Subdomain-Finder

# Go into the Subd folder
$ cd Subd

# Install the requirements
$ python3 -m pip install -r requirements.txt

🕹 Usage

$ python3 Subd.py -h
usage: Subd.py [-h] -d DOMAIN -l FILE [-s] [-sv LOGS_FILE]

Script to scan subdomains of a domain

options:
  -h, --help     show this help message and exit
  -d DOMAIN      Domain
  -l FILE        List of subdomains
  -s             Skip subdomains with the same ip
  -sv LOGS_FILE  Save the results to a file
  

Scan a domain using the subdomains list in the "default.txt" file

python3 Subd.py -d facebook.com -l default.txt

Scan a domain using the subdomains list in the file "default.txt" and skip the subdomains with the same ips

python3 Subd.py -d facebook.com -l default.txt -s

Scan a domain using the list of subdomains in the file "default.txt" and save the results in the file "logs.txt"

python3 Subd.py -d facebook.com -l default.txt -sv logs.txt
