# kevlu8 SMP
kevlu8's Minecraft SMP server!

# Why open source?

Well, I wanted viewers to be able to download the map if they wanted to without spending way too long on trying to build it themselves.

# Why am I here?

That's a really good question.

# How much time did you spend on making this (github repo)?

Ehhhh... maybe 2-3 hours

# Can I clone this?

Sure! You can run `git clone https://github.com/kevlu8/kevlu8smp.git` and get the repo on your local pc. As an alternative you can also fork it.

# How do I make my own server?

Fork this repo (or clone then commit and push if you want) then make an ngrok account. Then you need to go to kevlu8smp/.ngrok2/ngrok.yml and change the authtoken to your own which should be displayed as soon as you register (and verify your email).
After that you will need to go to heroku and create a new app. You can name this app whatever you want. I named it kevlu8smp because it's easier to remember. Now you will need to attatch your github repo to the heroku app (there is a button to do so).
Once you finish that, click deploy and wait for it to load. After it finishes, reload the page then go to the `Resources` tab. There will be some dynos. Switch the top one off and the bottom one on, then go to logs (not the deploy logs, the entire application's logs). Once you see `Updated db` or something along that, go back to resources, and switch the top one on and the bottom one off. Go back to logs, and once you see something along the lines of "Starting ngrok tcp", reload ngrok and go to "Tunnels", and you will see an IP address. That is the IP of your server! Just remove the tcp:// and you're good to go.

# **WARNING: THIS SERVER WILL CRASH A LOT AND WILL OCCASIONALLY SPIKE IN LAG DUE TO 1) MINECRAFT SAVING THE WORLD OR 2) THE HEROKU APP GOING TO SLEEP. THERE IS NO WAY TO PREVENT THIS AND EVERY TIME YOU GET DISCONNECTED YOU'LL NEED TO REDEPLOY THE APP** 
