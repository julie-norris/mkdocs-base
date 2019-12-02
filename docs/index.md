# Welcome to My Technical Take Home Page

## Questions

#### Rank your 5 favorite, and 5 least favorite, activities from this list: 
### [5 favorite and 5 least favorite Things a Support Engineer Does](https://gist.github.com/fool/b0f254ff8c72a5765b6a9138249789d6)

* Top 5:

    1. Receive occasional phone calls requesting support from our highest-value customers
    2. Work with people to figure out if Netlify's service can solve a particular workflow or integration challenge
    3. Submit bug reports and potentially bug fixes to closed and open source projects that Netlify maintains on GitHub
    4. Spot trends across many cases to improve Netlify's product and service
    5. Create video tutorials to help teach users a specific feature or use case

*  Bottom 5:
    1. Work with prospective customers to explain our service and the pricing model
    2. Manage a Support team
    3. Respond to Netlify customers on Twitter
    4. Deliver a talk to many people you don't know at a conference or meetup

(There really aren’t any other list items that are dislikes for me)



#### What is your favorite thing about providing technical support?

My favorite thing about providing technical support is finding the answer to the problem and then being able to share the solution with the customer. Seeing the customer’s satisfaction when I am able to provide a solution is really rewarding. And it starts to build great rapport so that the customer has confidence in my ability to help them when there are more challenging problems down the line. 



#### What did you think of our service during the time you used it?  Provide either some constructive criticism or some points that impressed you.  Be honest!  “It sucked” isn’t a wrong answer unless you don’t elaborate and provide some constructive criticism ;)

My first experience with the service was to create my personal website. I used some boilerplate templates to create my personal website and when I used Netlify to deploy the site it was very simple and easy and deployed quickly. 
Using the staticgen website proved to be a bit more challenging because I encountered errors in trying to deploy.  One issue was that the server was running but I got a 'page not found' error. It would be hugely benficial if the resulting alert box says "it’s working but there is no content". 



#### Talk about how you made your site and why you chose the tools you did.  Briefly explain a challenge you experienced in setting up this site and how you solved it.

Initially when I looked at the options on staticgen.com I thought I would use Jekyll because I had used that to make my personal website. Then I decided to do some research about the other options and gave some of them a try. Ultimately I decided to use the mkDocs generator because it is a good template for writing documentation. This made sense given the task of answering the questions for this interview exercise. I followed the instructions on [Netlify Common Configurations Documentation](https://docs.netlify.com/configure-builds/common-configurations/#mkdocs).
While I was testing different generators, before I decided to use mkDocs, I ran into the same error several times. The log was showing that the deploy succeeded, but the site was giving an error message. After adding content to the site this error no longer occurs. This can be confusing and different wording in the error message would be useful to end users. 


#### Provide a link to documentation for a technical/developer-focused product, which you think are well done, and briefly explain why you think they are well done.

[Twilio REST APIs](https://www.twilio.com/docs/usage/api)

I think the Twilio API documentation is well done. I used it when I added SMS messaging to my app, Carpool! that I created during my Hackbright Academy Fellowship.  The documentation is well done because it starts with some general explanation about APIs and authentication. The docs then go on to provide small digestible chunks of information specific to different functionality of their product with examples. As a new developer when I created my app I was able to read through the information and look at the sample code and apply it to my own needs. 



#### Why do you think SSL/HTTPS is important? 

Because we should all be concerned with security! Using SSL/HTTPS gives us a level of security that HTTP did not. The data between the browser and the server is encrypted when using SSL/HTTPS so that no one can read it. This was not the case with HTTP.   Certificates guarantee that the site being accessed is the correct site and prevents phishing sites from gaining accessing. 



#### Explain, in a couple of paragraphs, what you think 2 major challenges around DNS configuration are for less-technical internet end-users.

There are two major challenges around DNS configuration for less-technical internet end-users when they type in a URL and get an error saying that the page doesn’t exist or isn’t available. 
The first challenge is that the DNS might not be up to date. In that case the end user would get an error until the DNS is updated. This might take some time. The second issue is that the IP address may have changed and the device being used has the old IP address cached. In order to reach the website, the user will need to clear the cache. 



#### A customer writes in saying their “site won’t build”.  
Compose:
o	your best short (2-paragraph) customer-facing answer, 
o	without any additional data, 
o	that could be useful in the generic case, 
o	but would also lead to a customer providing a more actionable response.  

To problem solve, take a look at the log. What does the log say? Some frequent errors are :exit status 128, command not found, and case sensitivity. If your error is :exit status 128, try this: eliminate the error: (go to Settings > Build & deploy > Continuous deployment > Build settings, select Edit settings, then Link to a different repository). If your error is “command not found”, you may not have added the software required for that command hasn’t been installed in your build. You may need to add a Gemfile, requirements.txt, or pakage.json depending on which language you are using. For a ‘case sensitive’ error the cause is due to the fact that netlify is a case sensitive system and the language you are using may not be. In that case, go back and check the consistency of your code in regards to upper and lower case letters. You will have to remove the file and then add it again. 
If this information doesn’t get the desired results, retrace your steps to determine what you were trying to do at the point in your project when you got the error, what error you got, and exactly what is happening. 



#### (optional/bonus) Can you set up a redirect from “/netlify/anything” to https://www.google.com/search?q=anything ?

In JavaScript these three lines would execute the redirect correctly:

things = location.pathname.split('/');
    anything = things[things.length-1];
    location.replace("https://www.google.com/search?q=" + anything);	



#### (optional/bonus) Could you give us a suggestion to improve this test or the job posting?

The previous question is confusing because it is unclear if you are asking for a redirect from one specific ‘anything’ to another specific ‘anything’ , ie. a hard coded path, or to a general ‘anything’, ie. a variable path.  








