# Code Exercise
The wellist coding exercise for applicants

## Goal
The goal of this exercise is to have you demonstrate a few software choices while
making the failing specs in this project work. This goal is in service of our
overarching goal of having as fair an evaluation of your skills as possible, in service
of making the best possible hiring decision.

## Domain Model
This test is cut (heavily) from our actual rails api project - our product is about
connecting users to vendors. We collect information from users and use that to provide
recommendations (a list of vendors) to them. From there, the user can "save" vendors to
a wellist. 

...at least, that will be the case once you implement the wellist api as we've spec'd out.
It's a very basic api: you PUT one or more vendor IDs to the endpoint, and the api should
always return the vendor objects which makeup the wellist.

## Getting Started
If you don't have a working ruby on rails development environment, or  experience
getting a ruby on rails development environment up, and you have a mac computer, 
we recommend our setup repositiory: [Mac Setup](https://github.com/GivewellGetwell/laptop)

The installation instructions you'll find there, plus the setup script in this
repositories `/bin` directory, should get you up and running.

Please feel free to reach out if you have trouble getting to a state where `rake` gives
you the following output:

```
12 examples, 11 failures

Failed examples:

rspec ./spec/models/vendor_spec.rb:4 # Vendor should have many wellists
rspec ./spec/models/user_spec.rb:5 # User should have many vendors
rspec ./spec/models/user_spec.rb:4 # User should have one wellist
rspec ./spec/controllers/api/wellist_controller_spec.rb:49 # Api::WellistController DELETE #destroy removes multiple vendors
rspec ./spec/controllers/api/wellist_controller_spec.rb:37 # Api::WellistController DELETE #destroy removes a vendor from the wellist when called with user id and vendor id
rspec ./spec/controllers/api/wellist_controller_spec.rb:63 # Api::WellistController GET #show shows a users wellist, with vendors inline
rspec ./spec/controllers/api/wellist_controller_spec.rb:18 # Api::WellistController PUT #update adds multiple vendors to the wellist
rspec ./spec/controllers/api/wellist_controller_spec.rb:27 # Api::WellistController PUT #update allows us to hide vendors from the wellistry
rspec ./spec/controllers/api/wellist_controller_spec.rb:9 # Api::WellistController PUT #update adds a vendor to the wellist
rspec ./spec/models/wellist_spec.rb:5 # Wellist should have many vendors
rspec ./spec/models/wellist_spec.rb:4 # Wellist should belong to user
```
