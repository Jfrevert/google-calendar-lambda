# google-calendar-lambda

## About  

An `AWS` (Amazon Web Services) `Lambda` function for getting events booked into your `Google` calendar.
  
## How to use  

- Clone this repo  

  `git clone https://github.com/hughmp/google-calendar-lambda.git`  
  
  `cd google-calendar-lambda`  

- Install the dependencies  

  `yarn` or `npm i`  

- Install apex and configure `AWS`, as explained [here](http://apex.run/)  

- Set your `AWS` profile environment variable `export AWS_PROFILE=XXXXX` (in Windows use `set`)  

- Add your google calendar IDs into `config.js` in `functions/getBookings/src/`  

- Run `apex deploy -s GOOGLE_API_KEY=[INSERT YOUR GOOGLE API KEY HERE]`  

- Test your function `apex invoke getBookings`  

- You can now link an AWS `API Gateway` to invoke over HTTP  