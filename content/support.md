---
title: "Support"
date: 2018-06-26
anchor: "support"
weight: 
---
## Favorite Support activities

Many of the activities on your list interest me. It's difficult for me to select the top five, but here they are:

* Respond to 50+ support requests via email or chat most days
* Receive occasional phone calls requesting support from our highest-value customers
* Find and recruit teammates for the Support team
* Deliver a talk to many people you don't know at a conference or meetup
* Debug a customer's build using a programming language and framework that you've never seen before

## Least favorite Support activities

It was difficult for me to select five activities, so I selected two:

* Create video tutorials to help teach users a specific feature or use case
* Help manage communications during a service outage

## Favorite part of Support

I enjoy working with a customer to solve a difficult technical problem. This yields two outcomes: the satisfaction of solving the problem and the relationship that is built with the customer in working with them to solve the problem.

## Netlify service

Overall, my experience using Netlify was smooth. The documentation is well written and the GUI provides a good user experience. The speed of the deployment process and the quick reponse time accessing the deployed web site are impressive.

**Suggestion:**

* The quickest way to get started appears to be to deploy a pre-built template. Maybe this should be mentioned at the top of the Welcome page.

**Issue found:**
On the "JAMstack templates" page, when I select "Deploy to Netlify", I get the error: "You must specify a provider when calling netlify.authenticate". I cannot specify the provider anywhere. I tried multiple templates. I worked around this by creating a new Hugo site on my local file system and then copying the files from one of the Hugo templates (I describe this in the next section).

## Web site building process

I chose Hugo as my static site generator. It's one of the most popular generators and has a lot of pre-built templates to choose from. Using Hugo's command line interface, I created a new site. Then I downloaded a prebuilt template and tweaked the config.toml file, created the content and tested the site locally on my machine. Following that, I pushed my Hugo site to Github and created a new site in Netlify and pointed it to the Github repository. 

After deploying this site to Netlify, the styling on the page did not render correctly. I verfied in the Netlify logs that there were no deploy errors and checked the "Build Gotchas" in the documentation. I also tried adding a git submodule for the theme, instead of cloning it, but that didn't resolve the issue. As an alternative, I chose a different theme and went through the same process I described in the previous paragraph. It's working now.

## Developer-focused product

Stripe's developer documentation site (https://stripe.com/docs/api#intro) is well done. It provides good tutorials and reference material. The tabs on the right side organize the example source code for the client libraries. The site's content is well-written and avoids complicated payments terminology.

## Importance of SSL/HTTPS

Your page https://www.netlify.com/docs/ssl/ provides many good reasons to use SSL/HTTPS. Three of them are: Better site performance with HTTP/2, available site analytics from referrers that support HTTPS and encryption of login and form submission pages.

## DNS

Non-technical users may find DNS concepts confusing. These users may not be aware of the difference between a domain registrar and a web site hosting provider. They need to know how to configure the DNS records at the registrar to point to the web hosting server.

Users may encounter challenges when configuring DNS. The first is figuring out which DNS records to configure. There are A records, CNAME records and MX records and other record types as well. The second is that after configuring the DNS, users may expect their changes to take effect immediately. But the changes can take up to 24 hours to propogate across all of the DNS servers on the Internet.

## Customer issue: "Site won't build"

Hello Customer,

Thanks for contacting Netlify Support. As I understand, your site build is failing in Netlify. As a first step, please ensure that your build succeeds in your local environment. Once it does, verify that the package versions Netlify uses match yours. You can check this here: https://www.netlify.com/docs/build-settings/

If these package versions match, and you want to troubleshoot the issue further on your own, visit this page: https://www.netlify.com/docs/build-gotchas/

If you'd like more help, please provide me with a log of your failed build. To find this, go to the "Deploys" tab, click on the failed deploy, and click on "Click on Clipboard", and then paste the contents into the Support ticket.

Thanks,

Scott

# Redirect to google
This works. I created a \_redirects file and placed it in the static folder.

# Job post feedback

I like the emphasis on Support values and that the technical requirements are not strict. 

# Activity feedback

This activity has a good mix of technical and non-technical questions. I especially like the question about the site won't build, as customers will sometimes open a support issue without providing many details.
