## vercel.json

Vercel json config for express backend

```bash
  {
    "version": 2,
    "builds": [
        {
            "src": "index.js",
            "use": "@vercel/node",
            "config": {
                "includeFiles": [
                    "dist/**"
                ]
            }
        }
    ],
    "routes": [
        {
            "src": "/(.*)",
            "dest": "index.js"
        }
    ]
}
```

Vercel json config to support React Router in frontend

```bash
  {
    "rewrites": [
      {
        "source": "/(.*)",
        "destination": "/"
      }
    ]
  }
```
