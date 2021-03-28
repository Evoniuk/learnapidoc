---
title: API product overview
permalink: /docapis_doc_overview.html
keywords:
course: "Documenting REST APIs"
weight: 6.1
sidebar: docapis
section: docconceptual
path1: /docconceptual.html
last-modified: 2021-02-03
---

The product overview (usually the homepage of your product's documentation) explains what you can do with the product, including the high-level business goals, the market needs or pain points it solves, who the product or other features are for, and other introductory information.

Although a seemingly simple page, the product overview can overlap into marketing domains, create redundancies with README's, and pose challenges in connecting with a more diverse audience (both engineers and bizdev people) than the rest of your technical docs. Overall, the product overview is an area where documentation and marketing intersect in interesting ways.

{% if site.format == "web" %}
* TOC
{:toc}
{% endif %}

## Purpose of the product overview

Too often with developer documentation, the documentation gets quickly mired in technical details without ever explaining clearly what the product is used for. Don't lose sight of the overall purpose and business goals of your API by getting lost in the endpoints.

The product overview grounds users with a high-level understanding of the system. This high-level understanding is critical for users to grasp the system as a whole. It allows the details to fit into a broader conceptual framework. As users attempt to understand your product, they often start at this high-level, getting a gist of the shape of something as a whole before proceeding into more details.

For example, when you walk into a new store, do you gaze around a bit to take in the layout and size of the store first, or do you immediately look at the products on the aisle shelves? For me, I do the former. This is how many of our brains work &mdash; we start with the big picture (the forest) before diving into the details (trees and leaves). I elaborated more on this in [Reduction, layering, and distillation as a strategy for simplicity](/simplifying-complexity/reduction-layering-distillation.html). The product overview provides this initial orientation for the user with your product. Don't jump immediately into the fine-grained details of technical how-to without telling the larger story first.

## Key questions a product overview should answer

A product overview should address some basic who/what/why/how/when type questions:

* What is this product?
* What does it do? What problem does it solve?
* Who is it for? Who is the intended audience?
* Why would someone use this? What are some common use cases?

{% include course_image.html size="medium" border="true" filename="nonref_overview" ext_print="png" ext_web="svg" alt="product overview" caption="The product overview provides high-level detail about the purpose, audience, and market need for your API." %}

Keep in mind that there are thousands of APIs. If people are browsing your API, their first and most pressing question is, what information does it provide? Is this information relevant and useful to my needs? How does it differ from other products in this same space? The user's first question is usually not "How do I configure this endpoint."

## Telling your product's story

To tell your product's story, consider identifying a market need that your product solves. This is the basics of storytelling &mdash; there is some conflict that a protagonist (in this case, your product) addresses and solves. In [The Top 20 Reasons Startups Fail](https://www.cbinsights.com/research/startup-failure-reasons-top/), one of the main reasons startups fail is their inability to solve a market problem. The authors explain:

> Startups fail when they are not solving a market problem. We were not solving a large enough problem that we could universally serve with a scalable solution. We had great technology, great data on shopping behavior, great reputation as a thought leader, great expertise, great advisors, etc, but what we didn’t have was technology or business model that solved a pain point in a scalable way. (*CB Insights*)

To encapsulate this overarching story, the product overview focuses on the market problem that the product solves. If the product doesn't solve a market problem, that could be a red flag about the product itself. Although you're likely just writing the documentation (not doing corporate storytelling), it helps to understand this larger problem as it gives more context for your product.

## Common use cases

To make the product's market-solving characteristics more concrete, list some common use cases or business scenarios in which the product and API might be useful. These scenarios will give users the context they need to evaluate whether the API is relevant to their needs. Too often, product descriptions are general and high-level (e.g., "X product helps companies collaborate more effectively..."). These higher-level abstract descriptions fail to resonate with users.

{% include random_ad4.html %}

Use cases are concrete examples of how the product might be used. Continuing with the above example, a use case might be "X product allows writers to work on the same document simultaneously through a remote browser interface," or something. Usually, a product manager has already defined a list of key use cases for a product and would have these available.

## Product overview vs overviews (plural)

A developer portal usually has documentation for many different products, not just one. Each product will have its own product overview page. In fact, the homepage of the developer portal rarely has a product overview. Instead, the developer portal's homepage often serves as a routing board to the product overviews and other developer journeys.

Even a single product might have multiple product overviews for each of the features. The overview is just a term for the opening page of a product, the landing page or starting page. Whenever you need a high-level description of your product, you need a product overview page.

## Audience includes decision-makers

One important dimension to keep in mind with product overviews is the expanded audience. Product overviews aren't just read by your target documentation users, i.e., usually engineers. Product overviews are frequently read by product managers, executives, and other decision-makers who are trying to decide whether to purchase or move forward with the product. These decision-makers might be trying to size up the complexity of integration, how many person-hours the effort will consume, and whether the product will solve the problem they have. Only documentation can truly answer this question, not marketing material.

For example, a high-level executive might be trying to decide if implementing your product will require one-week integration effort by a single developer or a team of 50 developers working heads-down for six months. The product overview should give some indication of the development effort. Even if you don't call out the estimated development time, by browsing through the tasks in the docs, it should become clear what level of effort is involved in implementing the product.

In the overview, the high-level executive will be less interested in the technical details and more interested in conceptual and bigger picture content. List out the main components involved in the system, followed by an architectural diagram and an explanation. Save the excruciating technical details for the inner pages of the documentation.

## Overlap with marketing

Another facet of product overview pages is their frequent overlap with marketing content. In many organizations, there is a developer marketing group that handles product overviews which also cover this more high-level overview of the product. For example, if you browse the AWS Lambda documentation, you'll find that a higher-level product overview appears before the actual documentation. Here's the [marketing layer](https://aws.amazon.com/lambda/) to the product:

<a class='noCrossRef' href="https://aws.amazon.com/lambda/"><img style="border: 1px solid #dedede" src="https://s3.us-west-1.wasabisys.com/idbwmedia.com/images/api/awslambdaproducthomepage.png" alt="AWS Lambda product homepage" /></a>

This marketing layer covers these topics: Overview, Features, Pricing, Getting Started, Resources, FAQs, and Partners. The actual [Lambda documentation](https://docs.aws.amazon.com/lambda/latest/dg/welcome.html) is presented on another layer of the site:

<a class='noCrossRef'  href="https://docs.aws.amazon.com/lambda/latest/dg/welcome.html"><img style="border: 1px solid #dedede"  src="https://s3.us-west-1.wasabisys.com/idbwmedia.com/images/api/awslambdadochomepage.png" alt="Lambda documentation homepage" /></a>

If you read the first paragraph from each screenshot, you'll see how similar yet different the two descriptions are. They repeat many of the same points but in different ways. The documentation product overview addresses these questions:

* When should I use AWS Lambda?
* Are you a first-time user of AWS Lambda?

Beyond the product description, in this Lambda example, the marketing content even has its own [Getting Started](https://aws.amazon.com/lambda/getting-started/) page with tutorials, parallel to the documentation's [Getting started section](https://docs.aws.amazon.com/lambda/latest/dg/getting-started.html), which is more robust.

Typically, developer marketing teams write the marketing product overview, while developer documentation teams write the documentation product overview. But as you can see, this is an area where content overlaps and where some coordination across teams becomes essential. Suppose the doc team for Lambda wanted to emphasize certain points that the marketing team did not &mdash; it would create a confusing transition between the two sets of content.

But even with differences, the idea is that business decision-makers read the marketing content, while engineers read the documentation content. Marketers are primarily writing for these decision-makers while tech writers are primarily addressing the implementers (engineers).

Your organization might have multiple teams writing content like this, or you might be tasked with creating both the higher-level marketing layer and the documentation yourself (especially in startups). In some ways, having a single team or writer handle both types of content might lead to a more streamlined, unified content experience. When you're the sole writer, you're less likely to repeat yourself in different places in contradictory ways. You can simply devote a section of your documentation to the marketing content rather than housing it on another site.

If you are stuck with the two-site model (marketing on one site, docs on another), you could try to share content between these two sites, but usually marketing has a different system for managing and publishing content than the documentation teams. Marketers don't usually adopt docs-as-code systems but rather prefer more CMS-driven systems. These systems rarely share content with each other, and even if they did, the marketing versions might be written using another style, perspective, or approach that contrasts with your docs, making it difficult to single-source the content. For example, I once tried to re-use marketing content that was written entirely in third-person point of view ("the partner does X") rather than the traditional second-person point of view in docs ("you do X"). It didn't work out well.

{% include random_ad1.html %}

## Strategies for the documentation's product overview

What strategies should you implement when you're faced with writing a product overview for docs, especially when a product marketing team has their own product overview on a separate site? Consider the following:

* Find out who the marketing group is and what messaging they are focusing on for the product.
* If marketing content already exists and you want to leverage it (rather than just link to it), consider creating a condensed/streamlined version of the marketing overview content, and point users to the marketing overview for more details. You don't want to duplicate all the content because invariably, docs will go out of date as the other content evolves (not to mention the confusion of presenting two sets of overviews to users).
* Avoid copying any overblown promises about simplicity or ease of installation from marketing copy.

## Differences between marketing and documentation content

Here it's worth diving into some differences between documentation copy and marketing copy. While both genres might appear to share similar purposes in the product overview, avoid falling into marketing style in docs. For example, suppose you find a few pages of product descriptions that the marketing team already wrote, and you want to just copy it into the docs for the documentation product overview. Should you?

If you do this, strip out mention of the word "easy" or "just," as in "the implementation is so easy, you *just* have to do X...." To sell a product, marketing often gravitates toward promises about ease of implementation. This is perhaps the hallmark of marketing content (from a tech writer's perspective anyway). And many bizdevs or execs are trying to scope the difficulty of the implementation, so marketing's message about ease of implementation makes sense.

But as a technical writer, you not only have an obligation to be honest about implementation complexity, you must also recognize that what is easy for one user might be insurmountable to another. (If you've ever done DIY projects at home, you know what I'm talking about.)

Never say something is "easy" &mdash; instead, you might qualify the degree of development effort based on the role. For example, you could say that for a seasoned engineer familiar with Java and who has been developing cloud-based apps for years, implementing this product will likely not require more than a week of integration effort. But for someone new to cloud-based app development or less familiar with Java, there will be a much steeper learning curve and might require several months or more of preparation and learning to implement.

If you can qualify the level of development effort based on different audience types, this will provide more realistic information. You can still answer the exec's question &mdash; how difficult is this product to implement &mdash; without falling prey to promises of implementation ease.

By the way, it's worth noting that marketers often have a superficial technical understanding of a product, so they usually cannot make judgments about the implementation difficulty. They might be going off of an internal engineer's observation that it's "straightforward" or that it "should be easy to implement" or that "most engineers should find this familiar." What the marketer might not realize is that engineers usually make these estimations by assuming the audience has the same knowledge level and background as the engineer. Unfortunately, most marketers remain within the pre-sales context and so rarely see the post-sales realities, where many support cases and threads spring up with confused or frustrated users.

Beyond adjectives about easiness, in the previous Lambda examples, the marketing copy uses terms like "virtually any," "automatically," "precisely," and "favorite." These superlatives don't usually get used in documentation, which tends to be more factual and plain-speaking. Marketing tries to get users excited about a product by embracing these extreme adjectives, while documentation isn't overtly trying to sell or hype anything.

## Key differentiators in product overviews

As I've been arguing, the product overview space places you into murky territory where marketing and documentation blend. If you were to put on a marketing hat for a moment, what angle would you take in your writing (beyond language)?

Although it would be awesome to compare your product against competitor products, most likely your legal group will not allow it (mentioning competitors is usually taboo). And you might not have a deep understanding of other products to make a fair comparison. Or you might feel that readers will assume you're too biased and wouldn't trust your comparison anyway.

But what you can do is focus on your product's key differentiators. These are features your product has that make it unique in the market. For example, maybe users can access your app from the browser rather than installing it locally. You don't need to create a comparison chart showing how products X, Y, and Z lack online browser access. But by emphasizing this differentiating feature, you help establish a selling point and a potential reason for buying the product.

Remember that the product overview, unlike other documentation, often addresses a *pre-sales* scenario. As such, the reader is likely wondering how your product compares with other products in the same category. Why should they go with your product rather than another? What advantage does your product provide? Unless you know the competitive advantage of your product, you'll have a difficult time writing marketing-esque content in your product overview.

Then again, you might want to leave that topic alone entirely and just point users to marketing material. You will need to make a judgment call about where marketing ends and where documentation begins. If you do try to veer into the marketing domain, however, reading through competitive analysis docs from marketers could help inform your writing.

## Overlap with README's

Another challenge with product overviews is the overlap with README content. A README is an introductory overview file (a homepage) placed in a code repository such as GitHub. The README often has many elements of an overview similar to a product overview in documentation site. If your documentation references a code repo, that code repo needs a README. But do you duplicate the same information in the README that you do in the documentation overview?

Hopefully not. The README might have a high-level summary and information about installation, configuration, and usage. But this information should be much more condensed/abbreviated than more detailed documentation.

Many guides about writing README content assume that the README is the only documentation for the code in the repo. As a professional technical writer, I rarely work on projects that are so small that the documentation can be handled by a single page that lives in a code repo. If that's all you need for your product, great. However, chances are the README is only a glimpse of many more pages of configuration, installation, and usage detail that live in a more robust documentation site separate from the repo. If that's the case, you might want to just link to your docs in the README.

Although the README and product overview overlap a bit, the README has some elements that don't necessarily belong in regular documentation. Content elements specific to the README in the code repo might be the following:

* Code of conduct
* Contributor how-to protocol
* Filing issues
* Pull requests
* License information
* Team details/contributors

See [The Essential Sections for Better Documentation of Your README Project](https://www.welcometothejungle.com/en/articles/btc-readme-documentation-best-practices) by Thomas Parisot for a good guide about writing README content.

I admit that my preferences for the README might deviate from general recommendations from developers in this space. I am not a fan of duplicating the same information from the documentation into a README. Instead, I prefer to provide brief summaries only in the README and then point users to the main documentation for more details. For example, you could provide 1-2 sentences for each of the main sections and then point users back to your main docs for details. As a rule of thumb, a README might be the length of a poem while your docs are the length of a novel.

README's have the additional complication of being difficult to maintain. Unless you have rights to publish to the code repository, it might be cumbersome to update the README content. If you're an engineer who is writing the code and docs at the same time, this likely isn't an issue. But in many organizations, technical writers are separate from engineering teams, and technical writers usually don't publish code to GitHub repos. I've published to GitHub repos in the past (in an effort to speed along the publication of a sample app, I jumped through the hoops of the company's approval process and pushed out the content into the repo), but later I regretted doing so. I learned that the person who pushes content into a repo owns that content and all the filed issues, pull requests, and other responsibilities that come with repo management. I didn't want to be in that position &mdash; I wanted the engineers to own and maintain the code and control pushes to this space.

Overall, README files shouldn't contain so many doc details that the information begins to conflict or become outdated with your main documentation. As long as you have only brief, condensed information in your README, it likely won't go out of date with each release.

## Good Docs project template

If you're looking for more inspiration and guidance about product overviews, see the [API overview template from the Good Docs project](https://github.com/thegooddocsproject/templates/blob/master/api-overview/about-overview.md). They recommend similar sections as those I've been recommending here &mdash; establish who the docs are for, what problems the product solves, what market/industry the product is intended for, and so on. In the body of the overview, the Good Docs team recommends covering the following questions:

> * What is it supposed to do? (What problem does it solve, and for whom?)
> * What exact capabilities are available to the user? What services does it offer?
> * What does it not do that developers should know about?
> * What are the typical use cases?
> * How does it work? (What do users need to know about architecture and internal components?)
> * What dependencies does the developer need to know about before installing?
> * What technical requirements do readers need? Include development environment and licensing requirements.
> * What knowledge prerequisites does the developer need to know about before using the API?
>
> (See [The overview](https://github.com/thegooddocsproject/templates/blob/master/api-overview/about-overview.md))

This is all good information to include. Consider auditing your overview by asking each of these questions. Does your product overview provide answers? If not, add a section that answers the question.

## Sample structure of a product overview

Product overviews vary from product to product, but here's the general flow that I like to follow:

- Description of the product
- Intended audience
- Sample use cases
- Requirements to use the product
- List of components
- High-level architectural diagram of components + explanation
- Development effort/scope
- How to get support/help
- Link to getting started tutorial

These topics don't need to be standalone sections but can be interwoven into similar sections as you see fit.

At the end of the product overview, be sure to transition into the next logical step: getting started! Here's where your [getting started tutorial](docapis_doc_getting_started_section.html) gets handed off to the user. It's your call to action, so to speak.

{% include image_ad_right.html %}

## Sample product overviews

Here are a few sample product overviews.

### SendGrid

{% include course_image.html url="https://sendgrid.com/docs/User_Guide/index.html" filename="sendgridoverview" ext_web="png" ext_print="png" alt="SendGrid product overview" caption="SendGrid API overview" %}

The Sendgrid overview starts with two key sections: "What is SendGrid?" and "Who is SendGrid for?" I like the straightforward approach. Even in the description of what SendGrid is, the authors don't assume everyone knows what an SMTP provider is, so they link out to more information. Overall, in about 10 seconds you can get an idea of what the SendGrid API is all about.

{% include random_ad3.html %}

### Lyft

{% include course_image.html url="https://developer.lyft.com/docs/overview" filename="lyftapioverview" ext_web="png" ext_print="png" alt="Lyft product overview" caption="Lyft API overview" %}

Lyft's product overview starts in a similar way, with sections titled "What is Lyft?" and "Why Use Lyft as a Developer." Their homepage also provides information on access, rate limits and throttling, and testing. The Lyft authors also recognize that each tech domain has its own lingo, so they provide a [glossary](docapis_glossary_section.html) upfront.

### IBM Watson Assistant

{% include course_image.html url="https://cloud.ibm.com/docs/services/assistant?topic=assistant-index#index" filename="ibmcloudoverview" ext_web="png" ext_print="png" alt="IBM Watson Assistant overview" caption="IBM Watson Assistant overview" %}

IBM Watson Assistant starts off with a brief summary of the service, followed by a high-level diagram of the system and a summary about how to implement it. Including a diagram of your API gives users a good grounding about what to expect, such as the level of complexity and time it will take to incorporate the API.

### Video Skills Kit for Fire TV

{% include course_image.html url="https://developer.amazon.com/docs/video-skills-fire-tv-apps/introduction.html" filename="vskfiretv_productoverview" ext_web="png" ext_print="png" alt="VSK for Fire TV" caption="VSK for Video Skills Kit for Fire TV" %}

This is an overview I wrote for a product called "Video Skills Kit for Fire TV." The product overview stays at a high level by describing the capabilities the product provides, general implementation options, sample apps available, requirements to complete the implementation, supported countries, and next steps. There's a parallel product overview page called [Video Skills Kit for Echo Show](https://developer.amazon.com/docs/video-skills-multimodal-devices/introduction.html).

Both of these product overviews are like product landing pages within a larger developer portal that covers many different products. In fact, if you go to the [developer portal homepage](https://developer.amazon.com/), the page just routes you to different product overview areas.

## <i class="fa fa-user-circle"></i> Activity with product overviews

With the [open-source project you identified](docapis_find_open_source_project.html), identify the API overview. Then answer the following questions:

1. Does the documentation have a product overview?
2. Does the overview clarify who the API is for?
3. Does the overview indicate the market need or business problem the API solves?
4. What questions do you still have about the API after reading the overview?
5. How does the overview transition into a getting started tutorial or other first steps with the API?

{% include random_ad2.html %}

## Survey

I like to gather feedback about the articles I write. This helps me know if my arguments resonate with others or if my views are off-base with others' experiences. Here are about 10 brief survey questions for feedback. You can view the [ongoing survey results here](https://www.questionpro.com/t/PHwm1Zkxsv).

<script>
EMBED_PARAMS = {};
EMBED_PARAMS.surveyID =8125612;
EMBED_PARAMS.domain ="//www.questionpro.com";
EMBED_PARAMS.src ="//www.questionpro.com/a/TakeSurvey?tt=QU%2BU1R03H%2Bc%3D";
EMBED_PARAMS.width ="100%";
EMBED_PARAMS.height = "1000px";
EMBED_PARAMS.border = "hidden";
</script>
<div id="div_8125612"></div>
<script src="//www.questionpro.com/javascript/embedsurvey.js?version=1"></script>
