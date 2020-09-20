# #100DaysOfCode Log - Round 1 - Jeff Innes

The log of my #100DaysOfCode challenge. Started on August 2nd, 2020.

## Goals
- Learn CSS Grid
- Practice Responsive CSS
- Get comfortable using Promises
- Get comfortable with Async/Await
- Actually understand how to use 'this' and build classes
- Get more comfortable using APIs

## Planned projects
- Refactor my personal site to use CSS Grid (probably in addition to Flexbox) :white_check_mark:
- Make personal site Mobile friendly :white_check_mark:
- Make the blog on my personal site actually readable  :white_check_mark:
- Finish the prorated cost calculator app I started so, so long ago... :white_check_mark:
- Build a CLI to manage my Digital Ocean firewall settings (to start)
- Crowdsourced advice rating app
- Build super secret project (not ready to reveal this idea yet)
- Participate in [Hacktoberfest 2020](https://hacktoberfest.digitalocean.com/)
- Build something in [Rockstar](https://codewithrockstar.com/)
- *I'll add more projects as I think of them. I've been using the creation of this list to procrastinate starting the challenge...no more!*

## Log

### R1D1 
Worked on the readability of my blog. Mostly this involved tweaking some CSS rules.
I really wanted the date for the blog posts to show up as "X years X months X days ago" instead of just the raw timestamp from the DB. I played around with doing this in plain JS but ultimately decided to use Moment.js and its *duration* object.

### R1D2
Working on adding an "edit post" function to the blog. Got stuck for a bit because I forgot that Handlebars automatically drills down the variable scope when you use the 'each' helper. Link to edit now correctly prefills the form fields with the posts but the actual editing is thowing an error... for now.

### R1D3
It's amazing what fresh eyes see. The error yesterday was being thrown because I forgot to declare an object but was trying to add properties to it. Easy fix.
Worked on Prorated Cost calculator. Fixed an issue where the start date was not getting populated because JS Dates are not zero filled but the Input elements "value" property required it. Started converting to CSS grid to try and control the layout better.

### R1D4
Finished converting the Prorated Cost calculator to CSS Grid. Integrated the app into my portfolio site so it can be used/demoed. A number of style rules had to be modified or removed due to conflicting CSS rules. I wasn't too surprised because I started the calculator a long time before I had even decided to build a portfolio site. Maybe I should set up a repo template based off the portfolio site for projects where I want the code base publicly viewable... :thinking:

### R1D5
Spent some time today finishing up a CSS Grid course on Pluralsight and reading up on Grid. Started the refactor process on my portfolio site. So far I really like Grid. More refactoring tomorrow!

### R1D6
More CSS Grid refactoring. The home/about page is done, and I decided to combine the "contact" page into the about page. I'm not totally happy with the color scheme, but I'll come back to it sometime after I refactor the remaining pages to Grid.

### R1D7
One week down! I got distracted from the CSS Grid refactor with replacing as many "divs" as I could with more semantic tags. I managed to get the projects page refactored even though I went down the rabbit hole of semantic HTML.

### R1D8
Wrapped up the CSS Grid rework of my portfolio site. I also ended up combining some content that was previously on separate pages. Next up is making the whole site Mobile friendly because right now it is basically unusable on a phone!

### R1D9
Little bit of a rough start making the portfolio site mobile friendly. Everything I build for work is used on screens 1000px & up, haven't had much chance to flex this muscle; I'm definitely feeling a bit rusty. On top of that, Chrome's dev tool screen simulator wasn't triggering the media selectors and it took me a bit to figure out that my code wasn't the issue. Yet another reminder of how much it sucks that Mozilla axed the entire FireFox dev tools team.

### R1D10
Fiddle fiddle fiddle. That's the name of the responsive CSS game. I got really close tonight, just one last element is being difficult. I suspect it will require a small adjustment to the HTML so I can use grid or flex to controll the wrapping behavior, but I'll take a look tomorrow with fresh eyes.

### R1D11
Finally got all the mobile styles looking how I wanted. Pushed code to production... and nothing. It was all working in the browser simulation, but on mobile nothing changed. After some research, I found out that I needed to include a "Viewport" meta tag in the Head of my HTML file. I must have learned about that at somepoint, but I sure didn't remember it now. Anywho, after adding `<meta name="viewport" content="width=device-width, initial-scale=1">` to the Head, everything is happy on mobile.

### R1D12
I decided the next project I want to tackle is building a CLI to manage the firewall on my Digital Ocean account. I ended spending most of my time reading about ways to build a CLI but I did get the repo and basic files in place. I'll start actually coding it tomorrow.

### R1D13
I lied. I didn't really start coding the CLI project today. I had to do some after hours server updates for work and was just too tired to trust any code I write. Instead I spent time checking out some of the packages various tools recommended. Commander.js and Inquirer.js look like they will provide the functionality I'm looking for but I'm not quite sure what to do about cred storage yet.

### R1D14
Two weeks down! Feeling good about it for sure. Made some progress on the Digital Ocean CLI project. Commander.js is starting to make more sense, it just took staring at the docs long enough to realized that the option flags automagically create the property with a matching camel-cased name. Now it can read, store, or delete the API token.

### R1D15
Got sidetracked from the CLI project. The prorate calculator was getting lonely on my projects page. Started porting a dog counter project I made to experiment with Electron a while back. As of writing this, I don't really understand the process to build Electron into an installer. I had used Electron-Forge, but then they did a major version change and I didn't understand how to use it...

### R1D16
Finished porting the dog counter project and updating the styling to be responsive. Something that has been frustrating is that mobile views were zooming in on input fields but I didn't want that. Today I learned that if the input field's font-size is smaller that 16px most phones will zoom in. Easy enough to fix. I also spent some time reading the Digital Ocean API docs and made a few test calls with Postman.

### R1D17
Worked on the CLI some more. Tonight I got the commands to pull a list of firewalls and displaying them working. I feel like I'm really starting to get Commander and Inquirer. 

### R1D17
More CLI work. I spent a bunch of time trying to implement a recursive function call to reprompt the previous question in situations where the user only requested a display of info. In the process I overly complicated things by trying to turn everything into an async function. (I guess I'm just really excited to finally starting to feel like I get promises and async/await. Anyway, I ended up abandoning that line of thought because it was preventing me from getting any actual functionality done. After switching gears I finished the logic to select a firewall and nicely display it's info.
