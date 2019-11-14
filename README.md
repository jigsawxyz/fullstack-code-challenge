# Full Stack Challenge - Pictsy

Your task today is to write the code for Pictsy, a sexy new image sharing startup. Since we're starting from scratch, we'll need to build a REST API as well as our web app.

Here at Jigsaw we tend to use React & Redux for Web Apps, Node.js w/ Express.js for our API layer, and PostgreSQL for our SQL database.

However, you may use any technology stack you wish to complete the challenge. Also, don't bother hooking up a database or any remote services - please keep your data in memory and store images on the local file system. Which means you might want seed / bootstrap / teardown scripts to manage the state.

Feel free to use any libraries in your toolbox to complete the challenge, and please timebox yourself - you should be able to accomplish most to all of this in 4 - 8 hours.

OK! Are you ready to go?

## The Pictsy API 

Pictsy's CTO has asked you to build the API and Data layers for Pictsy's image services. She's kind of a stickler for tests, so make sure that all your functionality is tested, atleast along the happy path.

The Pictsy API should have the following endpoints:

#### -- Create
`HTTP POST /images`

The create endpoint should accept a valid image as input, generate a unique id representing the image, store metadata about the image, and save the image to the file system.

#### -- List
`HTTP GET /images`

The list endpoint should return a list of all images that are stored, ordered by the date they were created.

#### -- Show
`HTTP GET /images/<unique_id>`

The show endpoint should return the image file.
If the image id does not exist, it should return a 404 NOT FOUND error.

#### -- Data
`HTTP GET /images/<unique_id>/data`

The detail endpoint should return all data held about a single image record, retrieved by ID. 
If the image id does not exist, it should return a 404 NOT FOUND error.

#### -- Tag
`HTTP POST /images/<unique_id>/tags`

The create tag endpoint should tag an image with some text.

#### -- Get by Tag
`HTTP GET /images/tags/<tag_name>`

The get by tag endpoint should return all images tagged with given text.


## The Pictsy App

The product manager at Pictsy has asked you to build out a concept for the “browse” page of the website. Visually, they would prefer something minimal and clean. Feel free to borrow the style of any popular image browsing website.

Your app should display correctly on both desktop and mobile.

At the next meeting you need to have a demo that has these features:

* Display a collection of images

* Click on the images to get a closer look at them

* Add a tag to an image

* Filter images based on tags

---------------------------------------------------------------------

If you have any questions, comments, concerns, please reach out and talk to us. We are more than happy to discuss.

Good luck!
