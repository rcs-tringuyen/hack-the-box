```
[*] Service scan Directory Buster (tcp/80/http/dirbuster) ran a command which returned a non-zero exit code (134).
[-] Command: feroxbuster -u http://10.10.10.56:80/ -t 10 -w /root/.config/AutoRecon/wordlists/dirbuster.txt -x "txt,html,php,asp,aspx,jsp" -v -k -n -q -e -o "/root/results/10.10.10.56/scans/tcp80/tcp_80_http_feroxbuster_dirbuster.txt"
[-] Error Output:
thread 'tokio-runtime-worker' panicked at 'supplied instant is later than self', library/std/src/time.rs:292:48
note: run with `RUST_BACKTRACE=1` environment variable to display a backtrace
Aborted



```