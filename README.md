# Weather-Site-Hands-on-Javascript-project

**Weather Site**
  Obtain your API key 
  Look at the API documentation 
  Configure two URL's 
    URL's Needed for JSON Data
      http://api.wunderground.com/api/c492cda67fd210ae/conditions/q/84653.json
      http://api.wunderground.com/api/c492cda67fd210ae/forecast/q/84653.json
      
      AJAX Request
        myObj.open('GET', 'http://api.wunderground.com/api/f029e46fd0232d12/forecast/q/84653.json', true);
        myObj.responseType= 'text'; // coming as a string
        myObj.send();
        myObj.onload= function() {
        if (myObj.status=== 200){
        x = JSON.parse(myObj.responseText);
        console.log(x);
        } //end if
        }; //end function
        
  Build the app 
  Test the page 
  Modification
