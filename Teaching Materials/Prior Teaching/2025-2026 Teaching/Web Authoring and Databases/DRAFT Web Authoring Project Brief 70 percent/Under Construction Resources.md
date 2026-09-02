---
title: "Under Construction: Resources"
---

# Guidance and Support

## Planning Phase

Take the planning phase seriously. The time invested in thoughtful planning makes implementation considerably easier. Your planning documentation should show evidence of genuine thought about your target audience, design decisions, and site structure before you begin coding.

Research your chosen topic thoroughly. If your website provides information, ensure that information is accurate and properly referenced. If your website showcases products or services, think carefully about how to present them effectively.

## Design Principles

The four design principles (contrast, repetition, alignment, proximity) are not checkboxes to tick off. They are interconnected concepts that work together to create effective visual communication. Your planning documentation should show understanding of how these principles apply to your specific project.

Contrast helps users understand what is important. Repetition creates consistency and professionalism. Alignment creates visual order. Proximity shows relationships between elements. Consider how each principle serves your website’s purpose.

## Modern Layout Techniques

This project requires demonstration of both Flexbox and CSS Grid. These are the current standard approaches to CSS layout. Flexbox excels at one-dimensional layouts (rows or columns) and is particularly useful for navigation, card layouts, and distributing items in a container. CSS Grid excels at two-dimensional layouts where you need control over both rows and columns simultaneously.

You are not required to use only Flexbox and Grid for every layout decision. Sometimes a simple block element or inline-block is the right choice. The requirement is to demonstrate that you understand these modern techniques and can apply them appropriately.

## Responsive Design

Your website should work well on screens ranging from mobile phones to large desktop monitors. This does not mean it needs to look identical on all devices - it means the content should be readable and the navigation should be usable regardless of screen size.

Consider mobile users from the beginning rather than treating mobile as an afterthought. Test your website at various screen widths during development, not just after completion.

## Development Process

Build your website incrementally. Create the HTML structure first, then add basic CSS, then refine your layouts with Flexbox and Grid, then add responsive media queries and polish. This incremental approach makes debugging easier and helps you maintain working code.

Use the browser’s developer tools extensively. They allow you to inspect HTML structure, test CSS changes live, and view your site at different screen sizes. Learning to use these tools effectively is as important as learning HTML and CSS themselves.

## Code Quality

Write code that you could hand to another developer who would be able to understand and maintain it. Use meaningful class and ID names. Add comments where helpful. Format your code consistently. Organize your CSS logically.

Validate your HTML and CSS using the W3C validators. These catch syntax errors and standards compliance issues that might not be immediately visible but could cause problems later.

## Resources

You may consult tutorials, reference materials, and documentation while developing your website. However, all code you submit must be written by you. If you adapt code from a tutorial or other source, document this in your `planning.md` with proper attribution.

Recommended resources include MDN Web Docs, CSS-Tricks, and W3Schools for technical reference. For design inspiration, study professional websites in your chosen topic area, but do not copy their designs directly.

## Common Challenges

**Challenge:** Creating a navigation that works on both mobile and desktop
**Approach:** Start with a simple vertical navigation that works on mobile, then use media queries to transform it into a horizontal navigation on larger screens.

**Challenge:** Making images responsive
**Approach:** Set max-width: 100% and height: auto on images so they scale down on smaller screens but never scale up beyond their actual size.

**Challenge:** Deciding between Flexbox and Grid
**Approach:** Use Flexbox when arranging items in a single row or column. Use Grid when you need control over both rows and columns simultaneously, or when you want to create complex two-dimensional layouts.

**Challenge:** Writing effective documentation
**Approach:** Write your documentation for someone who understands basic web development but has never seen your specific project. Explain not just what you did, but why you made those choices.

---

# Additional Notes

## Scope and Ambition

This is a substantial project worth 70% of your module grade. The scope should reflect this weighting. A five-page website with sophisticated layouts, responsive design, and comprehensive documentation represents appropriate ambition for this assessment.

That said, a well-executed simple design is preferable to an overly ambitious design with technical problems. Focus on creating something that works reliably and demonstrates your skills clearly.

## Demonstration of Learning

This project should show growth from your Assignment 1 portfolio. The technical requirements are more demanding (five pages vs three, Flexbox and Grid required, responsive design emphasized). Your planning should be more thorough. Your design should show greater sophistication.

Use this project as an opportunity to consolidate and expand your learning. Experiment with techniques covered in class. Try implementing something slightly beyond what was explicitly taught. This is where real learning happens.

## Professional Context

The documentation requirements in this project reflect real-world professional practice. Developers regularly create planning documents, maintain project documentation, and write maintenance guides for clients or team members. These skills are as important as coding ability in professional web development.

Approach the documentation with the same care you bring to your HTML and CSS. Clear technical writing is a valuable professional skill.

---

# Learning Tips and Strategies

## Before You Begin Coding

Spend significant time in the planning phase. Sketch multiple versions of your layouts. Consider different color schemes. Think through your navigation structure. The time invested here saves time during implementation and results in a better final product.

Look at professional websites in your chosen topic area. What layout patterns do they use? How do they handle navigation? What design choices make them effective? You are not copying these sites, but learning from professional examples.

## During Development

Commit your code to GitHub frequently. This creates a history of your work and serves as backup. If something breaks, you can revert to a working version.

Test in multiple browsers regularly, not just when you finish. Browser-specific issues are easier to fix when you discover them early rather than after completing the entire site.

View your site on an actual mobile device if possible, not just in the browser’s responsive mode. Real devices sometimes behave differently than simulated ones.

## Problem-Solving Strategies

When something is not working:

1. Check the browser console for error messages

1. Use the browser’s element inspector to examine the HTML structure and applied CSS

1. Simplify the problem by temporarily removing code until the issue disappears

1. Search for error messages or specific problems - someone else has likely encountered the same issue

1. Take a break and return with fresh eyes

When you are stuck on a design decision:

1. Sketch multiple options on paper before committing to code

1. Look at how professional sites handle similar situations

1. Build a simple version first, then enhance it

1. Ask whether each design choice serves your users’ needs

## Time Management

This project runs for approximately three months. Divide the work into manageable phases:

**Weeks 1-2:** Planning, research, wireframes, site map
**Weeks 3-5:** HTML structure for all pages
**Weeks 6-8:** CSS implementation, basic layouts
**Weeks 9-10:** Flexbox and Grid layouts, responsive design
**Weeks 11-12:** Testing, refinement, documentation

Adjust this timeline based on your individual circumstances, but avoid leaving everything until the final weeks.

---

---

This project represents a significant portion of your module assessment and provides an opportunity to demonstrate comprehensive web development skills. Approach it with care, creativity, and professionalism. The result should be something you are proud to show others as an example of your capabilities.

## TO BE UPDATED: Page Structure Requirements

Your five pages should work together to create a cohesive website. Consider these approaches:

**Option A - Information/Resource Site:**

- Home page introducing the topic

- 3-4 content pages exploring different aspects

- Contact or resources page

**Option B - Business/Service Site:**

- Home page with overview

- Services or products page

- About page

- Gallery or portfolio page

- Contact page

**Option C - Educational/Tutorial Site:**

- Home page with introduction

- Multiple tutorial or lesson pages

- Resources page

- About or FAQ page

**Option D - Your Own Structure:**

- Propose and implement your own five-page structure

- Ensure clear purpose and logical organization
