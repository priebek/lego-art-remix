# Lego Art Remix
Easily remix Lego Art sets into custom pictures using computer vision

You can find a deployed version at [lego-art-remix.debkbanerji.com](https://lego-art-remix.debkbanerji.com/)

Made with ♥ by Deb

![Lego Art Meta Picture](https://raw.githubusercontent.com/debkbanerji/lego-art-remix/master/app/favicon.png)

## What is it?
In 2020, The Lego Group released the [Lego Art](https://www.lego.com/en-us/campaigns/art) theme, which allows people to create a predetermined image using lego studs.

Lego Art Remix lets you upload your own image, and then uses computer vision to use the studs from a Lego Art set that you already have to recreate the image.

This project is not affiliated with The Lego Group.

## Performance and Security
The computer vision techniques used are pretty inexpensive, and the resolutions being dealt with are naturally quite low, so as of the time of writing, the algorithm runs quite quickly. This allows for it to be run on the client, and on the machines that I tested, it ran in near real time.

The most computationally expensive part of the process is generating the instructions, since even pdf generation is done client side.

Since it runs entirely within the browser, no image data is sent to a server and so it's very secure.

## Bugs, Feature Requests, and Algorithm Improvements
*Direct any concerns or ideas for improvements to the [issues tab](https://github.com/debkbanerji/lego-art-remix/issues)*

As of the time of writing, I don't have all of the sets, and I haven't had much time to test. As a result, there's probably quite a few bugs, so let me know if you find any.

There's many features that could be added, such as more/custom resolutions or more flexible set selection. I can get to these if there's enough need.

Algorithm improvement ideas are always welcome. Improvements that maintain the efficiency to within a reasonable degree would allow the algorithm to keep running on the client, which I really like. That being said, putting in the work to add a server side computation option would allow for more complex approaches (such as constrained VAEs, etc.).
            
