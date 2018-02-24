# CrawlBox
Easy way to brute-force web directory.<br>

<a href="https://asciinema.org/a/keUhurPa1dzABWvVxBwhBu4Yp"><img src="https://asciinema.org/a/keUhurPa1dzABWvVxBwhBu4Yp.png" width="836"/></a>

<br>

# Operating Systems Tested
MacOSX

# Usage
<pre>python crawlbox.py [-h] [-v] [-w WORDLIST] url</pre>
positional arguments:

  <pre>url            specific target url, like domain.com</pre>
optional arguments:

<pre>  -h, --help     show this help message and exit
  -v, --version  show program's version number and exit
  -w WORDLIST    specific path to wordlist file
  -d DELAY       add delay between requests</pre>

# Example
web site scan with internal wordlist

<pre>python crawlbox.py www.domain.com</pre>
web site scan with external wordlist

<pre>python crawlbox.py www.domain.com -w wordlist.txt</pre>

# Install
(as root)
  <pre>
  git clone https://github.com/chamli/crawlbox.git
  cd crawlbox/
  pip install -r requirements.txt
  python crawlbox.py -h</pre>
note: tested with python 2.7.6