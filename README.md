# RSON
List of examples and idea repository. This will serves as the feature management community repository page.

## Basics
### Select Method
Client Request to the Server.
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
Server Response to the Client Request
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

### Insert Method
TODO
### Update Method
TODO
### Delete Method
TODO