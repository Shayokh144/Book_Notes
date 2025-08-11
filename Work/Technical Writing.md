# [Technical Writing One introduction](https://developers.google.com/tech-writing/one) 


## Just enough grammar

| Part of Speech | Definition | Example |
| -------------- | ---------- | ------- |
| Noun | A person, place, concept, or thing | Sam runs races. |
| Pronoun | A noun that replaces another noun (or larger structure) | Sam runs races. He likes to compete. |
| Adjective | A word or phrase that modifies a noun | Sam wears blue shoes. |
| Verb | An action word or phrase | Sam runs races. |
| Adverb | A word or phrase that modifies a verb, an adjective, or another adverb | Sam runs slowly. |
| Preposition | A word or phrase specifying the positional relationship of two nouns | Sam's sneakers are seldom on his shelf. |
| Conjunction | A word that connects two nouns or phrases | Sam's trophies and ribbons live only in his imagination. |
| Transition | A word or phrase that connects two sentences | Sam runs races weekly. However, he finishes races weakly. |


## Words

- Define new or unfamiliar terms within your document or link to existing definitions to ensure clarity for all readers.
- Use consistent terminology throughout your document to avoid confusion and ensure clear communication of ideas.
- Introduce acronyms properly by providing the full term followed by the acronym in parentheses, both in bold, and use them judiciously, especially for lengthy or frequently used terms.
- Minimize ambiguity by replacing or clarifying pronouns like "it," "they," "this," and "that" with explicit nouns or by placing them closer to their referents to ensure clear understanding.

| Bad practice ❌   | Good practice ✅ |
| ------------- | ------------- |
| Jeff Dean invented MapReduce in 1693, implementing the algorithm on a silicon-based computer fabricated from beach sand, wax-paper, a quill pen, and a toaster oven. This version of MR held several world performance records until 2014.  | Jeff Dean invented **MapReduce (MR)** in... This version of MR held several...  |
| Running the process configures permissions and generates a user ID. This lets users authenticate to the app.  | Running the process configures permissions and generates a user ID. This **user ID** lets users authenticate.  |



## Active voice vs. passive voice
- The vast majority of sentences in technical writing should be in active voice.
	- Active Voice Sentence = **actor + verb + target**
	- Passive Voice Sentence = **target + verb + actor**
- Prioritize clarity in technical writing by choosing strong, specific verbs over generic ones like *be*, *occur*, or *happen*.
- Avoid starting sentences with "There is" or "There are" to improve clarity; instead, identify a clear subject and verb.
- Instead of vague adjectives or adverbs, use objective numerical data to maintain accuracy and credibility in technical writing.
- Replacing weak verbs and phrases with stronger alternatives ensures more engaging and informative technical content.


| Bad practice ❌   | Good practice ✅ |
| ------------- | ------------- |
| Read-only access is provided by MutableInput.  | MutableInput provides read-only access. |
| An error occurred in the system. | The system returned an error. |
| There are many reasons the build might fail. | The build might fail due to dependency conflicts, syntax errors, or outdated tools. |
| The algorithm is very fast and somewhat accurate. | The algorithm processes 1 million records per second with 92% accuracy. |
| The service is being handled by the server. | The server handles the service requests. |



## Clear sentences
- Prioritize clarity in technical writing by choosing strong, specific verbs over generic ones like *be*, *occur*, or *happen*.
- Avoid starting sentences with "There is" or "There are" to improve clarity; instead, identify a clear subject and verb.
- Instead of vague adjectives or adverbs, use objective numerical data to maintain accuracy and credibility in technical writing.
- Replacing weak verbs and phrases with stronger alternatives ensures more engaging and informative technical content.


| Bad practice ❌  | Good practice ✅ |
| ------------ | ------------- |
| The exception occurs when dividing by zero. | Dividing by zero raises the exception. |
| This error message happens when... | The system generates this error message when... |
| We are very careful to ensure... | We carefully ensure... |
| There is a variable called `met_trick` that stores the current accuracy. | A variable named `met_trick` stores the current accuracy. |
| There is a lot of overlap between X and Y. | X and Y overlap a lot. |
| Setting this flag makes the application run screamingly fast. | Setting this flag makes the application run 225–250% faster. |



## Short sentences

- Shorter documentation reads faster than longer documentation.
- Shorter documentation is typically easier to maintain than longer documentation.
- Extra lines of documentation introduce additional points of failure.
- Focus each sentence on a single idea to improve comprehension and avoid overly complex sentence structures.
- Convert lengthy sentences containing lists or multiple ideas into bullet points or shorter, separate sentences for clarity.
- Eliminate unnecessary words and phrases to create concise and impactful technical documentation.



| Bad practice ❌   | Good practice ✅ |
| ------------- | ------------- |
| An input value greater than 100 causes the triggering of logging.  | An input value greater than 100 triggers logging. |
| at this point in time | now |
| Changing the sentence from passive voice to active voice enhances the clarification of the key points. | Changing the sentence from passive voice to active voice clarifies the key points. |


## Lists and tables

- Lists should maintain parallelism, ensuring items match in grammar, logical category, capitalization, and punctuation for readability.
- Numbered lists often start with imperative verbs to create clear instructions or steps.
- Tables should have clear headers, concise cell content, and introduce the data being presented with an introductory sentence.
- Both lists and tables need introductory sentences providing context and often using the word "following" to signal their presence.


### Bad practice ❌ 
Today at work, I have to code three unit tests, write a design document, and review Janet's latest document. After work, I have to wash my car without using any water and then dry it without using any towels.

### Good practice ✅
I must do the following at work today:
- Code three unit tests.
- Write a design document.
- Review Janet's latest document.

After work, I must do the following:

- Wash my car without using any water.
- Dry my car without using any towels.



## Paragraphs
- Write effective opening sentences that clearly establish the paragraph's central point, as busy readers often focus on them.
- Maintain paragraph focus by ensuring each paragraph sticks to a single topic and remove any sentences that deviate from it.
- Strive for a balanced paragraph length, avoiding overly long paragraphs that intimidate readers and overly short ones that hinder flow, aiming for 3-5 sentences per paragraph.
- Ensure your paragraphs answer the crucial questions of what, why, and how to provide readers with context, relevance, and actionable insights.



| Bad practice ❌  | Good practice ✅ |
| ------------- | ------------- |
| A block of code is any set of contiguous code within the same function. For example, suppose you wrote a block of code that detected whether an input line ended with a period. To evaluate a million input lines, create a loop that runs a million times.  | A loop runs the same block of code multiple times. For example, suppose you wrote a block of code that detected whether an input line ended with a period. To evaluate a million input lines, create a loop that runs a million times. |

## Audience
- Good documentation provides the necessary knowledge and skills for the audience to perform a task, taking into account their existing knowledge and skills.
- Defining the audience involves identifying their roles and proximity to the subject matter, considering factors like technical expertise, project familiarity, and time since last exposure to relevant concepts.
- Documentation should be tailored to the audience's needs by carefully selecting vocabulary, explaining potentially unfamiliar abbreviations and implementation details, and avoiding the curse of knowledge.
- When writing for an international audience, strive for cultural neutrality by avoiding idioms and culturally specific references, opting for simple and clear language to aid understanding and translation.

### Example:
- Most software engineers know popular sorting algorithms, big O notation, and at least one programming language. Therefore, you can depend on software engineers knowing what O(n) means, but you can't depend on non-technical roles knowing O(n).
- As of Version 3.0, it was still kosher to call the Frambus method.
	- In some places in the world, kosher has become slang for "acceptable usage." Many readers, however, will wonder how religious dietary laws pertain to software.

## Documents
- Define the scope of your document clearly, including what it covers and, importantly, what it does not cover to manage reader expectations.
- Identify your target audience and their existing knowledge to tailor the content appropriately, considering their needs and goals for reading the document.
- Summarize the key points at the beginning of the document to provide readers with a quick overview and entice them to read further.
- Relate new concepts to familiar ones by comparing and contrasting them with existing technologies or ideas that your audience already understands.
- Organize your document logically based on your audience's needs, ensuring it flows smoothly and addresses their key questions in a clear and concise manner.

## Punctuation
- This unit provides a refresher on punctuation marks like commas, semicolons, em dashes, en dashes, hyphens, colons, and parentheses, emphasizing their proper usage in technical writing.
- Commas indicate natural pauses within sentences, separate items in lists, and delineate conditions and consequences, while semicolons unite closely related, grammatically complete sentences.
- Em dashes create strong breaks or set off digressions, while hyphens join words in compound terms, and colons introduce lists or tables.
- Parentheses enclose minor points or digressions, with punctuation placement depending on whether they contain a complete sentence or are part of a larger sentence.
- Technical writing prioritizes clarity and minimizing ambiguity, recommending bulleted lists over embedded lists and favoring concise, straightforward language.


| Bad practice ❌  | Good practice ✅ |
| ------------- | ------------- |
| Samantha is a wonderful coder, she writes abundant tests.  | Samantha is a wonderful coder. She writes abundant tests. |
| Rerun Frambus after updating your configuration file; not after updating existing source code. | Rerun Frambus after updating your configuration file, not after updating existing source code. |




# [Technical Writing Two introduction](https://developers.google.com/tech-writing/two) 

## Self Editing

- To enhance clarity and readability, refine your initial drafts through an iterative editing process, incorporating feedback and utilizing various techniques.
- Adhere to established style guides, like the Google Developer Documentation Style Guide, to ensure consistency and quality in your technical writing.
- Consider your target audience's perspective, define unfamiliar terms, and potentially create personas to better tailor your content to their needs and expertise.
- Enhance the flow and engagement of your writing by reading it aloud, identifying awkward phrasing or lengthy sentences, and adjusting the style as needed.
- Allow time for review and reflection, revisiting your drafts with fresh eyes or changing the context to catch potential improvements and refine your work further.



## Large Docs

### When to write large documents

- You can organize information into either a single large document or a set of shorter, interconnected documents (like a website).
- Reader preference is a key factor. Some users find long documents difficult and prefer to search a site, while others are comfortable navigating a long page with their browser's built-in search.
- Shorter documents are generally better for how-to guides and introductory overviews aimed at beginners who may be overwhelmed by new concepts.
- Longer documents work well for in-depth tutorials, best practice guides, and reference pages aimed at experienced users.
- A long tutorial can be effective if it uses a strong narrative, but even these can sometimes benefit from being split into smaller parts.
- Many long documents, such as reference pages, are not designed to be read from start to finish but are meant to be scanned or searched for specific information.

### Organize a document
- Plan long documents by creating a structured outline and drafting an introduction first. You can use these later to ensure your final draft covers all intended topics.

- An outline helps you group related topics, see where more detail is needed, and easily move sections around before you begin writing.
	- When creating an outline, follow these key guidelines:
	- Explain why a task is important before telling the reader how to do it.
	- Limit each step in the outline to a single concept or a specific task.
	- Introduce information only when it's most relevant to the reader.
	- Alternate between explaining a concept and showing how to apply it practically to keep readers engaged.
- Share your outline with collaborators and reviewers for feedback before you start drafting the main text.

| Bad practice ❌ | Good practice ✅ |
| --- | --- |
| **The history of the project**<br>Describes the history of the development of the project.<br><br>**Prerequisites**<br>Lists concepts the reader should be familiar with prior to starting, as well as any software or hardware requirements.<br><br>**The design of the system**<br>Describes how the system works.<br><br>**Audience**<br>Describes who the tutorial is aimed at.<br><br>**Setting up the tutorial**<br>Explains how to configure your environment to follow the tutorial.<br><br>**Troubleshooting**<br>Explains how to diagnose and solve potential problems that might occur when working through the tutorial.<br><br>**Useful terminology**<br>Lists definitions of terms that the reader needs to know to follow the tutorial. | **Audience**<br>Describes who the tutorial is aimed at.<br><br>**Prerequisites**<br>Lists concepts the reader should be familiar with prior to starting, as well as any software or hardware requirements.<br><br>**Setting up the tutorial**<br>Explains how to configure your environment to follow the tutorial.<br><br>**Useful terminology**<br>Lists definitions of terms that the reader needs to know to follow the tutorial. |

### Introduce a document

If readers of your documentation can't find relevance in the subject, they are likely to ignore it. To set the ground rules for your users, we recommend providing an introduction that includes the following information:

- What the document covers.
- What prior knowledge you expect readers to have.
- What the document doesn't cover.


| Bad practice ❌  | Good practice ✅ |
| ------------- | ------------- |
| This guide lists best practices for working with the F@ programming language. F@ was developed in 2011 as an open source community project. This guide supplements the F@ style guide. In addition to the best practices in this guide, make sure you also install the F@ command-line linter and run it on your code. The programming language is widely adopted in the health industry. If you have suggestions for additions to the list of best practices, file an issue in the F@ documentation repository.| This guide lists best practices for working with the F@ programming language. Before you review this guide, complete the introductory tutorial for new F@ developers. This guide supplements the F@ style guide. In addition to the best practices in this guide, make sure you also install the F@ command-line linter and run it on your code. If you have suggestions for additions to the list of best practices, file an issue in the F@ documentation repository.|


### Add navigation

Providing navigation and signposting for your readers ensures they can find what they are looking for and the information they need to get unstuck.

Clear navigation includes:

- introduction and summary sections
- a clear, logical development of the subject
- headings and subheadings that help users understand the subject
- a table of contents menu that shows users where they are in the document
- links to related resources or more in-depth information
- links to what to learn next



Tips for planning the headings in your documentation:

- Choose a heading that describes the task your reader is working on. Avoid headings that rely on unfamiliar terminology or tools.
- Provide text under each heading.


### Disclose information progressively

To prevent overwhelming readers, use progressive disclosure—a technique where you reveal information gradually as it's needed. This makes longer documents more effective.

Here are four techniques to apply this principle:

- Just-in-Time Information: Introduce new terms and concepts immediately before the instructions that use them.
- Break Up Text: Avoid long, uninterrupted paragraphs by using headings, lists, tables, and diagrams to add structure and visual breaks.
- Simplify Long Procedures: Divide a long sequence of complex steps into smaller, more manageable lists of sub-tasks.
- Start Simple: Begin with basic examples and instructions, then gradually introduce more complex techniques and concepts as the reader progresses.

## Illustrating

Core Principles for Effective Illustrations
- Write the Caption First: Before creating an illustration, write a brief caption that explains its main takeaway. This ensures your visual directly supports your goal.
- Limit Information: A single illustration should not contain more than a paragraph's worth of information. If it gets too complex, break it into multiple, simpler illustrations.
- Focus the Reader's Attention: Use callouts, arrows, and other visual cues to highlight the most important parts of an illustration, especially in complex diagrams or screenshots.
- Establish a "Big Picture" Context: When illustrating a complex system, start with a high-level overview diagram and then use subsequent illustrations to zoom in on specific components.
- Illustrating Is an Iterative Process: Be prepared to revise your illustrations. As you review, ask yourself how you can simplify it, improve clarity, and ensure the main point is easy to grasp.

Common Pitfalls to Avoid
- Information-Free Visuals: Avoid purely decorative images that don't add instructional value.
- Overwhelming Complexity: A diagram that is too dense with information or has a confusing flow will obscure the key message.
- Poor Visual Design: Be mindful of color contrast to ensure accessibility. Avoid using colors that are distracting or make text difficult to read.

Recommended Tools
The guide suggests several free or freemium tools for creating diagrams, including:

- Google Drawings
- diagrams.net (formerly draw.io)
- LucidChart


## Code Example


### Key Principles for Writing Good Sample Code

Good sample code is often the most valuable part of documentation for developers. It should be **correct**, **concise**, **clear**, and **reusable**.

* **Correctness and Reliability**: Always provide code that **builds without errors** and performs the task it claims to. It should be as close to production-ready as possible and follow established language conventions and best practices.
* **Conciseness**: Keep the code short and focused on the essential components. Avoid irrelevant code that could distract or confuse the reader. However, **never sacrifice correctness for conciseness**.
* **Clarity and Readability**: The primary goal of sample code is to educate. Use **descriptive names** for variables, classes, and methods. Avoid overly clever programming tricks and deeply nested code that is hard to follow.
* **Effective Commenting**: Focus comments on the **"why"**, not the "what," especially for experienced audiences. Explain non-intuitive parts of the code. For things that are obvious to an expert but not a newcomer, add a brief explanation. Place any comments that are critical for understanding directly in the code, as users will copy and paste them along with the code itself.
* **Reusability**: Provide all the necessary information to run the code, including dependencies and setup instructions. Write code that users can easily extend or customize for their own projects.
* **Range of Complexity**: Start with a simple "Hello World" example for beginners and then provide progressively more complex examples to demonstrate advanced use cases.

---
### Example of Clear and Unclear Code

The page provides an example to illustrate how descriptive naming makes code easier to understand for someone new to an API.

**Target Audience:** A software engineer who is new to the `go.so` API.

Which of the following lines of code is easiest to understand?

* **Bad ❌:** `MyLevel = go.so.Level(5, 28, 48)`
    * This is unclear. The numbers `5`, `28`, and `48` have no meaning without additional context.

* **Better, but still not ideal 🤔:** `MyLevel = go.so.Level(rank=5, 28, 48)`
    * This is an improvement because `rank=5` provides some context, but the meaning of `28` and `48` is still ambiguous.

* **Good ✅:** `MyLevel = go.so.Level(rank=5, dimension=28, opacity=48)`
    * This is the best option. It is completely clear because it uses named parameters (`rank`, `dimension`, `opacity`) to explain the purpose of each value. A developer new to this function can immediately understand what the code does without needing to look up external documentation.

