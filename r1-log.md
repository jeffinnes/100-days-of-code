# #100DaysOfCode Log - Round 1 - Jeff Innes

The log of my #100DaysOfCode challenge. Started on August 2nd, 2020.

## Goals
- Learn CSS Grid
- Get comfortable using Promises
- Get comfortable with Async/Await
- Actually understand how to use 'this' and build classes
- Get more comfortable using APIs

## Planned projects
- Refactor my personal site to use CSS Grid (probably in addition to Flexbox)
- Make the blog on my personal site actually readable  :white_check_mark:
- Finish the prorated cost calculator app I started so, so long ago...
- Build a CLI to manage my Digital Ocean firewall settings (to start)
- Participate in [Hacktoberfest 2020](https://hacktoberfest.digitalocean.com/)
- *I'll add more projects as I think of them. I've been using the creation of this list to procrastinate starting the challenge...no more!*

## Log

### R1D1 
Worked on the readability of my blog. Mostly this involved tweaking some CSS rules.
I really wanted the date for the blog posts to show up as "X years X months X days ago" instead of just the raw timestamp from the DB. I played around with doing this in plain JS but ultimately decided to use Moment.js and its *duration* object.

### R1D2
Working on adding an "edit post" function to the blog. Got stuck for a bit because I forgot that Handlebars automatically drills down the variable scope when you use the 'each' helper. Link to edit now correctly prefills the form fields with the posts but the actual editing is thowing an error... for now.

### R1D3
It's amazing what fresh eyes see. The error yesterday was being thrown because I forgot to declare an object but was trying to add properties to it. Easy fix
Worked on Prorated Cost calculator. Started converting to CSS grid to try and control the layout better.
