## P11
any adress betwwen 128.119.40.128 128.119.40.191

128.119.40.64/28  128.119.40.80/28  128.119.40.96/28  128.119.40.112/28

## P16

a)Home addresses：192.168.1.1，192.168.1.2，192.168.1.3，router interface:192.168.1.4

b)

WAN:24.34.112.235,4000  LAN:192.168.1.1,3345

WAN:24.34.112.235,4001  LAN:192.168.1.1,3346

WAN:24.34.112.235,4002  LAN:192.168.1.2,3445

WAN:24.34.112.235,4003  LAN:192.168.1.2,3446

WAN:24.34.112.235,4004  LAN:192.168.1.3,3545

WAN:24.34.112.235,4005  LAN:192.168.1.3,3546

## P19

|                          Match                            |   Action   |
| --------------------------------------------------------- | ---------- |
| Ingress Port: 1;  IP Src: 10.3.\*.\*;  IP Dst: 10.1.\*.\* | Forward(2) |
| Ingress Port: 2;  IP Src: 10.1.\*.\*;  IP Dst: 10.3.\*.\* | Forward(1) |
| Ingress Port: 1;  IP Dst: 10.2.0.3                        | Forward(3) |
| Ingress Port: 2;  IP Dst: 10.2.0.3                        | Forward(3) |
| Ingress Port: 1;  IP Dst: 10.2.0.4                        | Forward(4) |
| Ingress Port: 2;  IP Dst: 10.2.0.4                        | Forward(4) |
| Ingress Port: 3;  IP Dst: 10.2.0.4                        | Forward(4) |
| Ingress Port: 4;  IP Dst: 10.2.0.3                        | Forward(3) |
