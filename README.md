# 리눅스 명령어

## TOP 명령어
* 시스템 프로세스 및 메모리 사용 현황을 실시간으로 출력하는 명령어로, 작업 관리자와 같은 개념이다.
***
### 사용법
```
top
```
***

```
A20203264@cjchun-HP:~$ top
top - 10:52:12 up 169 days, 20:18,  3 users,  load average: 0.10, 0.04, 0.01
Tasks: 338 total,   1 running, 337 sleeping,   0 stopped,   0 zombie
%Cpu(s):  0.1 us,  0.1 sy,  0.0 ni, 99.8 id,  0.0 wa,  0.0 hi,  0.0 si,  0.0 st
MiB Mem :  15658.3 total,   3357.5 free,   1159.4 used,  11141.5 buff/cache
MiB Swap:   2048.0 total,   2048.0 free,      0.0 used.  14165.3 avail Mem

    PID USER      PR  NI    VIRT    RES    SHR S  %CPU  %MEM     TIME+ COMMAND
   1015 gdm       20   0 6520908 254424 118956 S   1.0   1.6 158:29.84 gnome-shell
 816111 A202032+  20   0   13432   4300   3488 R   0.7   0.0   0:00.03 top
    726 avahi     20   0    9944   5584   3560 S   0.3   0.0 498:28.22 avahi-daemon
    733 root      20   0  747728  21388  17440 S   0.3   0.1 553:53.33 NetworkManager
    860 root      20   0 2600532  45340  28956 S   0.3   0.3   1857:29 containerd
      1 root      20   0  169344  13664   8480 S   0.0   0.1   5:33.39 systemd
      2 root      20   0       0      0      0 S   0.0   0.0   0:01.61 kthreadd
      3 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 rcu_gp
      4 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 rcu_par_gp
      5 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 netns
      7 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker/0:0H-events_highpri
      9 root       0 -20       0      0      0 I   0.0   0.0   2:31.61 kworker/0:1H-kblockd
     10 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 mm_percpu_wq
     11 root      20   0       0      0      0 S   0.0   0.0   0:00.00 rcu_tasks_rude_
     12 root      20   0       0      0      0 S   0.0   0.0   0:00.00 rcu_tasks_trace
     13 root      20   0       0      0      0 S   0.0   0.0   0:08.27 ksoftirqd/0
     14 root      20   0       0      0      0 I   0.0   0.0  13:36.75 rcu_sched
     15 root      rt   0       0      0      0 S   0.0   0.0   0:57.21 migration/0
     16 root     -51   0       0      0      0 S   0.0   0.0   0:00.00 idle_inject/0
     18 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/0
     19 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/1
     20 root     -51   0       0      0      0 S   0.0   0.0   0:00.00 idle_inject/1
     21 root      rt   0       0      0      0 S   0.0   0.0   0:57.08 migration/1
     22 root      20   0       0      0      0 S   0.0   0.0   0:14.92 ksoftirqd/1
     24 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker/1:0H-events_highpri
     25 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/2
     26 root     -51   0       0      0      0 S   0.0   0.0   0:00.00 idle_inject/2
     27 root      rt   0       0      0      0 S   0.0   0.0   0:58.67 migration/2
     28 root      20   0       0      0      0 S   0.0   0.0   0:16.26 ksoftirqd/2
     30 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker/2:0H-events_highpri
     31 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/3
     32 root     -51   0       0      0      0 S   0.0   0.0   0:00.00 idle_inject/3
     33 root      rt   0       0      0      0 S   0.0   0.0   0:56.36 migration/3
     34 root      20   0       0      0      0 S   0.0   0.0   0:21.40 ksoftirqd/3
     36 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker/3:0H-events_highpri
     37 root      20   0       0      0      0 S   0.0   0.0   0:00.00 cpuhp/4
     38 root     -51   0       0      0      0 S   0.0   0.0   0:00.00 idle_inject/4
     39 root      rt   0       0      0      0 S   0.0   0.0   0:56.74 migration/4
     40 root      20   0       0      0      0 S   0.0   0.0   0:05.93 ksoftirqd/4
```

## jobs 명령어
* 작업이 중지된 상태 또는 백그라운드로 진행 중인 상태를 표시하는 명령어
***
### 사용법
```
jobs [옵션]
```

## PS 명령어
* 현재 실행 중인 프로세스를 보여주는 명령어
***
### 사용법
```
ps
```
***

```
A20203264@cjchun-HP:~$ ps
    PID TTY          TIME CMD
 816054 pts/3    00:00:00 bash
 816108 pts/3    00:00:00 ps
```

## kill 명령어
* 프로세스에 종료 시그널을 보내는 명령어
***
### 사용법
```
kill [옵션] [PID]
```
***
#### kill에서 사용 가능한 명령어 모음
```
A20203264@cjchun-HP:~$ kill -l
 1) SIGHUP       2) SIGINT       3) SIGQUIT      4) SIGILL       5) SIGTRAP
 6) SIGABRT      7) SIGBUS       8) SIGFPE       9) SIGKILL     10) SIGUSR1
11) SIGSEGV     12) SIGUSR2     13) SIGPIPE     14) SIGALRM     15) SIGTERM
16) SIGSTKFLT   17) SIGCHLD     18) SIGCONT     19) SIGSTOP     20) SIGTSTP
21) SIGTTIN     22) SIGTTOU     23) SIGURG      24) SIGXCPU     25) SIGXFSZ
26) SIGVTALRM   27) SIGPROF     28) SIGWINCH    29) SIGIO       30) SIGPWR
31) SIGSYS      34) SIGRTMIN    35) SIGRTMIN+1  36) SIGRTMIN+2  37) SIGRTMIN+3
38) SIGRTMIN+4  39) SIGRTMIN+5  40) SIGRTMIN+6  41) SIGRTMIN+7  42) SIGRTMIN+8
43) SIGRTMIN+9  44) SIGRTMIN+10 45) SIGRTMIN+11 46) SIGRTMIN+12 47) SIGRTMIN+13
48) SIGRTMIN+14 49) SIGRTMIN+15 50) SIGRTMAX-14 51) SIGRTMAX-13 52) SIGRTMAX-12
53) SIGRTMAX-11 54) SIGRTMAX-10 55) SIGRTMAX-9  56) SIGRTMAX-8  57) SIGRTMAX-7
58) SIGRTMAX-6  59) SIGRTMAX-5  60) SIGRTMAX-4  61) SIGRTMAX-3  62) SIGRTMAX-2
63) SIGRTMAX-1  64) SIGRTMAX
```
