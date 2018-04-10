# Select Statement
Select statement or `SELECT` is the statement or term used to get the data you want from the server. The following examples is the way

## Selecting all available columns
**CLIENT REQUEST**
```json
{
    "database": "[DB database url]",
    "private_key": "[PRIVATE_KEY]",
    "SELECT": "[table_name]"
}
```

**SERVER RESPONSE**
```json
{
    "[table_name]": [
        {
            "[col_name1]": "[value 1]",
            "[col_name2]": "[value 1]",
            "[col_nameN]": "[value 1]"
        },{
            "[col_name1]": "[value 2]",
            "[col_name2]": "[value 2]",
            "[col_nameN]": "[value 2]"
        }{
            "[col_name1]": "[value N]",
            "[col_name2]": "[value N]",
            "[col_nameN]": "[value N]"
        }
    ]
}
```

## Selecting a specific columns
**CLIENT REQUEST**
```json
{
    "database": "[DB database url]",
    "private_key": "[PRIVATE_KEY]",
    "SELECT": {
        "[table_name]": [
            "[col_name_example1]",
            "[col_name_in_table]",
            "[col_name_every]"
        ]
    }
}
```

**SERVER RESPONSE**
```json
{
    "[table_name]": [
        {
            "[col_name_example1]": "[value 1]",
            "[col_name_in_table]": "[value 1]",
            "[col_name_every]": "[value 1]"
        },
        {
            "[col_name_example1]": "[value 2]",
            "[col_name_in_table]": "[value 2]",
            "[col_name_every]": "[value 2]"
        },
        {
            "[col_name_example1]": "[value N]",
            "[col_name_in_table]": "[value N]",
            "[col_name_every]": "[value N]"
        }
    ]
}
```