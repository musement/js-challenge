# Javascript Developer coding challenge

Using the assets provided, your task is to build a simple e-commerce application. 

Please, read all sections within this document carefully.

Points marked as optional and Extra Credits are entirely up to you. 
They will give you the chance to shine within the selection process but they are not required.

With the ["Guidelines"](#Guidelines) section in mind, you should complete at least the following required features.


## Required features

* Develop a simple build system for your application

* Avoid to use ANY external libraries for components or services

* Develop the “Add/Remove to Bag” and “Add/Remove to Wishlist” actions which work con client side only

* The page must show 6 activities on page load. Find the best way to browse the catalog and show more activities

* The bag in the header must be updated with the new quantities and the new total price

* Make the application responsive, in your own taste ( CSS )

* Unit testing on functions and components where you think it's appropriate

* [optional] Build a mini-bag with convenient actions, coherent with design. Example of a mini-bag is included within the images folder but you must develop a mini-bag that’s coherent with the page’s design.



## Guidelines

You can use Vuejs or React framework built with Webpack, you can start with the boilerplate you want

You must use the given API calls to retrieve activities(products) and you can choose any API client to work with

All code produced should have modularity, reusability and performance in mind, while being well documented

In the end, you should have a build task to output a production ready folder (e.g.: dist) with all your work as well as the source code that generated it.
This folder must not be committed and instructions to produce it must be provided in order to let us run the application in production mode.

If not specified in the design, it’s up to you to decide what’s best

You can't link to external resources, if necessary include them in your solution package


## API docs
- This is the basic curl to retrieve a product listing. You'll have to implement client API calls to get paginated response. The "limit" parameter is used to retrieve a defined number of items, "offset" is the number of items to be skipped
```
  curl -X GET \
    'https://api.musement.com/api/v3/activities?limit=6&offset=0' \
    -H 'accept-language: it' \
    -H 'content-type: application/json' \
    -H 'x-musement-currency: EUR' \
    -H 'x-musement-version: 3.4.0'
```
- From the call above, consider these response props:
```
  * cover_image_url => is a URL string where you have to append this query string to make a responsive image ?q=60&fit=crop&w=[image_width_in_px]&h=[image_height_in_px]
  * title => product title
  * description => product description
  * retail_price => the product price
```
Please refer to [this page](https://api-docs.musement.com/reference#get_activities) for documentation.


## Extra credit 

* Use CSS preprocessors

* Use of linting tools

* E2E testing

* Performant code

* Fast page load

* Optimized user experience

* Statically typed code



## Delivery

Create a **private Git repository** with the following format: 

	js_challenge_<first-name>-<last-name> 

[Github](https://github.com) allows private repositories for free, you only need to grant us access to it afterwards.
Please, use these accounts: dotBits, przemkow, zi, gionatan-lombardi

Commit your work as you progress, we look at the commit history as well

You can delete the contents of this README and replace it with content of your own



## Eliminatory Points

Not following these points may cause an immediate elimination:

* Project is delivered in any way other than in a private GIT repository
* The project's [Required Features](#Required Features) aren’t fulfilled 
* Lack of build task to output production ready (e.g.: dist) folder
* Lack of instructions to run the project



## Assets Provided

* SVG icons
* Fonts
* HTML code - index.html
* CSS code - main.css
* Sample Image - main.css
* API docs
