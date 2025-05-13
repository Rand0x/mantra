<<<<<<< HEAD
<h1 align="center">「👁️」 About Super Mantra</h1>
=======
<h1 align="center">「👁️🔑」 About Super Mantra</h1>
>>>>>>> b182841 (Switch to Super Mantra)

<p align="center"><img src="assets/banner.png"></p>

The tool in question was created in Go and its main objective is to search for API keys in JavaScript files and HTML pages.

It works by checking the source code of web pages and script files for strings that are identical or similar to API keys. These keys are often used for authentication to online services such as third-party APIs and are confidential and should not be shared publicly.

By using this tool, developers can quickly identify if their API keys are leaking and take steps to fix the problem before they are compromised. Furthermore, the tool can be useful for security officers, who can use it to verify that applications and websites that use external APIs are adequately protecting their keys.

In summary, this tool is an efficient and accurate solution to help secure your API keys and prevent sensitive information leaks.

## Help
![](assets/help.png)

## Usage
![](assets/usage1.png)

## Install

From go:

```
go install github.com/Rand0x/mantra@latest
```

From source code:

```
git clone https://github.com/Rand0x/mantra
cd mantra
make
./build/mantra-amd64-linux -h
```

## Usage Docker

```
docker build -t mantra .
echo <URL> | docker run -i --rm mantra <options>
# or
docker run -i --rm mantra <options>
# insert your URLs
```

### Coded by Brosck, UPGRADE by Rand0x

I saw this tool and liked it. It needed some upgrades, like a proxy, rate limiting, and so on. So, I added these features and called it Super Mantra.
<<<<<<< HEAD
Fork of https://github.com/brosck/mantra
=======
Fork of Github-Repo: https://github.com/brosck/mantra
>>>>>>> b182841 (Switch to Super Mantra)
