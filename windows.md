# Work in progress

### Find all bound ports and filter for a specific port number.

```cmd
netstat -ano | findstr "13102"
```

### Kill a process by PID.

```cmd
taskkill -f -pid  29804
```

### Find all routes.

```cmd
route print
route print -4
route print -6
```

### Reset full windows networking stack (Administrator)

```cmd
ipconfig /release
ipconfig /flushdns
ipconfig /renew
netsh int ip reset
netsh winsock reset
```

### Shutdown / Reboot the machine, when finished.

#### Shutdown

```cmd
shutdown /s -t 0
```

#### Reboot

```cmd
shutdown /r -t 0
```

#### Reboot into UEFI/BIOS/Setup

```cmd
shutdown /r /fw /f /t 0
```

#### Reboot into windows recovery environment

```cmd
shutdown /r /o /f /t 0
```

### Pathping / Ping

#### No timeout, keep pinging

```cmd
ping -t 8.8.8.8
```

#### Force resolve ipv4

```cmd
ping -4 -t 8.8.8.8
```

#### Force resolve ipv6

```cmd
ping -6 -t 8.8.8.8
```

#### ipv4, no timeout, TTL of 1 second
```cmd
ping -4 -t -w 1 198.18.0.4
```

### Pathping

...
