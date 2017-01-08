#ALLERGO-SCAN

![Image of Allergo-Scan](https://github.com/laurage/allergo/blob/master/allergo.jpg)

#Introduction

This app has been built by a team of four people over nine days and was the second of two projects during our time on the Web Development course at [Le Wagon](https://www.lewagon.com), Nantes (France). The requirements of this project were to build an authenticated RESTful Rails application. A hosted version of **Allergo-scan** can be found [here](http://www.allergo-scan.com/) The code can be viewed [here](https://github.com/laurage/allergo).

#The App

**Allergo-scan** is a web app which lets users scan supermarket products' barcodes and warns them when they are allergic or intolerant to some of the product's ingredients.
It uses [Open Food Facts](https://world.openfoodfacts.org)'s API, a website that lists more than 100 000 products and their ingredients.

To fully benefit of the experience of the scan, access the app on your computer or an Android device using the Firefox browser. Otherwise, manual input or search by name are also possible.

#How to use the site

Upon registering each user is prompted to fill their allergic profile, with the degree to which they are allergic or intolerant to each ingredient. At home or at the supermarket, they can scan products and are told whether or not they can eat the product.
If the product isn't in the database, they are asked if they'd like to add it to it.
They can choose to follow products they consume regularly, and receive in-app alerts and email alerts if the products composition changes in ways that affects their allergy.

#How it was built

**Allergo-scan** is a Rails application. It was made using Bootstrap CSS framework, SASS, JS, jQuery, and Ruby.

The search is implemented with [pgSearch](https://github.com/Casecommons/pg_search) and [Algolia Search](https://www.algolia.com/).
Authentication is enabled by [Devise](https://github.com/plataformatec/devise) and [Omniauth-Facebook](https://github.com/mkdynamic/omniauth-facebook).

I used Illustrator and Sketch to create the wireframes & UI.

#Challenges during the build

Using the Open Food Fact database proved itself challenging. Its strength is based on its collaborative approach: anyone can add a product to it. However, the validations are minimum which means many products are listed several times and the data collected is often inconsistent. Ideally, it would require either to work in partnership with Open Food Fact to help them check their data more consistently from the start or to clean the database before using it. Another approach could be to work with supermarkets and brands directly so they provide us with first hand data.

One of our main concern through the project has been to accurately identify products. We had to find a scan that would work on mobile, which turned out to be very challenging. We also realised as we tested it that lighting conditions and size and material in which the barcode is printed highly affects recognition rates. Being such an essential part of our app, this would be the feature I would focus on first if I was to pursue the project.

#Getting started

These steps are required in order to run the application:
*1. Ruby, Rails and Postgresql must be installed
*2. Install the gem of the Gemfile: $bundle install
*3. Run $rails server and go to [http://localhost:3000](http://localhost:3000) in your browser to view the site.

#Credits

* The font used throughout the site was taken from [Google Fonts](https://fonts.google.com/)
* The icons used in this project where taken from [The Noun Project](https://thenounproject.com/)
