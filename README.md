Indy.rb March Meetup Live Notes
--------------------------------

### Presentations

- RSpec and Selenium integration - Dave Christiansen
- Javascript - Dave Strus
- Teaching Ruby as a first language - Robby Slaughter  
  

#### Teaching Ruby as a First Language  
*by Robby Slaughter*  


##### Biggest Problem  

We don't know where students are coming from, and where they are going.  


##### Why Ruby?  

* No one knows it
* Students dno't automatically slack off
* Clean syntax
* Fully OO
* Constructs lend to diagramming and discussion  
  

##### How are we doing it?  

* Assign a one-month workshop with daily tasks.
* Use variety of online tutorials.
* Provide support, not instruction.
* Require completion; expect drop-outs.  
  

##### Student Question War Stories  

(Various code blunders presented.)  

##### What's Next?  

Almost nobody is teaching Ruby at the University level.  
Basically nobody is teaching it as a first language.  

Ruby is good for teaching:  

* Web development
* OO design
* Testing / TDD
* ...  
  

#### Javascript + Rails  
*by Davey Strus*  

We use a ton of javascript at nFrame.  We needed a way to load certain javascript files for certain views.  Davey wrote a function (OK, several functions) that will effectively 'require' javascript files in other javascript files.  It's... involved.

* Require a few javascript files everywhere
* Load a javascript file based on the controller name
* Auto-run a function based on the view  

JavascriptAutoInclude: http://github.com/kernow  

Sprockets (by 37signals): http://getsprockets.org  

(more links to come!)  

#### RSpec & Selenium  
*by Dave Christiansen*  

For TriSano, Dave needed automated integration tests that drive the browser (on their Continuous Integration server).  

Selenium's IDE can be used to create tests that drive the browser.  This alone is difficult to automate.  Dave wrote some code to allow you to export the Selenium tests to RSpec.  This quickly led to abondoning the Selenium IDE, and writing a lot of helper methods, allowing them to reuse the tests they write frequently.  

Dave abandoned the Selenium grid, and essentially wrote his own.  In the future, Dave is looking at refactoring the TriSano integration system to have a more expressive API, favor XPath over DOM ids only, and integrate Cucumber.  


Sponsors
========
Thanks to [Engine Yard](http://engineyard.com) and [New Relic](http://newrelic.com/) for sponsoring the March Meetup!

About EngineYard
-----------------
> We focus on deployment and operations support, so you can focus on developing your business. Start while in development and scale your user base without stress along the way. Engine Yard supports the Ruby community by sponsoring the development of Rails, Merb, Rubinius and other open source projects. We're here 24/7, by phone, at (866) 518-YARD or email, at info@engineyard.com.

About New Relic
---------------------------
> New Relic RPM is a Ruby on Rails Performance Management solution that enables developers to quickly and cost effectively detect, diagnose, and fix application performance problems in real time. www.NewRelic.com
