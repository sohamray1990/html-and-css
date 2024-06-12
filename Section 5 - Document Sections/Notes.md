Self-Contained Compositions (or the ARTICLE element) :

Categories -
Flow content (Document flowing from top to bottom)
Sectioning content (Defines the scope of the outline)
Palpable content (It's expected generally something is inside the element)

Content model -
Flow content

An article element represents complete or self-contained compositions in a document, page etc. This could be a form post, magazine, blog post, user comment etc. or any other independent item of content.
In other words, if you take that piece out of the document, it could still be it's own document and still make sense. A big part of being an HTML author is looking up at the content and deciding what tag, element works best for that piece of the content.
So, we have to look at our content and make a judgement call. Does this section of the article match the meaning of an article element.

---

Thematic Groupings (section) :

Categories -
Flow content (Document flowing from top to bottom)
Sectioning content (Defines the scope of the outline)
Palpable content (It's expected generally something is inside the element)

Content model -
Flow content

The section element represents a generic section of a document or application. A section, in this context, is a thematic grouping of content, typically with a heading.

---

Tangential Content (aside) :

Categories -
Flow content (Document flowing from top to bottom)
Sectioning content (Defines the scope of the outline)
Palpable content (It's expected generally something is inside the element)

Content model -
Flow content

The aside element represents a section of a page that consists of content that is tangentially related to the content aound the aside element and which could be considered as separate from that content. Such sections are often repesented as sidebars in printed typography.

---

Headings and Rank (h1-6) :

Categories -
Flow content (Document flowing from top to bottom)
Sectioning content (Defines the scope of the outline)
Palpable content (It's expected generally something is inside the element)

Content model -
Phrasing content

Heading content defines the header of a section (whether explictly marked up using sectioning content elements, example - <h1> ABC <h1> OR implied by the heading content itself, example <section><h2> Heading within the section</h2></section>).

These elements have a rank given by the number in their name.
h1 > h2 > h3 > h4 > h5 > h6

---

Headers and Footers (header and footer) :

Categories -
Flow content (Document flowing from top to bottom)
Palpable content (It's expected generally something is inside the element)

Content model -
Flow content, but with no header or footer element descendants

A header element is intended to usually contain the section's heading (an h1-h6 or hgroup element), but is not required. The header can also be used to wrap up a section's table of contents, search form, relevant logos.

A footer element represents a footer for it's nearest ancestor sectioning content or sectioning root element. A footer typically contains information about it's section such who wrote it, links to related documents, copyright data etc.

---

Addresses (address element) :

Categories -
Flow content (Document flowing from top to bottom)
Palpable content (It's expected generally something is inside the element)

Content model -
Flow content, but with no heading content, sectioning, header, footer elements.

The address element represents the contact information for it's nearest article or body element ancestor. If that's the body element, then the contact information applies to the document as a whole.
The address element must not be used to represent arbitrary addresses (eg. postal addresses), unless those addresses are in fact the relevant contact information. It should not contain information other than contact information.
