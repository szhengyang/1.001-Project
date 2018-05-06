*Web access is required

To test the product locally:

1. In the node.js terminal, run node --max-old-space-size=8192 app.js 

   In the console, look out for the message 'tree created'. Takes about 5 minutes. 

2. In chrome, access the address: localhost:8081/index.html

3. At the bottom of the page, after filling up the details, clicking 'Submit' will take
   the user to the results page. 


During the product demo, the AWS server was used. However, an extra large server with 16GB
of RAM was purchased to run the algorithm. With cost considerations in mind, the EC2 
instance was only run for the product demo.  