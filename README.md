<h1 align="center">「👁️🔑」 About Super Mantra</h1>

<p align="center"><img src="assets/banner.png"></p>

The tool in question was created in Go and its main objective is to search for API keys in JavaScript files and HTML pages.

It works by checking the source code of web pages and script files for strings that are identical or similar to API keys. These keys are often used for authentication to online services such as third-party APIs and are confidential and should not be shared publicly.

By using this tool, developers can quickly identify if their API keys are leaking and take steps to fix the problem before they are compromised. Furthermore, the tool can be useful for security officers, who can use it to verify that applications and websites that use external APIs are adequately protecting their keys.

In summary, this tool is an efficient and accurate solution to help secure your API keys and prevent sensitive information leaks.

## Help

```
Usage of supermantra:
  -c string
        cookies
  -d    detailed
  -ep string
        extra, custom (regexp) pattern
  -p string
        proxy, e.g. http://127.0.0.1:8080 or socks5://192.168.0.10:1080
  -r int
        max requests per second (0 = unlimited)
  -s    silent
  -t int
        thread number (default 50)
  -ua string
        User-Agent (default "Super Mantra v4.0")
```

## Usage

```
cat js-urls.txt | supermantra
echo "http://<js-url>" | supermantra
```

## Install

From go:

```
go install github.com/Rand0x/super-mantra@latest
```

From source code:

```
git clone https://github.com/Rand0x/super-mantra
cd super-mantra
make
./build/supermantra-amd64-linux -h
```

## Usage Docker

```
docker build -t supermantra .
echo <URL> | docker run -i --rm supermantra <options>
# or
docker run -i --rm supermantra <options>
# insert your URLs
```

### Coded by Brosck, UPGRADED by Rand0x

I saw this tool and liked it. It needed some upgrades, like a proxy, rate limiting, and so on. So, I added these features and called it Super Mantra.
Fork of https://github.com/brosck/mantra
