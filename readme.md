A repo for my extragalactic project/assignment

data were retrived from [SDSS DR17](https://skyserver.sdss.org/dr17/SearchTools/sql) with the following queries:
> sdss1.csv
```
SELECT p.g, p.i, p.r, s.z 
FROM PhotoObj AS p 
JOIN SpecObj AS s ON s.bestobjid = p.objid 
WHERE s.z BETWEEN 0.09 AND 0.1 AND s.class = 'GALAXY'
```

> sdss2.csv
```
SELECT p.g, p.i, p.r, s.z 
FROM PhotoObj AS p 
JOIN SpecObj AS s ON s.bestobjid = p.objid 
WHERE s.z BETWEEN 1.00 AND 1.01 AND s.class = 'GALAXY'
```