# Exploring Remix

To start the app run `npm run dev`.

I've seen Remix mentioned a few times now, which is usually my signal to spend a little bit of time playing around with it to see what it's all about. I followed the [15 Minute Introductory Tutorial](https://remix.run/docs/en/v1/tutorials/blog) and had a great time with it. 

For context, my experience of web development up to this point is mostly React frontend development talking to a Django Python API. The appeal (and selling point) of Remix is the merging of those two pieces into one framework. I was curious what the difference would be between the traditional Django serverside rendered applications, after having spent some time with Remix my current opinion is that it's no different, it's just a lot more "Reacty" than Django templating which makes frontend development a lot easier and more pleasant to work with.

# Thoughts (In no particular order)
 - I like the JSX and that it has the look and feel of simple HTML. Templating in JSX is very familiar to me due to React, and it felt natural building out FE pages.
 - I really like the BE being right next to the FE. I am tired of opening up the Django BE API in another window, making changes, verifying the output is as expected, then making changes to a React FE component to fetch that data, display it etc. BE/FE communications can get very chatty when data is being submitted, particularly if data validation is being done on the backend and must be communicated back to the frontend. With Remix I was making a change at the top of the file, then simply scrolling down to edit the FE. It's very clear how the code is separated out, the function Post() for example is the part that renders the UI, much like in React. The loader() and action() functions define the BE behaviour. I think I still need to get my head around exactly which bits of code run on the FE, and which on the BE, but in my mind the Posts() function was for FE and the other two were for BE logic, clearly delineating the two and making it easy to think about information flow between them.
 - 
