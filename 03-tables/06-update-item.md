# Update Item

Update an item in the given table with the specified ID.

> **Note:** Table names are case-sensitive

## HTTP Request

```bash
PATCH /api/1/tables/[table-name]/rows/[row-id]
```

## Example Request

```bash
$ curl --data "active=1&title=Example" \
        https://database.account.directus.io/api/1/tables/projects/rows/1 \
                -u usrSTeeornngkti:
```

```javascript
client.updateItem('projects', 1, {
  active: 1,
  title: 'Example'
});
```

## Parameters

> **Note:** The parameters are based on the table's column.

## Response

> **Note:** The architecture of this response is based on your schema.

```json
{
  "id": 1,
  "active": 1,
  "title": "Example"
}
```
