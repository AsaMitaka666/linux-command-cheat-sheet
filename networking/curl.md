# Linux curl Commands

`curl` is a command-line tool used to transfer data from or to servers using different protocols such as HTTP and HTTPS.

---

# curl

## Description

`curl` sends requests to URLs and displays the response.

## Syntax

```bash
curl URL
```

## Example

```bash
curl https://example.com
```

---

# Download Files

## Description

`curl` can download files from the internet.

## Example

```bash
curl -O https://example.com/file.zip
```

The `-O` option saves the file with its original name.

---

# Follow Redirects

## Description

`-L` follows HTTP redirects.

## Example

```bash
curl -L https://example.com
```

---

# HTTP Headers

## Description

`-I` displays response headers.

## Example

```bash
curl -I https://example.com
```

---

# GET Request

## Description

GET requests retrieve data from a server.

## Example

```bash
curl https://api.example.com/users
```

---

# POST Request

## Description

POST sends data to a server.

## Example

```bash
curl -X POST https://api.example.com/users
```

Send JSON data:

```bash
curl -X POST \
-H "Content-Type: application/json" \
-d '{"name":"asa"}' \
https://api.example.com/users
```

---

# Check Website Response Time

## Example

```bash
curl -w "%{time_total}\n" -o /dev/null -s https://example.com
```

---

# Authentication

## Example

```bash
curl -u username:password https://example.com
```
