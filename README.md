## Inspiration
When shopping on Amazon, I've been noticing that it's hard to forget to add a needed item to my order. The website suggests similar items, "also bought with" items, and other items I may be interested in. What if it was that easy to avoid forgetting something on an everyday trip to the grocery store?

## What it does
Some large grocery stores around the world are adding screen-based advertisement mounted on the cart itself. Carted takes this concept a step further, with both front and rear view cameras. Carted employs facial recognition to recall past purchase history and combines that information with the contents of your cart in real time. For example, if you have spaghetti noodles, marinara sauce, and french bread in your cart and are headed to the checkout, Carted may then ask if you forgot to buy parmesan. It then can also suggest new items, or alert the customer about sales on items they usually buy. Imagine how helpful this could be to the busy mom who has absolutely no time to make a second trip to the grocery store!

## How we built it
It is a multitier architecture centered around individual functionality. 
  - Service Layer - This is a Centralised service endpoint, which interacts with other layers. 
    - Basic responsibilty is to interact with other layers.
    - Communicate with Google Cloud to detect objects.
    - Interacts with Firebase and Algolia to do data operations.
    - Service endpoint for UI
  - FaceRecog - This layer is responsible to recognize users, using pre-trained models. 
  - UI Layer layer- End user interface.
  - Database  - Firebase
  - Search Layer - Algolia
## Technology Used
 - Face Recognition - Python, OpenCV and Deep Learning
 - Object Detection - Google Cloud Vision API
 - Rest API - C# Web Api
 - Database - Firebase
 - Full Text Search - Algolia
 - UI - Angular 1.6

## What's next for Carted
We plan to improve our model and continue to make it more reliable and accurate, 
adding extensive security and privacy features, and also implementing a new GPS 
feature which will guide the customer toward the location of the desired product in the store. 


Created as part of Hackathon Project - HackKU 2019
