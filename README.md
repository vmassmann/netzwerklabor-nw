# netzwerklabor-nw
Netzwerklabore der BBS Brinkstraße Osnabrück - NW Test Plants

Hier findet man die **Router-/ Switch-Grundkonfiguration** zur *Wiederherstellung* im Netzwerklabor.



# NW Test Plant - allgemein

* 4x Testbeds mit 
** 3x Router
** 3x Switch
** 1x Steckdosenleiste

## Grundzustand der Netzwerkkomponenten

Verbindet man sich über eine serielle Konsolenverbindung mit einer Netzwerkkomponente,
dann meldet sich diese mit einem spezifischen Banner.
Für den Fall, dass eine andere Konfiguration per *copy run startup* oder *wr mem* gespeichert wurde,
können hier die Grundkonfigurationen zur Wiederherstellung des Labor-Grundzustands bezogen werden.

## Wiederherstellung
des *Labor-Grundzustands* einer Netzwerkkomponente

```
Stellen Sie sicher, dass Sie sich auf der "richtigen" Komponente befinden!
```

### Router

```
erase startup
reload
```

! spezifische Grundkonfiguration von hier laden

```
copy run startup
```

### Switch

```
erase startup
delete flash:vlan.dat
reload
```

! spezifische Grundkonfiguration von hier laden

```
copy run startup
```

### NW Test Plant R006 v1
#### NW Test Plant R006 v1 - Test Plant 1
* Router ISR 2901-SEC/K9
* Switch Catalyst 2960+24TC-L


### NW Test Plant R112 v1
* nutzbar in den IT Laboren R111 und R113
  
#### NW Test Plant R112 v1 - Test Plant 1
* Router ISR 4321-SEC/K9
* Switch Catalyst 2960+24TC-L
  
#### NW Test Plant R112 v1 - Test Plant 2
* Router ISR 4331-SEC/K9
* Switch Catalyst 2960+24TC-L
  
#### NW Test Plant R112 v1 - Test Plant 3
* Router ISR 2811-SEC/K9
* Switch Catalyst 2960+24TC-L


# IS Infrastruktur
* tbd.

