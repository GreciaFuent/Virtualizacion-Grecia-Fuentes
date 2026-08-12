# Assessment 01 (Group 4)

### Mayda Daniela Matul Alvarado - 1535523
### Grecia Fernanda Fuentes Hernández - 1537723

## ZeroTier Configuration

A new ZeroTier network was created with the name `assessment-01`.

**Network ID: 363c67c55a5a2b2f**


![ZeroTier Network](utils/img1.png)

The IPv4 subnet configured for the network is:

```text
10.241.9.0/24 and 10.242.9.0/24
```
---

![IPv4 subnet configured ](utils/img4.png)

## Client Configuration

## Hostname Configuration


```text
cliente-01
```

![Client 01 Hostname](utils/img2.png)


```text
cliente-02 
```

![Client 01 Hostname](utils/img3.png)


```text
cliente-03
```

![Client 01 Hostname](utils/img32.png)

---

```text
router
```

![Client 01 Hostname](utils/img12.png)

---

## Static IP Configuration

A static ZeroTier IPv4 address was manually assigned.

![ZeroTier IPv4 ](utils/img9.png)


```text
router (10.241.9.1 / 10.242.9.1)
```

![Client 01 Static IP](utils/img14.png)



```text
cliente-01 (10.242.9.2)
```

![Client 01 Network Verification](utils/img11.png)

```text
cliente-02 (10.242.9.3)
```


![Client 01 Network Verification](utils/img10.png)


```text
cliente-03 (10.241.9.4)
```

![Client 01 Static IP](utils/img15.png)


## Managed Route

![ZeroTier Managed Route ](utils/img25.png)


## IP forwarding

![status 1](utils/img19.png)

![status 1](utils/img20.png)

## ICMP connectivity test (Ping)


```text
cliente-01 to cliente-02 and cliente-03 
```

![Ping Client 01](utils/img18.png)
![Ping Client 01](utils/img23.png)

```text
cliente-02 to cliente-01 and cliente-03 
```

![Ping Client 02](utils/img17.png)
![Ping Client 02](utils/img24.png)


```text
cliente-03 to client-01 and to cliente-02
```

![Ping Client 03](utils/img21.png)

![Ping Client 03](utils/img22.png)


## Network path  (Tracepath)

```text
cliente-01 to cliente-02 and cliente-03 
```

![Tracepath Client 01](utils/img31.png)
![Tracepath Client 01](utils/img28.png)

```text
cliente-02 to cliente-01 and cliente-03 
```

![Tracepath Client 02](utils/img30.png)
![Tracepath Client 02](utils/img29.png)


```text
cliente-03 to client-01 and to cliente-02
```

![Tracepath Client 03](utils/img26.png)
![Tracepath Client 03](utils/img27.png)