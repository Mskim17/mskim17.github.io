---
layout: post
title:  Strapi Setting
date:   2022-09-06 15:50:35 +0300
image:  strapi.jpg
tags:   Resources
---
Strapi Setting

## 1. 버전 정보(Version Information)

* OS : Ubuntu 20.04LTS
* Node : 14.19.2
* Mysql : 8.0.30

### 2. Strapi 설치 (Strapi Install)

{% highlight markdown %}
PREREQUISITES

The installation requires the following software to be already installed on your computer:

Node.js (opens new window): only LTS versions are supported (v14 and v16). Other versions of Node.js may not be compatible with the latest release of Strapi. The 14.x version is most recommended by Strapi.
npm (opens new window)(v6 only) or yarn (opens new window)to run the CLI installation scripts.
Python (opens new window)when using a SQLite database
{% endhighlight %}


{% highlight js %}
  npx create-strapi-app@latest my-project
  yarn create strapi-app my-project
{% endhighlight %}


### 3. Strapi Issue

* Product / Develop 방식에 대한 Strapi 정책 참고

https://github.com/strapi/strapi/commit/a52a2eae43c0491d25aaa37c475d7f3887578083