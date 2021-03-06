[![Dependency Status](https://www.versioneye.com/user/projects/57673e8c276f0f0052974a19/badge.svg?style=flat)](https://www.versioneye.com/user/projects/57673e8c276f0f0052974a19)    [![Codewake](https://www.codewake.com/badges/codewake.svg)](https://www.codewake.com/p/lucee-5-application-template-for-heroku)

# Lucee 5 Application Template for Heroku

Blank application template to deploy [Lucee 5](http://lucee.org) apps on Heroku

---

Find this project useful? [Show some love :revolving_hearts:](https://www.creatorlove.com/mikesprague/lucee-5-heroku-buildpack) and buy me a cup of cofee! :coffee:

---

[![Deploy](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)

Demo: [https://lucee5.herokuapp.com](https://lucee5.herokuapp.com) | [https://lucee5.herokuapp.com/test.cfm](https://lucee5.herokuapp.com/test.cfm)

## Credits/Notes:

- This project is based off of the offical Lucee Heroku Buildpack

## Requirements

- [Maven](http://maven.apache.org/) to build the project
- [Foreman](https://github.com/ddollar/foreman) to run locally

## Instructions

To get started, run the following commands in GitBash (or your terminal of preference):

```bash
$ git clone https://github.com/mikesprague/lucee5-heroku.git
$ cd lucee5-heroku
$ mvn package
$ foreman start
```

NOTE: On Windows, start foreman with the following command:

```bash
$ foreman start -f Procfile.dev
```

You should now have Lucee up and running at <http://localhost:5000>. Start adding your code.

To deploy your site to Heroku you need to setup a free Heroku account, install the Heroku toolbelt (Suggested reading: [Getting Started with Java on Heroku](https://devcenter.heroku.com/articles/getting-started-with-java)). Then...

```bash
$ heroku apps:create [NAME]
$ git push heroku master
$ heroku open
```

You should now be looking at your app running on Heroku.

NOTE: If you get a Heroku application error try reloading the page. This is a known issue. I think the Lucee dependencies aren't quite ready when this happens, I need to look into it further.

Enjoy!
