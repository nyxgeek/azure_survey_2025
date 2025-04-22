# Statistics on Username Formats


### Top Username Formats - By Number of Tenants

```
+-----------------------+---------------+
| userlist              | total_tenants |
+-----------------------+---------------+
| john.50               |         78209 |
| jsmith_15x5.75        |         67828 |
| john.smith_10x50.500  |         20681 |
| jjsmith_10x5x10.500   |         10466 |
| johns_5x15.75         |          8896 |
| smith.50              |          7752 |
| sjohn_15x5.75         |          5348 |
| j.smith_15x5.75       |          2918 |
| smithj_5x15.75        |          2847 |
| johnsmith_10x50.500   |          1904 |
| jjs_4x5x5.100         |          1885 |
| smithjj_10x5x10.500   |          1208 |
| john.j.smith.1000     |          1108 |
| john.s_5x15.75        |          1043 |
| smith.john_50x10.500  |           546 |
| johnjs_5x10x10.500    |           418 |
| s.john_15x5.75        |           382 |
| john.j.smith.250      |           223 |
| smith.j_5x15.75       |           164 |
| smithjohn_50x10.500   |           129 |
| john.james.smith.3600 |            31 |
| smithjoh_10x50.186    |            23 |
| johnsmit_10x50.178    |             1 |
+-----------------------+---------------+
```

---


---

### Top Username Formats - By Total User Population

```
[graph of all formats sorted by popularity - total users ]
```

---

#### John.Smith Format

These were extracted from approximately 70 million UPNs by first grepping out ```'^[a-z]\{2,\}\.[a-z]\{2,\}@'``` to get 'name.name' formatted UPNs. Then john.smith UPNs were filtered using grep -f to match a file of first names in regex format (e.g., ```'^john\.'```).
Since some names are also last names, there will be some false positives from this method, but this should be fairly close.

```
John Smith (any found): 84514
John Smith ( >3 found): 51067
John Smith ( >5 found): 43575
```

#### Smith.John Format

These were extracted from approximately 70 million UPNs by first grepping out ```'^[a-z]\{2,\}\.[a-z]\{2,\}@'``` to get 'name.name' formatted UPNs. Then smith.john UPNs were filtered using grep -f to match a file of first names in regex format (e.g., ```'^smith\.'```).
Since some names are also last names, there will be some false positives from this method, but this should be fairly close.

```
```
