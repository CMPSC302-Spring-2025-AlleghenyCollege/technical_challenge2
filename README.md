# Technical Challenge 2: Semantic HTML and JAMstack with 11ty
## Review of HTML, Semantic HTML, and JAMstack Concepts. Introduction of 11ty.
## Deadline: 11am on January 31st, 2025

---

### Overview

In this challenge, you will build a simple, accessible, and high-performance site using semantic HTML and 11ty (Eleventy). You will learn to:
- Apply semantic HTML elements to structure your webpage for accessibility and SEO.
- Use 11ty to create a static site generator (SSG) that builds your site.
- Understand how JAMstack principles (JavaScript, APIs, and Markup) contribute to modern web development.

### Resources

- [HTML5 Semantic Elements](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)
- [11ty Documentation](https://www.11ty.dev/docs/)

---

### Requirements

1. **Semantic HTML**
   - Modify an empty `base.html` file in the `site/_includes` directory to make whatever site you wish. Include at least 20 elements from the following list, at least 10 of which must be semantic elements:
     - `html`, `img`, `footer`, `br`, `b`, `button`, `body`, `h1`-`h6`, `li`, `ul`, `div`, `table`, `section`, `script`, `em`, `meta`, `title`, `nav`, `style`, `article`, `template`, `noscript`, `span`, `link`, `header`, `svg` 

2. **Set Up a New Eleventy Project**

   - [Install](https://nodejs.org/en/download/) `Node.js` if you don't already have it 
   - In the `site/` directory, initialize a `Node.js` project by running the following command to create a `package.json` file:

   `npm init -y`

   - Install [Eleventy](https://www.11ty.dev/)

   `npm install --save-dev @11ty/eleventy`

3. **Configure Eleventy**
   - Create an Eleventy configuration file

   `touch .eleventy.js`

   - Then, open `.eleventy.js` and add the following configuration:

      ```
      module.exports = function(eleventyConfig) {
         return {
            dir: {
                  input: ".",
                  includes: "_includes",
                  output: "_site"
            }
         };
      };
      ```

4. **Run Eleventy**
   - Run Eleventy to generate the site

   `npx eleventy`

   This will generate files inside the `_site` directory.

   - Start a local development server

   `npx eleventy --serve`

   - Now, open `http://localhost:8080` to see your site in action! Stop here, do not deploy it!

## Report

Write a report, completing prompts provided in `writing/report.md`.

## Submission 

Commit your updated files to the repository with meaningful commit messages.

## Evaluation

To receive credit for this assignment, all of the following items in the checklist must be completed and checked off:

1. [ ] The site includes a semantic `base.html` file.
2. [ ] At least 20 HTML elements from the given list are correctly used.
3. [ ] At least 10 of the used  HTML elements are semantic elements.
4. [ ] The 11ty project is set up correctly.
5. [ ] The 11ty project is configured correctly.
6. [ ] The 11ty development server runs successfully and the site is previewed locally.
7. [ ] A report is completed, which includes a screenshot of locally built site. 
8. [ ] The repository contains all source files, including the generated files.
9. [ ] Meaningful commit messages are used to document progress.
10. [ ] The completed tasks have been checked off correctly.
