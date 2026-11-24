# Accessibility and SEO — Lucas Tippie

## Conclusion answers

**1. Why should positive tabindex numbers be avoided?**

Positive tabindex numbers change the normal keyboard order. This can make focus jump around the page and confuse users. They are also harder to maintain when new content is added. Use the natural HTML order, tabindex="0" when an item needs a normal Tab stop, and tabindex="-1" for a target that receives focus without adding a Tab stop.

**2. What is SEO?**

SEO means search engine optimization. It helps search engines understand a website and helps people find its content in search results.

## Changes in index.html

- Added a skip link as the first element inside body.
- Made the visible main element the focus target with id="main" and tabindex="-1".
- Added a strong visible focus outline and normal document-order navigation.
- Added tabindex="0" to selected headings for the assignment's Tab demonstration.
- Added ARIA names for navigation, main, and sections.
- Changed the generic title and description to describe the page.
- Added one clear h1 and an ordered h2/h3 heading structure.
- Replaced placeholder navigation with descriptive links to existing pages or real sections.
- Preserved the Bootstrap column examples, existing English language setting, viewport, semantic landmarks, and decorative icon aria-hidden attributes.
- Closed the head element properly and removed a reference to a stylesheet that does not exist.
- Added reduced-motion styling.

The lesson's display:none target cannot receive focus, so this page uses the visible main element instead. Normally static headings do not all need Tab stops: screen readers can navigate them using heading commands. Only the selected lesson demonstration headings have tabindex="0".

## Narrated video script (about one minute)

Highlight the indicated code while reading:

1. **title and meta description in head**
   “This is my Version 5 Bootstrap page. I changed the title to Bootstrap Layout Examples, with my name. I also changed the description so it clearly explains what the page contains. These help search engines understand the topic, and the description may appear in a search result.”

2. **h1, h2, and h3**
   “I added a clear main heading and smaller headings for each section. The headings organize the content for visitors and help explain the page topic.”

3. **navigation links**
   “I replaced vague links with descriptive labels, like Bootstrap grid examples and Open the practice form. These tell users and search engines where each link goes.”

4. **existing lang, viewport, header, main, and footer**
   “The original page already had an English language setting, a mobile viewport, and semantic elements like header, main, and footer. These already provide a useful foundation for an understandable, accessible page.”

5. **skip link, main target, and ARIA attributes**
   “For accessibility, I added a skip-to-main-content link, visible keyboard focus, and ARIA labels. Pressing Tab reveals the skip link, and Enter moves to the main content. These features help keyboard and screen-reader users.”

## Hands-on steps still required

These are personal exercises, not completed on your computer by the code changes.

1. Use the screen reader your teacher requires on the Canvas assignment. The pasted assignment did not include the extension-installation link or the video URL; use the original Canvas page for those.
2. Use Tab for interactive items and your screen reader's reading commands for regular text. Listen to image descriptions.
3. Compare the W3C before and after pages below. The accessible version includes skip links, descriptive image alternatives, and structured headings.
4. Open your updated index.html in a browser. Press Tab, Enter, and Tab again. Verify the skip link appears and focus moves into the main content. Test Shift+Tab too.
5. Record your screen and microphone while highlighting the code above and reading the script in your own voice. Use the recording tool from the assignment.
6. Upload the recording to Canvas Studio or your teacher's accepted video service, check the sharing permissions, and submit its link. No recording or Canvas submission has been made by this update.

## Sources

- MDN tabindex: https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Global_attributes/tabindex
- Google SEO Starter Guide: https://developers.google.com/search/docs/fundamentals/seo-starter-guide
- W3C inaccessible news: https://www.w3.org/WAI/demos/bad/before/news.html
- W3C accessible news: https://www.w3.org/WAI/demos/bad/after/news.html

## Verification

Static checks passed for skip-link placement, target focusability, one main landmark, one h1, no positive tabindex values, matching internal-link targets, ARIA label references, and SEO metadata. Automated browser testing was blocked by the execution environment, so the keyboard and screen-reader checks above remain necessary.
