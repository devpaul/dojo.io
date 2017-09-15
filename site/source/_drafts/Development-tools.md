---
title: Development Tools
authorId: pshannon
---

Engineers want three things. They want to be able to deliver great software as quickly as possible with confidence. 
Doing this goes beyond simply selecting the right framework. It requires you to set up and become comfortable with
your development environment and knowing what solutions your tools provide.

Selecting your tools begins by understanding your project and development workflow. The project workflow is the 
process that takes a piece of software from conception through deployment. It typically looks something like this

* Conception
* Design
* Breakdown & Estimation
* Setup
* Development
* Test
* Deployment
* Support

Typically these project phases occur asynchronously throughout the life of the project. Very agile teams may be able
to take a new feature from conception to deployment very quickly while other teams may have bottlenecks or business
reasons that slow down this process.

As engineers our workflow is dominated by the development phase of a project. Therefore it is important that we
select tools that help us avoid unnecessary bottlenecks and conquer the steps in development. The first of these
is steps involves development itself and [setting up a development environment](http://dojo.io/TODO) and an IDE.
Next is selecting tools that will help build your project and produce an artifact that will eventually be deployed
to your customers. These tools are your frameworks, packages, and compilers that help you quickly build software
using good patterns. Testing and debugging tools imbibe your code with quality and confidence that help ensure that
code will behave how it is expected. Finally we'll want tools that help integrate code and features together as
well as tools that help decouple our processes from others to avoid bottlenecks so we can deliver quickly.

## Build Tools

Dojo 2 comes with most of the tools you need to build right out of the box. The excellent 
[dojo cli](https://github.com/dojo/cli) comes with [Webpack](https://webpack.js.org/) for bundling code, 
[Intern](https://theintern.io/) for automated testing, [tslint](https://palantir.github.io/tslint/) for enforcing 
common styling making code easier to read.

For those unfamiliar with Webpack, it is a code bundler that is capable of building and bundling an entire project
together including assets and dependencies. It is different from the previous generation of bundlers like the
[dojo builder](https://dojotoolkit.org/documentation/tutorials/1.10/build/) because of its extensible build process.

Dojo's cli extends Webpack as part of its build process. When `dojo build` is used your project is scanned for an
entry point where TypeScript can begin compiling your application. 

* Dojo-cli
* webpack
* postcss
* TypeScript
* grunt (gulp)
* @types

## Testing

* code styling (tslint)
* intern
    * unit testing
    * functional testing
    * benchmarking
    * plugins
        * a11y
        * visual regression

## Debugging Tools

* source maps

## Development Server

* webserv

## Continuous Integration

* TravisCI
* Appveyor