Karun Narayan 912828354
add name here and student ID

In order to compile, cd into proper directory with java files. Before you compile and run the server you should set up the internet browser. In firefox go to preferences or settings and then go to network settings. Click settings. Click the the manual proxy configuration. In http proxy type in "localhost" and in the port put "8080". Now your browser is gonna use the java proxy. Now you should clear cache and delete history in your browser. Then run "javac -deprecation *.java". This command compiles and then use 
"java ProxyCache 8080" to run the proxy server.

To test the proxy I used the given example website, "http://gaia.cs.umass.edu/". When i put this into the browser I could link different links on the page. But eventually some links take me to a https website and the proxy fails there. Also if I try to open a new tab and enter a random http website like "http://pngbirds.myspecies.info" the program crashes. Everytime you want to enter a new website into the search bar you have to clear cache and history and restart browser. I tested out different websites from "http://scratchpads.eu/explore/sites-list", this website gives me a bunch of http website to test it out on. Again when testing a specific website from here, I go down a rabbit hole of links and the proxy crashes once I enter a https link. This is expected behavior. If I am on one website and decide to switch to an entirely different one by entering it in the adress bar, the proxy fails.

We have a proxy that works when you enter a http website with only http links. Once you hit a https link, the proxy will crash as expected.
