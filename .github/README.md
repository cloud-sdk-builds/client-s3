# 🟡 Community Browser CDN Build – JavaScript SDK Client Package

This repository provides a **community-maintained, browser-ready distribution** of the npm module
[`@aws-sdk/client-s3`](https://www.npmjs.com/package/@aws-sdk/client-s3/v/3.826.0).

Each package is **automatically built and published to a CDN**, allowing developers to use the SDK client **directly in browsers** with **zero bundling or build steps**.

> ⚡ No build process required — import directly from a CDN and start using it immediately.

---

## ⚠️ Trademark & Affiliation Notice

This project is a **community-operated distribution** and is **not affiliated with, endorsed by, or sponsored by**
Amazon Web Services or the official SDK maintainers.

“AWS”, “Amazon Web Services”, and related marks are trademarks of their respective owners.
All original SDK source code remains licensed under its respective upstream license.

---

## 📦 Usage

You can use this package directly in the browser via **jsDelivr** using an **import map**.

### 📌 This Version

CDN URL

```text
https://cdn.jsdelivr.net/gh/cloud-sdk-builds/client-s3@3.826.0/index.min.mjs
```

SRI SHA Hash
```text
sha384-Q3nRoL3y4vCnA7hTvEbnKRZ1FJqBmWxGsX4FbNdWnjaSMsP5G8OTCUaVzSoWKHw+
```

### 📌 Latest Version

```text
https://cdn.jsdelivr.net/gh/cloud-sdk-builds/client-s3/index.min.mjs
```

---

## 🧩 Example (Browser Usage)

```html
<!DOCTYPE html>
<html>
  <head>
    <script type="importmap">
      {
        "imports": {
          "@aws-sdk/client-s3": "https://cdn.jsdelivr.net/gh/cloud-sdk-builds/client-s3@3.826.0/index.min.mjs"
        },
        "integrity": {
          "https://cdn.jsdelivr.net/gh/cloud-sdk-builds/client-s3@3.826.0/index.min.mjs": "sha384-Q3nRoL3y4vCnA7hTvEbnKRZ1FJqBmWxGsX4FbNdWnjaSMsP5G8OTCUaVzSoWKHw+"
        }
      }
    </script>
  </head>
  <body>
    <script type="module">
      import { } from "@aws-sdk/client-s3";
      // Refer to official SDK documentation for usage examples
    </script>
  </body>
</html>
```

---

## 📚 Available Packages

Any official `@aws-sdk/*` module published on npm can be built for browser CDN usage.

If a package you need is not yet available, please open an issue in:

```
https://github.com/cloud-sdk-builds/.github/issues
```

---

## 🔧 Repository Contents

* **`index.min.mjs`**
  A single, production-ready, minified ES module bundle intended for direct browser usage.

* **`.github/`**
  Internal automation files (not required for end users).

* **`LICENSE`**
  Licensing terms for this distribution.

---

## 🌐 CDN URL Format

### Latest Version

```
https://cdn.jsdelivr.net/gh/cloud-sdk-builds/{aws_service_name}/index.min.mjs
```

### Specific Version

```
https://cdn.jsdelivr.net/gh/cloud-sdk-builds/{aws_service_name}@{aws_version}/index.min.mjs
```

Replace

- {aws_service_name} with client-s3 or client-dynamodb or client-lambda etc.,
- {aws_version} with aws service specific version

---

## 🔒 Security Notice

When using CDN builds in production environments:

* Always pin to a specific version (`@3.826.0`)
* Avoid using `latest` in production to prevent unexpected breaking changes

---

## 🤝 Contributing & Requests

To request support for additional browser-ready SDK packages, please open an issue:

```
https://github.com/cloud-sdk-builds/.github/issues
```

---

## 📜 License

This distribution follows the license terms included in the repository:

```
https://github.com/cloud-sdk-builds/client-s3/blob/refs/tags/3.826.0/LICENSE
```

---

If you want, I can next give you a **legally safest naming pattern** for all repositories (very important for trademark safety, especially avoiding “aws-sdk” in repo names while still keeping discoverability).
