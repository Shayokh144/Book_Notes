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


