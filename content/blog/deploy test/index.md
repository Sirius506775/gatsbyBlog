---
title: deploy test

date: "2022-11-24"

description: 블로그 배포 후, deploy 테스트를 실시합니다.
---

> deploy를 하고 실제 페이지에 반영되기까지에 시간이 필요합니다..

### 아래 코드는 page-data.json 파일이다.

```json
{
  "componentChunkName": "component---src-pages-index-js",

  "path": "/",

  "result": {
    "data": {
      "site": { "siteMetadata": { "title": "DongHeon's Devlog" } },

      "allMarkdownRemark": {
        "nodes": [
          {
            "excerpt": "Far far away, behind the word mountains, far from the countries Vokalia and\r\nConsonantia, there live the blind texts. Separated they live in…",

            "fields": { "slug": "/new-beginnings/" },

            "frontmatter": {
              "date": "May 28, 2015",

              "title": "New Beginnings",

              "description": "This is a custom description for SEO and Open Graph purposes, rather than the default generated excerpt. Simply add a description field to the frontmatter."
            }
          },

          {
            "excerpt": "Wow! I love blogging so much already. Did you know that \"despite its name, salted duck eggs can also be made from\r\nchicken eggs, though the…",

            "fields": { "slug": "/my-second-post/" },

            "frontmatter": {
              "date": "May 06, 2015",

              "title": "My Second Post!",

              "description": null
            }
          },

          {
            "excerpt": "This is my first post on my new fake blog! How exciting! I'm sure I'll write a lot more interesting things in the future. Oh, and here's a…",

            "fields": { "slug": "/hello-world/" },

            "frontmatter": {
              "date": "May 01, 2015",

              "title": "Hello World",

              "description": "Hello World"
            }
          }
        ]
      }
    },

    "pageContext": {}
  },

  "staticQueryHashes": ["2841359383", "3257411868"],

  "slicesMap": {}
}
```