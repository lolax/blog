---
title: I - Negotiation & Initialization
date: '2019-01-11'
---

## Part 1 - Individual Contributions

### Contribution Graph

https://github.com/Lambda-School-Labs/labs9-map-scratcher/graphs/contributors
My handle is @lolax

### Summary

While I have more pull requests for front end, my work this week was fairly balanced between front end and back end. As a team, our efforts for the first half of the week were dedicated to planning and negotiating strategy; those efforts are not reflected in trello cards or PRs, but they were no less integral. My back end PR was a combined effort with several other members of my team. It represents the first steps we took to establish a foundation for the new technologies we chose to work with. My front end contributions consisted of refining our map component, adding preferences for the prettier extension to assist in standardizing our formatting, and expanding the map page component to reflect the basic elements in the wireframe for that page with some light styling for layout. 
	
### Tasks Pulled

**Front End**
	Leaflet Implementation Fix
        https://github.com/Lambda-School-Labs/labs9-map-scratcher/pull/20
        https://trello.com/c/9vBDgZQT/23-set-up-leaflet-component
    Expand Map Page Component
        https://github.com/Lambda-School-Labs/labs9-map-scratcher/pull/23
        https://trello.com/c/ThVkSaJC/33-map-page-component
    Add Prettier Preferences
        https://github.com/Lambda-School-Labs/labs9-map-scratcher/pull/22
        https://trello.com/c/OOA4Xsgh/28-add-prettierrc
**Back End**
    Prisma Setup & Deployment
        https://github.com/Lambda-School-Labs/labs9-map-scratcher/pull/9
        https://trello.com/c/CEFwFKVa/12-deployed-to-the-web

### Detailed Analysis

The pull request I made this week that I feel most deserves a detailed analysis is the one for prisma setup and development because it was the culmination of almost an enitre day's work for me, Kyran, and Jacob. We were all completely new to Prisma, meaning that initializing the Prisma environment required substantial reliance on the documentation and an introductory tutorial. Adhering to these references and through some trial and error, we were able to set up our file structure for the backend. 

![Prisma file structure](https://www.datocms-assets.com/9114/1547228397-screen-shot-2019-01-11-at-12-14-33-pm.png)


Included in the setup process was adding the proper dependencies to index.js and bringing in typedefs,resolvers, and a Prisma concept called "context" for the GraphQL server.

![Dependencies and GraphQL server](https://www.datocms-assets.com/9114/1547228366-screen-shot-2019-01-11-at-12-39-08-pm.png)

Next, we wrote several queries, mutations, and typedefs for the basic schema of our data. After testing a basic user type to acclimate to the syntax and patterns, we wrote types for users, countries, and visits (which reprepresent the intersection between a user and a country). 

![Typedefs](https://www.datocms-assets.com/9114/1547228316-screen-shot-2019-01-11-at-12-38-07-pm.png)

Our queries, mutations, and schema were then tested and improved using the Prisma playground. Interpretting the error messages provided by the playground was challenging at first, but our understanding became increasingly clearer with practice.

We used Prisma commands in the terminal and their web app to create a Service, which relies on a server deployed to Heroku and a Postgres database. Note that the Prisma GUI displays these as "Not Reachable" but we are able to reach them so we believe this is an error on Prisma's part.

![Server and database](https://www.datocms-assets.com/9114/1547229227-screen-shot-2019-01-11-at-12-51-39-pm.png)


## Part 2 - Milestone Reflections

Our experience forming a team has been far more involved than I imagined. I deeply enjoy working with each person on my team, which perhaps obscured the possibility that each would not necessarily work well with each other person. This week was particularly strenuous because on day one we needed to finalize many serious decisions prior to establishing consistent group dynamics or guidelines. The diversity of personalities and strengths and interests on our team is wonderful for writing code, but made discussions and negotiations more difficult. To help our team dynamic, I consistently made a concerted effort to understand what each other person was saying. During conflict-resolution discussions, I tried to contribute ideas and offer verbal support for the ideas of others to fortify them, especially when it seemed like they weren't necessarily being heard. When it seemed like a conversation was becoming circular or unproductive or other tasks needed to be prioritized, I spoke up to suggest redirection. In retrospect, there are a few things I wish I'd done differently. To begin with, I wish I had researched our stack when it was originally proposed so that my input could have been better informed. Additionally, I regret letting stress and challenges bring out negativity in my attitude. It's easy to commiserate, but it is far more useful to meet another person's misery with support.
