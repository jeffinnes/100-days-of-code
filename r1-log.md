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
- Make personal site Mobile friendly
- Make the blog on my personal site actually readable  :white_check_mark:
- Finish the prorated cost calculator app I started so, so long ago...
- Build a CLI to manage my Digital Ocean firewall settings (to start)
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
