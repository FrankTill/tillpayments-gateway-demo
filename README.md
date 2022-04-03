# Demo code for working with Till Payments Gateway in Python
## What is this
This is some demo codes about how to work with Till Payments gateway. As of now, it demos the following scenarios.
* Send a signed debit request
* Validate the signature of postback requests from the gateway.
Detailed documentation can be refered [here](https://gateway.tillpayments.com/documentation/apiv3)
## Some tips about the signature
Apart from what's mentioned in the official docs, based on my experience, attention needs to be paid on the fololowing:
* Please strip all the white spaces off the payload before hashing it
* In some languages, like Python, when stringify JSON, the default quotation marks are single quotes. You'll have to make it double-quotes.

Frank@Till