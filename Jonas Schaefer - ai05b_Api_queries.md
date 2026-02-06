# API Query Building Assignment
---

## USGS Earthquake Queries

### Query 1: [eathquAKES IN THE LAST DAY WITH A 4.5 MAGNITUDE OR HIGHER]
**URL:**
```
https://earthquake.usgs.gov/fdsnws/event/1/query?format=geojson&starttime=2024-01-01&minmagnitude=4.5

```

**Parameters used:**
- `format=geojson`: [it tells USGS to return data to JSON format]
- `starttime=2024-01-01`: [only earth quakes that happened after this date.]
- `paraminmagnitude=4.5`: [only shows earthquakes witha magnitude of 4.5 or higher]

**Result:** [Brief description of what JSON data you got back - how many earthquakes? what magnitude range? etc. returned 200 earth quakes mostly ranging from 4.5-6.2 magnitude ]

---

### Query 2: []
**URL:**
```
https://earthquake.usgs.gov/fdsnws/event/1/query?format=geojson&minlatitude=32&maxlatitude=42&minlongitude=-125&maxlongitude=-114&starttime=2024-02-01

```

**Parameters used:**
- `format=geojson`: [JSON output]
- `minlongitude/maxlongitude`: [bounding box for cali]
- `starttime=2024-02-01`: [Earthquakes from the last 7 days only]

**Result:** [returned around 80 earth quakes that were small]

---

### Query 3: [largest earth quake in last 30 days]
**URL:**
```
https://earthquake.usgs.gov/fdsnws/event/1/query?format=geojson&orderby=magnitude&limit=1&starttime=2024-01-01
```

**Parameters used:**
- `format`: [JSON output]
- `parameter2=magnitude`: [sorts by biggest magnitude first]
- `atarttime 2024-01-01`: [last 30 days]

**Result:** [Returned 1 earthquake magnitude around 8.8 with location included in the JSON.]

---

## Open Library Queries


### Query 4: [Search for books with the keyword “Python programming”]
**URL:**
```
[https://openlibrary.org/search.json?q=python+programming
]
```

**Parameters used:**
- `paq=python+programming`: [search for books with that phrase]

**Result:** [Reurned hundreds of books like learning python and python crash course ]


### Query 5: [Search for books by author Stephen King]
**URL:**
```
https://openlibrary.org/search.json?author=stephen+king
```

**Parameters used:**
- author=stephen+king - filters results to that author
- 

**Result:** [it returned many books including IT, The Shining, and Carrie]

### Query 6: [search for books published in 2020]
**URL:**
```
https://openlibrary.org/search.json?publish_year=2020
```

**Parameters used:**
- publish_year=2020`: [ only books from that year]

**Result:** returned me thousands of books with a wide range of authors and genres