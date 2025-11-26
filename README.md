# URL Splitter

URL Splitter is a lightweight web app that allows you to display multiple websites **side by side in a split-screen layout** using iframes. The number of columns adjusts automatically based on the number of URLs provided.

## GET Parameters

The page supports the following URL parameters:

* `urls` (required):
  A comma-separated list of URLs to display in iframes.
  Each URL will be shown in a separate column.

  ```
  ?urls=https://google.com,https://wikipedia.org
  ```

* `title` (optional):
  Sets the page title.

  ```
  &title=Comparator
  ```

## Examples

Display two sites side by side:

```
https://your_username.github.io/url-splitter/?urls=https://google.com,https://wikipedia.org
```

Display three sites and change the page title:

```
https://your_username.github.io/url-splitter/?urls=https://google.com,https://wikipedia.org,https://example.com&title=My%20Comparator
```

## Features

* Automatic layout based on the number of URLs
* Clean and minimal interface
* Fully client-side; no server required
* Each iframe loads from the client’s IP address

## Warnings

* Some sites may **block iframes** due to security policies (X-Frame-Options or Content-Security-Policy).
* All requests to the URLs come from the client’s IP, not from the server.

---

This project allows you to quickly and easily visualize multiple websites at once, making it ideal for comparisons or simultaneous testing.

