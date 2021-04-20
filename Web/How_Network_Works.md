### Concepts

**Networks**

- A set of computers that can intercommunicate

**Internet**

- A larger version of network. Internet is made up of small "local networks"

**Web**

- An information system where documents and other web resources are identified by URL, which are accessible over internet

**IP Address**

- A unique address to find a computer an the network.

**DNS (Domain Name System)**

- It's likea phone book for a web. Take hostname and translate it to corresponding IP Address and vice versa.

**URLs (Uniform Resource Locator)**

- Port
  - Every server has 65,535 unique "ports" you can talk to - unless specified, it will use default port.
  - HTTP default port is 80
  - HTTPS default port is 443
- Query String
  - You can pass in multiple arguments - separated by '**&**'

Structure of URL

![image](https://user-images.githubusercontent.com/44216709/115333478-b8db1100-a167-11eb-8680-353e29352c8d.png)


### How network works?

Two issues when multiple computers are connected

1. How do we identify each unique computer?

2. How do we connect each of them?

Each computers are linked together through a router. As the number of computer increases routers will communicate with routers from other networks. Here, IP Addresses are used.

How ever these IP Addresses are not easy to memorize. So, we use hostnames to talk to servers - [site.com](http://site.com) / computer-a.site.com. Here, DNS is used to translate these hostname into corresponding IP Address for the server - and vice versa.

_\*\* 127.0.01 - this computer that you're on. The name of _[localhost](http://localhost)\* always maps to this IP address.
