# Delete Column

> **Note:** Table names are case-sensitive

<span class="request">`DELETE` **/api/1.1/tables/[table-name]/columns/[column-name]**</span>
<span class="description">Deletes a column to the given table.</span>
<span class="arguments">Name</span> | Value | Description
**table_name** _String_             | <span class="required">Required</span>    | Table name
**column_name** _String_            | <span class="required">Required</span>    | Column name

```bash
$ curl -X DELETE  https://instance--key.directus.io/api/1.1/tables/projects/columns/intro \
        -u [user-token]:
```

```php
$client->deleteColumn('projects', 'intro');
```

## Response

<span class="attributes">Attribute</span> | Description
--------|-----|------------
**success** _Boolean_ | Whether or not the bookmark was deleted.
**error** _Error Object_ | This object contains error information (if any). <a class="object">**Error Object**: View Nested Attributes</a>

#### Successful

```json
{
  "meta": {
    "table": "projects",
    "column": "intro"
  },
  "success": true
}
```

#### Unsuccessful

```
{
  "meta": {
    "table": "projects",
    "column": "intro"
  },
  "success": false,
  "error": {
    "message": "column `intro` does not exists in table: `projects`"
  }
}
```