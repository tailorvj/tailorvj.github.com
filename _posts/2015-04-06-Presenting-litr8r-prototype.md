---
published: false
---

## litr8r is for simultaneouse translation in live broadcasts

Live event translators rejoice, I've just published the first prototype of my litr8r live translation software for live broadcasts, codename Shoshana. This is actaully my first ever node.js project and relies on Express.js and Socket.io

The app currently consists of 2 simple views: Input and Output.

The translator runs Input and translates by simply typing phrases and pressing Enter to send to the output.

Output screen is sent to a video mixer, where it is mixed with live video using green screen Chroma key. If you don't know what that means, get a VJ wink emoticon

I'm going to run it in production on a Raspberry Pi in the yearly memorial service for Israelis and Palestinians live broadcast on April 21st.

I put up a demo (use Google Chrome) on Heroku and uploaded project to GitHub. Links:

[Input](https://tranquil-anchorage-5276.herokuapp.com/input)

[Output](https://tranquil-anchorage-5276.herokuapp.com)

[Github](https://github.com/tailorvj/litr8r)

Next stage for this project would be creation of separate translation rooms I guess. We'll see how it evolves from there.

Happy birthday litr8r.

