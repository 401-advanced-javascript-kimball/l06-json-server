# l06-json-server

### Author: Jonathan Kimball

### Links and Resources

* [submission PR](https://github.com/401-advanced-javascript-kimball/l06-simple-api/pull/2/)

#### Documentation

* Could not do this correctly!  Swagger hub is failing to import more than one route at a time!
  * [swagger hub page](https://app.swaggerhub.com/apis/JAKimball/default-title/0.1)

## Requirements

### Build a working JSON Server

* [x] Implement an API server suitable for a storefront, using json-server
  * [x] Install `json-server` globally
  * [x] Create a new repository called "simple-api"
  * [x] Create a folder called `data` with a `db.json` file
  * [x] Start json-server from within the `simple-api` folder and "watch" your database file
    * [x] `json-server --watch=./data/db.json`
  * [x] Data models should contain the following fields:
    * [x] `categories`
      * [x] `_id`, `name`, `display_name`, `description`
    * [x] `products`
      * [x] `_id`, `category`, `name`, `display_name`, `description`
  * [x] Your api will (should) respond to the following endpoints:
    * [x] `/categories`  
      * [x] GET
      * [x] POST
    * [x] `/categories/:id/`
      * [x] PUT
      * [x] DELETE
    * [x] `/products`
      * [x] GET
      * [x] POST
    * [x] `/products/:id/`
      * [x] PUT
      * [x] DELETE
  * [x] Use `httpie` (command line) or Postman to POST some categories and products into your API so that you have some data in there. 
  * [x] Confirm that GET, PUT, and DELETE also work

* [x] Connect a web server
  * [x] Open this [React Application](https://codesandbox.io/s/w638oyk7o8) and "Fork" it
  * [ ] Open the .env file and enter the URL to your API Server (if it's not running on http://localhost:3000)
  * [x] This server is configured to use the routes noted in the first lab requirement
  * [x] If your lab is working, this app will show your API Data!

* [x] Swagger Documentation
  * [x] In your API, Create a folder called `docs`
  * [x] Go to swagger.io and use the Inspector application to test your api
  * [x] Write and publish swagger documentation with Swagger Inspector
    * [x] It will publish it to "Swagger Hub"
    * [x] Convert the YAML to JSON and then copy and paste swagger.json from the editor and add to your server project.
    * [x] For submission, this file needs to be in your repository
      * **Swagger does not seem to be currently operating correctly when selecting multiple routes to document.  Rather than try to combine the resulting files, I've just included all routes in individual files in the docs folder.**
    * [ ] Additionally, add the URL to the swagger hub page where you build the docs to your README.
      * Could not do this correctly!  Swagger hub is failing to import more than one route at a time!
      [swagger hub page](https://app.swaggerhub.com/apis/JAKimball/default-title/0.1)

### Testing

**No automated testing is required for this assignment**
