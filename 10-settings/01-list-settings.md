# Get Settings

Get all Directus settings.

## HTTP Request

```bash
GET /api/1/settings
```

## Example Request

```bash
$ curl https://database.account.directus.io/api/1/settings
```

```javascript
client.getSettings();
```

## Response

```json
{
  "global": {
    "cms_user_auto_sign_out": "60",
    "project_name": "Directus Demo",
    "project_url": "http:\/\/examplesite.dev\/",
    "cms_color": "#7ac943",
    "rows_per_page": "200",
    "cms_thumbnail_url": ""
  },
  "files": {
    "allowed_thumbnails": "",
    "thumbnail_quality": "100",
    "thumbnail_size": "200",
    "file_naming": "file_id",
    "thumbnail_crop_enabled": "1",
    "youtube_api_key": ""
  }
}
```
