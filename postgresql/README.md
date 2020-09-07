# postgresql

# NAME

postgresql

# SYNOPSIS

kubectl apply --recursive -f postgresql

# Description

Postgresql non-HA instance

# Configuration

```
kpt cfg list-setters .
kpt cfg set . $PARAM $VALUE --description $REASON
```

Afterwards, initialise the database with `instance/config/init.sql_`.

# SEE ALSO
