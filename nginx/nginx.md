% Nginx and Regex 
% Sudhanshu Dubey
% 24th August 2019

## What is Nginx?

> nginx [engine x] is an HTTP and reverse proxy server, a mail proxy server, and a generic TCP/UDP proxy server, originally written by [Igor Sysoev](http://sysoev.ru/en/).

- The above is how Nginx [define themself](https://nginx.org/en/).
- For us simple folks, its a webserver.

## Nginx vs Apache

- From [this site](https://www.hostingadvice.com/how-to/nginx-vs-apache/) we can get a nice and brief comparison of the two.
- What we experience is that Nginx is smaller and faster.
- But, compared to Apache, its a lot difficult to configure.

## What is Regex?

- Regular Expressions (Regex) are an excellent way to search for patterns in any text.
- Its quite intimidating for beginners but is an extremely valuable tool once you get your hands on it.
- You can learn regex from [here](https://medium.com/factory-mind/regex-tutorial-a-simple-cheatsheet-by-examples-649dc1c3f285?source=email-f233d69a16f5-1565139564660-digest.reader------0-49------------------b13881b2_1fc2_470c_af03_4868c26244c7-1).
- And then practice it [here](https://regex101.com/).

## Nginx + Regex

- The configuration of Nginx mostly depends (from my experience) on how you are checking the [location](https://nginx.org/en/docs/http/ngx_http_core_module.html#location).
- And location can be pattern matched using Regex.

## CGI on Nginx

- [FastCGI](https://www.nginx.com/resources/wiki/start/topics/examples/fcgiwrap/) is how you get Common Gateway Interface in Nginx.
- In the above instructions, we are given a default configuration file.
- To use CGI in Nginx, we need to somehow pass the address of the file to fcgiwrap.socket.

## Problems for Userdir

- ``Userdir`` means that each user has it's own public_html directory.
- The path becomes variable and that's troublesome.
- If correct path is not provided, the file will get downloaded.

## My solution

1. Use regex to get path
1. Do not use ``root``.
1. Use fastcgi_param instead to pass the path of the file.

## Thanks
