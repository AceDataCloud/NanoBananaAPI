# Nano Banana Image Generation API

Nano Banana AI image generation service offers functions such as image generation and image editing.

API home page: [Ace Data Cloud - Nano Banana Image Generation](https://platform.acedata.cloud/services/44fa6ed2-1ad1-4c7e-a8bd-30002728c0d1)

## Get Started


This document introduces the integration and usage of the Nano Banana Images API. This interface supports two capabilities: **image generation (generate)** and **image editing (edit)**.

### Application Process

Before use, please enter the [Nano Banana Images API](https://platform.acedata.cloud/documents/23985a11-d713-41d1-ad84-24b021805b3d) on the Ace Data Cloud platform and click Acquire to apply for activation. The first application usually has free credits available. Once activated, you can obtain a Bearer Token for API calls on the platform.

### Interface Overview

- **Base URL**: `https://api.acedata.cloud`
- **Endpoint**: `POST /nano-banana/images`
- **Authentication Method**: Include `authorization: Bearer {token}` in the HTTP Header
- **Request Headers**:
  - `accept: application/json`
  - `content-type: application/json`
- **Actions**:
  - `generate`: Generate images based on text prompts
  - `edit`: Edit based on given images
- **Asynchronous Callback**: Optional, receive task completion notifications and results via `callback_url`

### Quick Start: Generate Image (`action=generate`)

**Minimum Required Parameters**: `action`, `prompt`
When you only want to generate an image based on a prompt, set `action` to `generate` and provide a clear `prompt`.

#### Request Example (cURL)

```bash
curl -X POST 'https://api.acedata.cloud/nano-banana/images' \
  -H 'authorization: Bearer {token}' \
  -H 'accept: application/json' \
  -H 'content-type: application/json' \
  -d '{
    "action": "generate",
    "prompt": "A photorealistic close-up portrait of an elderly Japanese ceramicist with deep, sun-etched wrinkles and a warm, knowing smile. He is carefully inspecting a freshly glazed tea bowl. The setting is his rustic, sun-drenched workshop. The scene is illuminated by soft, golden hour light streaming through a window, highlighting the fine texture of the clay. Captured with an 85mm portrait lens, resulting in a soft, blurred background (bokeh). The overall mood is serene and masterful. Vertical portrait orientation."
  }'
```

#### Request Example (Python)

```python
import requests

url = "https://api.acedata.cloud/nano-banana/images"
headers = {
    "authorization": "Bearer {token}",
    "accept": "application/json",
    "content-type": "application/json",
}
payload = {
    "action": "generate",
    "prompt": (
        "A photorealistic close-up portrait of an elderly Japanese ceramicist "
        "with deep, sun-etched wrinkles and a warm, knowing smile. He is carefully "
        "inspecting a freshly glazed tea bowl. The setting is his rustic, sun-drenched "
        "workshop. The scene is illuminated by soft, golden hour light streaming through "
        "a window, highlighting the fine texture of the clay. Captured with an 85mm "
        "portrait lens, resulting in a soft, blurred background (bokeh). The overall mood "
        "is serene and masterful. Vertical portrait orientation."
    ),
}
resp = requests.post(url, json=payload, headers=headers)
print(resp.json())
```


## More

For more info, please check below APIs and integration documents.

| API | Path | Integration Guidance |
| ---- | ---- | ------------ |
| [Nano Banana Images API](http://platform.acedata.cloud/documents/23985a11-d713-41d1-ad84-24b021805b3d) | `/nano-banana/images` | [Nano Banana Images API Integration Guide](http://platform.acedata.cloud/documents/2fb479f8-63ec-424c-a93e-b12cd4250f9e) |
| [$t(document_title_nanobanana_tasks_api)](http://platform.acedata.cloud/documents/617810f5-081f-4866-a21a-cededecb0ccd) | `/nano-banana/tasks` | [Nano Banana Tasks API Integration Guide](http://platform.acedata.cloud/documents/e01ef840-3158-4eec-a6e7-337dada8d155) |

Base URL: [https://api.acedata.cloud](https://api.acedata.cloud)

## Support

If you meet any issue, check our from [support info](https://platform.acedata.cloud/support).