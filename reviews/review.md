# Technical Documentation Review Template

## Documentation Title

[Crawlee](https://crawlee.dev/)

## Reviewer Information

- **Name**: Ayu
- **Date of Review**: 25 September 2024
- **Review Level**: Beginner

## 1. Summary

<!-- Provide a concise summary of the documentation. What is it about? What purpose does it serve? -->

Crawlee is a web scraping and browser automation library that helps users build reliable crawlers. It makes HTTP requests that mimic browser headers and fingerprints and can switch crawlers from HTTP to headless browsers. These features allow crawlers to appear human-like and be undetected by modern bot protections.

## 2. Clarity and Comprehensiveness

- **Clarity**:

  <!--
  - Is the information easy to understand?
  - Are the sentences and paragraphs clear and straightforward?
  - Is the language appropriate for the intended audience?
  -->

The information is easy to understand, and the language is appropriate for the intended audience.

However, not all sentences and paragraphs are clear and straightforward. Some folks might like to read the documentation line by line, which can cause them to read something a couple of times to understand better.

Below is an example:

In the "[Creating a new project](https://crawlee.dev/docs/introduction/setting-up#creating-a-new-project)" section:

> A prompt will be shown, asking you to select a template. Crawlee is written in TypeScript so if you're familiar with it, choosing a TypeScript template will give you better code completion and static type checking, but feel free to use JavaScript as well. Functionally they're identical.

Adding some punctuation and splitting the long sentence into shorter ones would be helpful for clarity and better understanding. Although Crawlee is written in TypeScript, considering it also offers to use JavaScript, the sentence above can be improved with something like:

> A prompt will be shown, asking you to select a template. Choosing a TypeScript template will give you better code completion and static type checking if you're familiar with it. Otherwise, you can select JavaScript. Functionally, they're identical.

As the documentation is aiming audiences with the knowledge of JavaScript—and potentially TypeScript—another suggestion is not to mention them at all and go straight to the point as below:

> A prompt will be shown, asking you to select between a TypeScript or JavaScript template.

- **Comprehensiveness**:

<!--
 - Does the documentation cover all necessary topics?
 - Are there any missing sections that are critical for understanding?
 - Does it provide sufficient examples, diagrams, or references?
-->

The documentation covers all necessary topics and provides sufficient examples and references. It even provides a [dedicated chapter for examples](https://crawlee.dev/docs/examples). It's also very thoughtful to provide technical explanation pages within the "[Guides](https://crawlee.dev/docs/guides)" chapter and link them within the docs.

## 3. Accuracy and Relevance

- **Accuracy**:

<!--
 - Are the technical details correct?
 - Is there any outdated or incorrect information?
-->

I found at least one outdated information as below:

The "[JavaScript rendering](https://crawlee.dev/docs/guides/javascript-rendering)" chapter explains the JavaScript rendering through a demonstration.

As per documentation, I should get `ACTOR:` and nothing else on the console when I ran the first code. Instead, I got the below info on the console with no `ACTOR:` printed anywhere:

"`bash
INFO  CheerioCrawler: All requests from the queue have been processed, the crawler will shut down.
INFO  CheerioCrawler: Final request statistics: {"requestsFinished" :1, "requestsFailed" :0, "retryHistogram":[1], "requestAvgFailedDurationMillis":null, "requestAvgFinishedDurationMillis":4688, "requestsFinishedPerMinute":9, "requestsFailedPerMinute" :0, "requestTotalDurationMillis":4688, "requestsTotal" :1, "crawlerRuntimeMillis":6821}
INFO  CheerioCrawler: Finished! Total 1 requests: 1 succeeded, 0 failed. {"terminal":true}
```

It further says:

> You can confirm this using Chrome DevTools. If you go to https://apify.com/store, right-click anywhere in the page, select View Page Source and search for ActorStoreItem you won't find any results.

Searching for `ActorStoreItem` in the View Page Source found 183 results for all CSS classes. If these classes do not correspond to the documentation, they must be updated to match what `ActorStoreItem` users want to look for.

- **Relevance**:

<!--
 - Is the content relevant to the current state of the product/technology?
 - Does it align with the latest best practices and standards (e.g., Google's technical documentation style guide, Microsoft Manual of Style)?
-->

The content is relevant to the product's current state. In general, the documentation aligns with the latest Microsoft Writing Style Guide. For example, the documentation is written like we speak. However, it can still be improved by following the best practices of [Top 10 tips for Microsoft style and voice](https://learn.microsoft.com/en-gb/style-guide/top-10-tips-style-voice).

One example is to improve the consistency of contractions, such as it's, you'll, you're, we're, and let's.

Taking from the "[Pagination](https://crawlee.dev/docs/introduction/real-world-project#pagination)" section in the "Real-world project" chapter:

> When switching between pages, _you will_ see that the URL changes to:

And right in the following line:

> Try clicking on the link to page 4. _You'll see_ that the pagination links update and show more pages.

## 4. Structure and Organization

- **Logical Flow**:

<!--
 - Is the documentation logically structured?
 - Are sections and subsections well-organized?
-->

The documentation is logically structured and well-organized. It's pleasant to follow.

However, one subsection in a page might be part of a heading. In the "[JavaScript rendering](https://crawlee.dev/docs/guides/javascript-rendering)" chapter, "[Waiting for elements to render](https://crawlee.dev/docs/guides/javascript-rendering#waiting-for-elements-to-render)" might be a subsection of "[Headless browsers](https://crawlee.dev/docs/guides/javascript-rendering#headless-browsers)". But they have the same heading level.

- **Navigation**:

<!--
 - Is it easy to navigate through the document?
 - Are there clear headings, subheadings, and an index/table of contents?
-->

The documentation is easy to navigate because the headings, subheadings, and table of contents are clear, and links are generously provided.

## 5. Visual and Design Elements

- **Visuals**:

  <!--
  - Are diagrams, screenshots, and tables used effectively?
  - Are visuals clear, properly labelled, and relevant?
  -->

 Screenshots are used effectively. They're also clear, properly labeled, and relevant.

- **Design**:

  <!--
  - Is the document aesthetically pleasing?
  - Is there consistent use of fonts, colors, and formatting?
  -->

 The documentation's aesthetics can be improved. Admonitions (notes, info, tips, warning cards) are very helpful for clarity and caution. However, some pages, e.g., [Scraping the Store](https://crawlee.dev/docs/introduction/scraping), have back-to-back admonitions, which can distract the audience.

 Fonts and colors are consistent throughout the docs. Yet, some formatting can be improved for consistency. Let's take an example from [Getting some real-world data](https://crawlee.dev/docs/introduction/real-world-project) page. There are two ways a link is formatted in the documentation:

  - **As an inline code**

    > ...when we already know that everything we want to extract can be found at the `https://warehouse-theme-metal.myshopify.com/collections` page.

  - **As an external link**

  > Let's open DevTools by going to https://warehouse-theme-metal.myshopify.com/collections in Chrome...

## 6. Suggestions for Improvement

<!--
- Provide specific, actionable suggestions to improve the documentation.
- Mention any sections that need expansion, rephrasing, or additional content.
-->

### Actionable Suggestions

- Some long sentences can be broken into shorter sentences for better reading and understanding.
- Using punctuation properly can help the audience understand the exact meaning of a sentence.
There might be another way to avoid using heavy back-to-back admonitions so that the audience isn't distracted.
- The consistency of using "you" and "we" can be improved. For example, in the "[Scraping the Store](https://crawlee.dev/docs/introduction/scraping)" page, some sections use "you", and some go with "we"."

### Sections that Need Expansion, Rephrasing, or Additional Content

There are below sentences in the "[Headless browsers](https://crawlee.dev/docs/guides/javascript-rendering#headless-browsers)" section:

> You can choose from two libraries to control your browser: Puppeteer or Playwright. The choice is simple. If you know one of them, choose the one you know. If you know both, or none, _choose Playwright, because it's better in most cases_.

> _Playwright is a little more pleasant to use_, but both libraries will get the job done.

Looking at the wording I emphasize here, the documentation recommends that the audience use Playwright. But it'd be great to explain why Playwright is better than Puppeteer so that the audience can confidently choose one. Also, these sentences give a subjective opinion.

It'll be even better to have a table that shows the differences, such as their strengths and weaknesses.

## 7. Notable Strengths

<!--
- Highlight what the documentation does well.
- Mention sections that are particularly well-written or effective.
-->

The documentation is quite informative for those who are new to web scraping. It provides detailed explanations about how to use the tools, along with enough code examples and screenshots.

The "[Introduction](https://crawlee.dev/docs/introduction)" chapter, in particular, does a great job of walking the audience to understand Crawlee and scraping data step-by-step.

## 8. Identified Errors/Inconsistencies:

<!--
- List any errors, inconsistencies, or ambiguities.
- Provide examples where necessary.
-->

Please see explanations and examples in below sections:

- [2. Clarity and Comprehensiveness](#2-clarity-and-comprehensiveness)
- [3. Accuracy and Relevance](#3-accuracy-and-relevance)
- [Sections that Need Expansion, Rephrasing, or Additional Content](#sections-that-need-expansion-rephrasing-or-additional-content)

## 9. Best Practices Compliance

- **Standards**:
  <!--
  - Does the documentation adhere to recognized standards (e.g., Google's Documentation Guide)?
  - How does it compare with industry best practices?
  -->

 Creating standards throughout the documentation can be improved. Please see the "Relevance" in the [3. Accuracy and Relevance](#3-accuracy-and-relevance) as an example.

## 10. Overall Assessment

<!--
- Provide an overall assessment of the documentation, including a summary of your key findings.
- Rate the document on a scale from 1 to 5 based on overall quality and usability.
-->

I rate the document 3 on a scale of 1 to 5.

As a background, I have no knowledge of web scraping. Reading the documentation and following the instructions helped me understand web scraping and what Crawlee does. I also gained more knowledge about web scraping, crawling (which I heard a lot about but am not sure what it is), and so on.

Why 3? I'm one of those readers who read line-by-line when I want to understand something more. Sometimes, I had to read a paragraph a couple of times to understand the information because some sentences were not straightforward and too wordy.

## 11. Additional Comments

<!-- - Any additional observations or comments. -->
