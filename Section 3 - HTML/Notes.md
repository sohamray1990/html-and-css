HTML -

The first thing we need to understand when it comes to HTML, is that we are talking about documents. More specifically, text documents.

An HTML document is just a text document.

BIG WORD ALERT : User Agent

Agent - Something that acts on someone else's behalf
User Agent - A Software that acts on the user's behalf. Example -

Browsers
Screen Readers
Googlebot

In this course, we are talking about creating those documents that will be requested by users.
So, we have an essential job. We want to HELP user agents do their jobs successfully. Our job is to help user agents deliver the contents in the most understandable, accurate way possible. So that, ALL users can benefit from it.

"Build Good habits, Break Bad habits".

---

Markup (Describing Content) - Literally the marks that an editor might make on a document to provide instructions or clarifications.

Soham Ray (This is his name) <- Markup can be this, but which part of the document is it? It is only Soham or Ray or Soham Ray?

<name> Soham Ray </name> <- We're marking up the document. These pieces have a name - TAGS. A Start Tag and an End Tag.

- Tags are a way to "markup" the document that is friendly to user agents (softwares that are acting on behalf of users) and easy for humans to read and write.
- "Markup" describes the document
- By marking up a document, you are attempting to add meaning

---

Language (Consistent Meaning) - The idea of language is to provide a consistent meaning, just like English or Spanish. Everyone writing HTML should be using the same markup to mean the same thing. This also means it's our job to learn and use the language fluently to use for it's purpose. To communicate meaning.

- Consistent Vocabulary
- Can convey meaning clearly
- Exists to facilitate communication
- When learning, can go to a dictionary to look it up

---

BIG WORD ALERT :

Semantic - Having to do with meaning.
Author - To contribute to writing a document. Adding meaning (being concerned to semantics) is a part of authoring.

When we author something, we are adding meaning. We are not just writing the contents, we are also making sure the contents are understood. And that's PART of authoring. So, when we add tags to a document, we are authoring a document. We're contributing to it, extending it and helping it to communicated accurately.

---

Tags, Attributes and Elements (The Building Blocks) : The Tag is about meaning. We can then add other related pieces of information or instructions to a Tag.

<name type="first" nickname="false"> Soham </name>

Here, "type" is an attribute. Syntax - attributeName = attributeValue.  
The above entire BLOCK with the Tags, Attributes and it's Contents is called an Element.

---

Elements and Trees :

<name>
<firstname> Soham </firstname>
<lastname> Ray </lastname>
</name>

Well formatted markups make it easy to see the relationships to tree data structures.

---

Markup Language is a proven technology, a proven approach to MARKING UP documents. And it exits everywhere.

Example - Change Word .docx to .zip and we can see the document.xml file where the WORD document content will exist, along with the markup. So, when Microsoft Word reads this markup language, it interprets it like a user agent and displays the file to the user. (Word Markup Language - WML).

So, now we'll start focusing on HTML which is a Hyper Text Markup Language.

---

Conceptual Aside : Specifications

"A Specification is a standard of precise requirements."

Internet technologies are governed by many such specifications. Sometimes, we call it just "spec".
So, there's a HTML specification. There's CSS specification. This course teaches you how to READ the specs. You'll be able to read the specification, make decisions and keep yourself upto date with the latest changes in the technology.

---

The HTML Specification (Dictionary for our markup language and lot more than that) :

The specification is for providing semantic-level markup language and associated semantic-level scripting APIs for authoring accessible pages on the web ranging from static documents to dynamic applications.

From DOM Spec -
Elements, attributes and attribute values in HTML are defined to have certain meanings (semantics).
These definitions allow HTML processors, such as web browsers or search engines, to present and use documents and applications in a wide variety of contexts that the author might not have considered.

By authoring good HTML, you are helping to make HTML document future proof. By being a good HTML author, you are extending the life of the project you are working on.

---

Conceptual Aside : Author VS Implementor

Authors - Writing and adding meaning to the document.
Implementor - Creating a user agent which will communicate the documents to the user.

We are working together, authors and implementors. We are following the specification when we add meaning. And interpretors are following the specification when they interpret the meaning.

You are READING the same specifications the people making Google Chrome are.

---

Content Models and Kinds of Content :

Big Word Alert -

Content Model : A description of the elements intended contents.

<element> ... </element> [... is the content model which discusses what is allowed]
