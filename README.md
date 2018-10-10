* [The mission](#the-mission)
* [Site documentation](#gwt-documentation)


# The mission

This is an initiative to update the GWT site and enrich with new content, the goal is to update the current content and to add content that refers to the new libs/frameworks related to GWT.

Also make the site a good place for starters, by adding tutorials, demo, and tools that help them start using GWT with minimum efforts.

> this is an opinionated project - the goal here is not to get new opinions on what the docs should look like, but to break up many small segments of work to see if we can end up with a better overall project

## Improvements outlines

### The home page has four main links :

- #### Overview

	- The overview seems to be ok needs some update. maybe the list of the apps built with GWT.

  - Why should I use GWT.

  
- #### Download

	Maybe we need to set the maven/gradle dependencies here.
  also if we build a CLI tool here we might add here maybe, also might provide it with sdkman.

- #### Getting started
	this needs most of the work.

	- This still uses ANT, so we need to use MAVEN at least here (or Gradle).

  - uses OLD devmode so might change to super devmode.

  - Create a simple CLI to get started with GWT.

  - Make use of the mvp4g web project generator.

	- Introduction to use GwtBoot starters.

- #### Docs

  - Split the tutorials from the documentation maybe add them on the home page.

  - Add tutorial for each section in the documentation maybe at the end of each section.

  - Add tutorials for new GWT libs and frameworks provided by the lib/framework author.

  - Rest is common, so maybe introduce a rest tutorial with different rest clients.

  - Introducing the new RPC from Colin.

  - Tutorials for building GWT apps with different back-end techs spring-boot, vertx ..etc

  - Tutorials for JsInterop and how to interact with other JS Libs.

  - Remove old / deprecated stuff

**In the home page we can introduce the following new topics:**

- Community

  - Listing GWT libs and frameworks (good collection at https://gwt.zeef.com/awesomegwt )
  - Built with GWT.


- J2CL / GWT 3
  - GWT 3.0 progress
  - Writing Apps for GWT 3.0
  - GWT 3.0 vs. GWT 2
  - Help get GWT 3.0 out.


- Tutorials - moved out from docs

  - List all tutorials.


- News, Blogs and Article - moved out


- Social Media
  - Twitter account.
  - Face book account
  - Be more active on Linked-in, G+


# GWT Documentation

* GWT documentation is published under http://www.gwtproject.org/doc/latest/DevGuide.html

## Reference

* Markdown processor: https://github.com/sirthias/pegdown

## Adding content

* See: http://www.gwtproject.org/makinggwtbetter.html#webpage

## Building

If you have Grunt installed :
* build the assets using Grunt: `grunt`
* then run: `mvn clean install`
* after that you will find the generated documentation in `target/generated-site/`.

If you don't have Grunt installer :
* build the assets using Maven and Grunt plugin: `mvn clean install -Pgrunt`
* after that you will find the generated documentation in `target/generated-site/`.

### Running locally
Run the site locally for easy visual testing

* Change to the `target/generated-site` folder.
* Open the `index.html` file in your browser.
* Additionally, you could run any local HTTP server in this folder.

