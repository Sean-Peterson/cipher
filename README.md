# Cipher

Cipher is a Drupal website that uses a custom module to encrypt user messages.

## Requirements

* It should present a custom form with 3 text inputs. We want you to use text inputs rather than radio buttons or menus so that you can practice validation.

* One input should be a shift value, one should be a direction, and the third should be the phrase to be encrypted.

* Then you should redirect to a second page to show the result - the encoded phrase. Here are a couple examples of input and output.

* The shift value is the number of places to shift each letter over.

* If the shift direction is "right" then you will add the shift value. For example: "a" with a shift value of 1 and a direction of right would become "b". A shift direction of "left" with a shift value of 1 would turn "b" into "a".

* If the shift amount takes you over the bounds of the alphabet then cycle back to the beginning. For example: a shift value of 3 with the direction of right would turn "z" into "c".

* Any spaces or punctuation in the input phrase should be ignored and reproduced in the final result without being shifted.

* Your final result should be in all lowercase.

## BDD
1. Input:
  Shift value = 3
  Shift direction = right
  Phrase = "hello"

  Output:
  "khoor"

2. Input:
  Shift value = 1
  Shift direction = left
  Phrase = "hi there!"

  Output:
  "gh sgdqd!"

### Form validation:

* The shift value must be a positive integer

* The shift direction must be either "left" or "right".

* The only special characters that should be allowed in your input phrase are spaces and punctuation.

## To run Bookstore from a personal computer:

You will need the following properly installed on your computer.

* Git
* PHP
* MAMP

## Installation

**Step 1**: Clone this repository to your local computer

```console
git clone https://github.com/Sean-Peterson/drupal-bookstore
```

**Step 2**: Open mamp and set port: apache port: 8888 and mysql port: 8889

**Step 3**: Set mamp configuration web server to the project directory

**Step 4**: Open a web browser and navigate to localhost:8888/MAMP/ and then click on the phpMyAdmin link

**Step 5**: Click on Import, choose file, and select drupal-bookstore/sites/db-backup/bookstore.sql

**Step 6**: Start MAMP servers

**Step 7**: In your web browser navigate to localhost:8888
