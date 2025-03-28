---
title: HSET
description: HSET sets field value in the string-string map stored at key
---

<!-- This file is automatically generated. Any modifications made directly to this file
  may be overwritten. For more details on how this file is generated and how to use
  the related commands, refer to the documentation available in the `internal/cmd/cmd_*.go` files.
-->

#### Syntax

```
HSET key field value [field value ...]
```


HSET sets the field and value for the key in the string-string map.

Returns "OK" if the field value was set or updated in the map. Returns (nil) if the
field value was not set or updated.
	

#### Examples

```

localhost:7379> HSET k1 f1 v1
OK 1
localhost:7379> HSET k1 f1 v1 f2 v2 f3 v3
OK 2
localhost:7379> HGET k1 f1
OK v1
localhost:7379> HGET k2 f1
OK (nil)
	
```
