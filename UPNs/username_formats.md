# Statistics on Username Formats


### Top Username Formats - By Total User Population

```
[graph of all formats sorted by popularity - total users ]
```

---

### Top Username Formats - By Number of Domains

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
