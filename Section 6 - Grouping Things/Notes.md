The p element (represents paragraph) :

Categories -
Flow content (Document flowing from top to bottom)
Palpable content (It's expected generally something is inside the element)

Content model -
Phrasing content

A paragraph is typically a run of phrasing content that forms a block of text with one or more sentences that discuss a particular topic, as in typography, but can also be used for more "general thematic grouping". For instance, an address is also a paragraph, as is a part of a form, a byline, or a stanza in a poem.

---

Quotes (blockquote element) :

Categories -
Flow content (Document flowing from top to bottom)
Sectioning root
Palpable content (It's expected generally something is inside the element)

Content model -
Flow content

Blockquote element represents a section that is quoted from another source.

Attribution for the quote, if any, must be placed outside the blockquote element.

---

Unordered Lists (ul li elements) :

Categories -
Flow content (Document flowing from top to bottom)
If the element's children include at least 1 li element.

Content model -
0 or more li and script-supporting elements

The ul element represents a list of items, where the order of the list is not important - that is, where changing the order would not materially change the meaning of the document.

The li element represents list items. Context in which the element can be used -

> ol element
> ul element
> menu elements

---

Ordered Lists (ol li elements) :

Categories -
Flow content (Document flowing from top to bottom)
If the element's children include at least 1 li element.

Content model -
0 or more li and script-supporting elements

The ol element represents a list of items, where the items have been intentionally ordered.
The "reversed" attribute is a boolean attribute. If present, indicates a descending list (3, 2, 1...). If the attribute is ommitted, the list is an ascending one.

---

Association Lists (dl, dt, dd element) :

dl element represents an association list consisting of 0 or more name-value groups (a descriptive list).

Categories -
Flow content (Document flowing from top to bottom)
If the element's children include at least 1 name-value group element (Palpable content).

Content model -
0 or more groups consisting of one or more dt elements followed by one or more dd elements

---

Multidimensional Content (table element) :

Tabular - Consisting of or presented in columns or tables. Represents data with more than one dimension, in the form of a table.

Categories -
Flow content (Document flowing from top to bottom)
Palpable content (It's expected generally something is inside the element)

Content model -
thead, tbody, tfoot

**_ As an HTML AUHTOR, you need to think ONLY about what is best for the presentation of that data to the user, the way they need to consume it, the device they will consume it on, the way they will use the data, what they'll be looking for. Once you put the hat on, the user agent and the user is should be what's present in your mind. All the work of database and code was done so that you can abstract all the work away so that it can fade into the background. The best work does fade into the background and all that's left is the user experience. How data is stored does not always match how it should be expressed. _**

"Be an AUHTOR, provide the User Agent with Meaning"

In other words, maybe it's not necessarily a table, maybe it's an ordered/unordered list or an association list. If it's visual, maybe instead of a table it should be a card.

---

Dominant Content (main element) :

Categories -
Flow content (Document flowing from top to bottom)
Palpable content (It's expected generally something is inside the element)

Contexts in which it can be used -
Where flow content is expected, but only if it is a "hierarchically correct main element".

Content model -
Flow content

The main element represents the dominant contents of the document.

A hierarchically correct main element is one whose ancestor elements are limited to html, body, div, form. Each main element must be a hierarchically correct main element.
A document must not have more than one main element that does not have the hidden attribute specified.

---

DIV... and Doing It Wrong :

Categories -
Flow content (Document flowing from top to bottom)
Palpable content (It's expected generally something is inside the element)

Content model -
Flow content

The div element has no special meaning at all. It represents its children.

Authors are strongly encouraged to view the div element as "an element of last resort", for when no other element is suitable. Use of more appropriate elements instead of the div element leads to better accessibility for the readers and easier maintainability for the authors.

<div>
    <div>Soham Ray</div>
    <div>Coder with a varied lot of interests Website:</div>
    <div>
        <div>Website</div>
        <div>https://sohamray1990.github.io/portfolio</div>
        <div>Phone :</div>
        <div>+91 XXXXX365</div>
    </div>
</div>

From a pure authoring perspective, the above markup makes no sense. It's meaningless. And not only is it more difficult for the user to get good information from it, consider if you had to go back and edit this content to figure out what it was doing.

There are many, many HTML authors out there today who are writing the HTML like this because they are entirely focused on making things work visually. And so they are using the elements just as hooks for CSS. That's incorrect. We are good HTML authors, we are marking up the document to add meaning to desribe the document for a more maintainable and accessible HTML documents.

You are thinking as an author. You are thinking about describing and adding meaning to the document. You are not thinking visually (one particular user agent). You are already more skilled in HTML authoring than many web developers if the above code looked wrong to you.

Scenarios to use DIV -

<article lang="en-US">
    <h1>My use of language and cats </h1>
    <p> Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>   
    <div lang="en-GB">
        <p>Vel molestiae vitae eius enim dolor repudiandae odio saepe praesentium numquam nam repellat fugiat dolorum nostrum pariatur deleniti quod, ab cupiditate accusantium tempore eligendi perspiciatis. Iste aliquam praesentium assumenda asperiores qui deserunt, nostrum possimus dicta, ea nulla sunt illum eligendi. Qui, maxime!</p>
    </div>
</article>

In this specific case, the div is necessary as a wrapper to the paragraph which has content in a different language. There is no HTML element to say this is in a different language, there's only an attribute.
