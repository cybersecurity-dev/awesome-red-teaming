# Reconnaissance

## [NMAP](https://www.kali.org/tools/nmap/)

```terminal
nmap -sS -sV -T4 -p 1-1000 <remote-ip>
```

## [FEROXBUSTER](https://www.kali.org/tools/feroxbuster/)
```terminal
feroxbuster -u http://<remote-ip>/blog/
```

```terminal
feroxbuster -u http://<remote-ip>/blog/ -x php
```

```terminal
feroxbuster -u http://<remote-ip>/blog/ -s 200 -s 301 -x php -q
```

## [EXPLOITDB](https://www.kali.org/tools/exploitdb/)

```terminal
searchsploit nibbleblog
```

## [METASPLOIT](https://www.kali.org/tools/metasploit-framework/)

```terminal
msfconsole -q
```

```terminal
msf6> search nibble
```

## [REVERSE SHELL](https://www.imperva.com/learn/application-security/reverse-shell/)

Method: `Python pty module`
  ```terminal
  python -c 'import pty; pty.spawn("/bin/bash")'
  ```
