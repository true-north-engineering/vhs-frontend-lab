# VHS Rental shop - Blast from the past

Welcome to our frontend laboratory exercise deisgned for aspiring frontend developers like you who want to work with us on amazing projects. :)
Here you will find the task description along with its requirements. At the end, there is a guidance section where you will find notes on what
to do before you start working on the task and technologies you may use.

Keep in mind that it's not neccessary for you to fulfill all the requirements for us to consider you as a worthy candidate. We understand that sometimes you might have other pressing issues or you just have a lot of hobbies or even tasks you're doing for other interviews. Of course, the more you deliver and the cleaner your solution is, we will be able to assess your level of knowledge and experience better.

Let's go on with the task description now. We wish you happy coding and good luck with this assignment! :D

We are creating a cutting edge VHS rental application management system for our special clients that value the old time retro VHS experience.

![img_1.png](backtothepast.png)

### VHS Rental Application

Think of this application as a digital VHS shop. We would expect such an application to provide an interface where users could browse the
VHS catalogue, see details on specific items and maybe even be able to search through the catalogue by typing a term in a text input.

If you were the manager of such VHS shop, an application like this would be expected to provide functionality of creating new VHS items for the catalogue,
as well as being able to update existing VHS items or deleting them from the catalogue altogether.

We will make things a little bit simpler for this version of the lab by not including user management in the frontend. That means that functionalities like
login, registration, forgotten/reset password or logout are not necessary. Every user can access all the functionalities.

Additionally, we will provide you with a finished VHS backend service that you can just run and start sending HTTP requests to it and it will just work (unless it doesn't, in which case just email us and will solve the issue :D).

This brings us to the question of what then needs to be done exactly? Well, here is a list of requirements.

#### Requirements

- make a screen that represents the VHS catalogue (list all VHS items available)
- make a screen where the user can see details of a specific VHS item (screen where the user ends up when they click on an item in the catalogue)
- make a screen where the user can create a new VHS item that will be submitted to the catalogue (there needs to be a form that the user fills out and then submits it)
- when creating a new VHS item, allow the user to upload a thumbnail image of the movie (see additional info below)
- make a screen where the user can edit an existing VHS item (same form as when creating a new VHS item, but this time the form is automatically filled with existing data and the user can edit it)
- make it possible for the user to delete an existing VHS item
- add a simple search input on the VHS list page where the user will be able to search the catalogue by item title
- all of above operations need to communicate with the provided backend service (e.g. using axios)
- don't forget to do simple routing between pages (selecting a VHS item goes to details page, but user should be able to return to the homepage by clicking some navigation button etc.)

Additional info:

- when creating new VHS items, you need to have the following fields
  - title (movie name)
  - description (short description of the movie, like a synopsis)
  - genre (movie genre)
  - duration (movie length, in minutes)
  - releasedAt (year of movie release)
  - rentalPrice (price of rental, an integer)
  - rentalDuration (length of one rental in days, e.g. 3 days)
  - quantity (how many tapes of this item are currently available in the shop)
  - thumbnail (small image that represents the movie, it needs to be uploadable from the user's computer)
- all of those fields need to be editable as well as show up on the details page of a VHS item

#### Bonus requirements related to UI/UX Design

This is an optional list of requirements that you can try to fulfill if you have some past experience with UI/UX Design. Sometimes we need to work out what our screens are going to look like
before implementation and it's always a bonus if you can help out in this manner. Keep in mind that the development part is of the highest priority here, so if you don't have too much time it's better to
deliver more code than design. :)

For making screen designs, you can use whatever you see fit. Some of us who tried working with UI/UX used Figma, so this is our preference.

You can do whatever you want considering the design. You have full freedom here. :)

- create a Figma design for each screen mentioned in the main requirements
  - VHS item list
  - VHS item details
  - create new VHS item form
  - edit existing VHS item form

# Guidance:

### Setup your account and repository

1. Setup your GitHub account if you don't already have it
2. Fork your own repository from the original one
3. Create your own branch
4. Add your mentor as member to your repository with role Maintainer

### Run provided backend service

In this repo you can see the vhs-backend folder which contains a finished VHS backend application written in NestJS (a backend framework based on NodeJS). For details on how to run it, you can check out the README.md file in vhs-backend folder. You will need to have Docker and NodeJS 16 installed for that, but you will find more details in the backend readme file.

The backend also contains the REST API specification you will need to complete this assignment. It uses Swagger UI which is available at http://localhost:3000/api once you run the backend server. There you will find all API routes you can call from your frontend as well as their detailed description (what they take as input in the request and return as a response).

If you're not able to run the backend or something doesn't work, contact us and we will help you with it.

### Tech stack

We use React + Typescript to write frontend for our projects so we would prefer if you also used React. However, it is not necessary at all.
If you have more experience writing in Vue.js, Angular, Svelte, or just pure JavaScript that's good as well, feel free to implement the solution however you know.

Usage of Typescript is a bonus, but also not necessary. Additionally, your application can be a classic Single Page Application (SPA), but you can also use technologies like NextJS which
allows server side rendering or incremental site regeneration and other cool features.

Just don't write a mobile app, we're targeting browsers, so the only requirement is that your build uses HTML, CSS and JavaScript. :)
