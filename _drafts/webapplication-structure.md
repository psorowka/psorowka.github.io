---
layout: post
title: The web-application dilemma
category : web
tagline: ""
tags : []
---

Dilemma:

 - Often one Application for both data-interface (API) and webfrontend
 - Frameworks like rails encourage those structures
 - few information on how to structure code in a good manner
 - rails best practice to split controllers, but how to keep Business Logic DRY?

Solution Suggestion: 

 - strict SRP - also for Controllers
 - all shares same models
 - look at webfrontend as an API-Client
 - split controllers, but use class inherition for business logic
 - split structure into validation (e.g. models, service classes, business logic) and presentation (e.g. API controller -> repsond with JSON and Webfrontend-controller, user frontend)
 - keep things DRY!
 - API Design first
