# Introduction to APIs

## Learning Objectives for this section

- Describe what an API is and why we might use one.
- Explain the common role of JSON on the web.
- Introduce the native ES6 `fetch()` method to make GET requests for data.
- Render a React component using data loaded from a `fetch()` request.

## What is an API?

**What is an API?**

> Basically, an API is a service that provides raw data for public use. As third-party software developers, we can access an organization's API and use their data within our own applications.

What if you want a Google map embedded in your web app to show people where they can visit you? You aren't going to make that map yourself, so somehow you have to call Google. Well, Google has an API you can call to get the map information - all you have to do is send a request to the API that Google provides, and Google gives you a google map back that you can use.

API stands for "Application Program Interface" and technically applies to all of software design. The DOM and jQuery are actually examples of APIs! Since the explosion of information technology, however, the term now commonly refers to web URLs that can be accessed for raw data.

> Q: Why do we care?

Why recreate data when we don't have to? Think about past projects or ideas that would be easier if you could pull in data already gathered elsewhere.

APIs can provide us with data that would we would otherwise not be able to create ourselves.

As we move into building single page applications, now is the perfect time to start understanding how to obtain data on the client side and then render it on the browser.

## API Exploration

There are a variety of APIs available on the internet. To call an API, send a request to a URL, and that API returns data to your program. You can pull data from anywhere that offers an API.

You can make this request as specific as you'd like - each web app out there offers different options for their API. You just have to find out from them what you can request!

Here are just a few examples of APIs that you can use. Check it out - the left column is the common name you might know. The right column is the URL you, in your program, would send a request to. You can click those URLs to see what each call would return.

| What's the API? | Sample URL - you call this |
|------|------------|
| **[Giphy's API: request a list of all funny cats](https://github.com/Giphy/GiphyAPI)** | http://api.giphy.com/v1/gifs/search?q=funny+cat&api_key=dc6zaTOxFJmzC |
| **[OMDB's API: request list of Game of Thrones Season 1 episode info](http://www.omdbapi.com/)** | http://www.omdbapi.com/?t=Game%20of%20Thrones&Season=1 |
| **[The Star Wars API: request R2-D2 info](http://swapi.co/)** | http://swapi.co/api/people/3 |
| **[Markit Digital's API: request current Apple stock info](http://dev.markitondemand.com/MODApis/)** | http://dev.markitondemand.com/Api/Quote/xml?symbol=AAPL



> Does the JSON look unreadable in the browser? If you're using Chrome, install the [JSON View plugin](https://chrome.google.com/webstore/detail/jsonview/chklaanhfefbnpoihckbnefhakgolnmc?hl=en).


### Hmmm.

Can you think of any websites you go to that pull information from other places, so they probably use an API?
