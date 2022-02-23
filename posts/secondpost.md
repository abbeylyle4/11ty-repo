---
title: Wikipedia API Contextualized and Leveraged
description: This is a post on My Blog about Wikipedia APIs.
date: 2022-02-23
tags:
  - number 2
layout: layouts/post.njk
---
First, an **application programming interface** (API) is a connection between computers or between computer programs that allow applications to talk to each other. They are very versatile and basically act like a mutual friend between both systems. 

We will be walking through how APIs are visualized, how they work, and how the JSON response is used. The example that we will be contextualizing is Wikipedia's API and how we can leverage it using the Wikipedia query tag.

## Fetch
The main goal for us here is to communicate with Wikipedia's API so that we can render their content on our own projects! We can do this by using the `fetch` tag. It is "behind the scenes" of the web component. It is what starts the process to retrieve information through APIs. In this case, the `fetch` tag is used to communicate with Wikipedia to find the respective article so that it can be rendered on the page. In the source code of the Wikipedia query, it shows the `fetch` tag requesting the address which then leads to the JSON API response.
![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/cqe45udiulbvjcoui1p9.png)

## APIs Visualized
The Wikipedia query tag communicates with Wikipedia's API service by searching for a Wikipedia article with the title specified. In this image of the Wikipedia query source code, you can see that the code is grabbing the Wikipedia article based on the search that the user will input. ![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/xw22bqe39ffvkgr95q6w.png)
To include the Wikipedia query in your own projects, the following syntax can be implemented. Below, we are specifying that the Wikipedia articles should be searched by the location specified by the user![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/zyb3c4o8au7w7dwqjyku.png)
**JSON Response and Display**
The JSON response is the default result of the fetch request because it is easily readable and easy to translate. When the JSON response is received, the web components are displayed on your own projects!

You can find more information about APIs [here](https://www.redhat.com/en/topics/api/what-are-application-programming-interfaces). For more information about the Wiki API, you can find its documentation [here](https://en.wikipedia.org/w/api.php)! For reference I have attached my own GitHub [repository](https://github.com/abbeylyle4/ip-project/blob/master/src/LocationFromIP.js).