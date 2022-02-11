# Custom patch notes

* uses an older version of ring, which is natively bound so multiple versions cannot exist
* octorust uses a new ring version, because it uses version 7 of jsonwebtoken (instead of older, 6)

## Updating octorust

* grab new sources
* downgrade jsonwebtoken to 6
* disable JWT calculation in auth, return Err() always
