---
title: Universal Chirpy Prompts for Enhancing Blog Posts
description: Two master prompts to either optimize your blog content or get structured feedback using Chirpy's advanced Markdown features.
date: 2025-06-21 18:00:00 +0000
categories: [Chirpy, Workflow]
tags: [markdown, prompt, automation]
hidden: true
---

Writing Markdown blog posts in **Chirpy** can be powerful when you use all the features the theme supports — from Mermaid diagrams and code highlights to responsive images and MathJax. But not every post needs every feature.

Below are **two universal prompts**:  
- The first gives you **feedback** on what to add and where.  
- The second gives you a **fully rewritten** blog post with Chirpy enhancements applied.

You can copy-paste either one into ChatGPT, Claude, or any AI assistant that accepts prompts — then paste your raw post under it. That’s it.

---

## 🔍 Prompt 1: Get Feedback on What to Add

> Use this prompt when you want to keep your blog post unchanged but receive **actionable suggestions** about what Chirpy-specific Markdown enhancements you’re missing.

````markdown
I am using the Chirpy Jekyll theme for my blog. I will give you a raw blog post written in plain Markdown (without enhancements). Your job is **not to rewrite it**, but to give me clear, detailed feedback on what Chirpy-specific Markdown enhancements I should add, and exactly where I should put them.

These enhancements must follow **Chirpy’s official syntax and capabilities only**. Don’t make up anything outside of Chirpy’s supported features. Use the documentation from Chirpy as your exact reference, including:

- Filepath highlights  
- Footnotes and reverse footnotes  
- Inline code and code blocks (with optional language, filename, or line number toggles)  
- Prompts (`tip`, `info`, `warning`, `danger`)  
- Custom image options: size (`w`, `h`), position (`.left`, `.right`, `.normal`), shadow, caption, dark/light mode, and preview image in front matter  
- Embedded media: audio/video from file or platforms (YouTube, Twitch, etc.)  
- Mermaid diagrams  
- Math blocks and inline math using MathJax (with correct `$$` syntax and equation labels)  
- Front Matter options: `description`, `pin`, `author`, `image`, `toc`, `math`, `mermaid`, etc.  
- Lists (ordered, unordered, ToDo)  
- Tables  
- Blockquotes  

**Important Rules:**
1. Do not add or change the original content.
2. Only suggest changes that are necessary based on the content's context (e.g., don’t suggest Mermaid for non-diagram topics).
3. If a certain feature is applicable but optional, mention it as a light suggestion, not a requirement.
4. Use simple, everyday English in your explanations.
5. Make the suggestions in a structured format, like this:

Suggested Improvements:

1. Use a file path highlight in this sentence: "Located at /assets/data".
Suggestion: /assets/data{: .filepath}


2. Turn this paragraph into a "tip" prompt: "Make sure to save before closing."
Suggestion: > Make sure to save before closing. {: .prompt-tip}


3. Add a preview image to the Front Matter using:
image: /path/to/preview.jpg



Only use Chirpy Markdown. Don't simplify anything into generic Markdown or HTML.


---

🛠 Prompt 2: Fully Rewrite the Blog Using Chirpy Markdown

> Use this when you want the AI to rewrite your entire blog post using every applicable Chirpy Markdown feature correctly.



I am using the Chirpy Jekyll theme. I will provide you with a raw blog post written in normal Markdown or text. Rewrite and return a **fully enhanced version** using only **Chirpy-supported Markdown features**. Make it perfect for readability, structure, and SEO, while keeping the original meaning.

Apply the following formatting and features, **only if they make sense** for the blog’s topic (e.g., technical, editorial, tutorial, etc.):

- Use proper Front Matter (`---`) with keys like: `title`, `description`, `date`, `categories`, `tags`, `author`, `pin`, `image`, `toc`, `math`, `mermaid` as needed
- Add a preview image in the Front Matter if relevant, using `image:` with `path`, `alt`, and optional `lqip`
- Use filepath highlights: `path/to/file`{: .filepath}
- Use inline code and code blocks, with language and filename attributes where needed
- Add footnotes and reverse footnotes if references or explanations are required
- Embed Mermaid diagrams or MathJax equations only if the topic contains diagrams or math
- Use Chirpy-style prompts (tip/info/warning/danger) for key information or notes
- Use Chirpy-enhanced image syntax: size (`w`/`h`), position (`.left`, `.right`), shadow, light/dark variants
- Embed video/audio using Chirpy’s `include` Liquid syntax if needed
- Convert relevant parts into lists: ordered, unordered, description, or ToDo
- Add links and tables using proper Markdown

**Important:**
- DO NOT invent or hallucinate content. Stick to the original message.
- DO NOT use generic HTML or Markdown. Only use Chirpy-supported syntax.
- Optimize for readability and structure without overloading it with features.
- If a feature doesn’t naturally fit the content, skip it.
- Use correct spacing between sections, proper heading levels, and TOC if appropriate.

Return the entire blog post as a single `.md` file (Markdown format), starting with Front Matter and ending with the last line.


---



