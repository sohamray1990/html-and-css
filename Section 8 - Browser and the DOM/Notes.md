Conceptual Aside - HTTP :

Hypertext - Text that references other text which the user agent enables the user to immediately access. We can go BEYOND just text.
Protocol - A system of tools between two entities to communicate.
Server - A computer or software that manages access to services and resources (like documents, images and videos).
Client - A computer or software that requests resources or services from a server.

A Request has an address, it even includes the User Agent, that's making the request.

HTTP/1.1 200 OK
Content-Length: 12
Connection: close
Content-Type: text/html

"A Blog post about HTML and CSS!"

A Response from a server might look something like this where it has in the protocol ways of saying, yes, I've this thing you are requesting. It exists.
And then below that it has the actual contents, which again is just text. Now, what we are showing here is just texts but we're talking about hypertexts. We can deliver hypertext. We build hypertext using hypertext markup language. But what it makes it hypertext is the fact that within that text you can link, you can reference other hypertext markup documents.

https://www.google.com/ (142.250.64.100)

When we make a request from a website, we're actually already accustomed to specifying what the transfer protocol is. That's why we have HTTP or HTTPS in front of the address that we are requesting in front of the resource that we are requesting from the server. Hypertext Transfer Protocol or a secure version of Hypertext Transfer Protocol is what we're using to make the request. And then the request will transfer into an address that specifies where to get the resource, the document etc from. So, all that together comprises hypertext transfer protocol.

Hypertext Transfer Protocol -

A set of rules for how two entities (client and server) can transfer text between themselves. Text which can link the user to other related text. And that's where the hyper comes from. Beyond text, it's hypertext. Its more than text.
That text then is usually marked up or described given meaning using a markup language: HTML.

When we say hypertext, the HT in HTML, we're talking about text that goes beyond just standard text but can reference other documents within it. And we markup our hypertext documents using hypertext markup language that we've been discussing all along.

In the modern age, we send more than just documents. We send images, we send videos. Now, that's technically still just text that's then interpreted by the user agent. But as a general concept that sometimes called hyper media, meaning everything that we send across the Internet, but all of that is still sent via HTTP.

---

Anchor Tags & Hypertext :

One of the most important elements of the Internet.

Links are a conceptual concept that represents a connection between two resources, one of which is the current document. These are typically called hyperlinks. Links to other resources exposed to the user by the user agent, so that the user can cause the user agent to navigate to those resources. That is, you click or tap on a link and the browser goes and get that resource.

<a href="https://sohamray1990.github.io/portfolio">My Portfolio</a>

The a element with href attributes that allow the user agent to inform the user that they can reference these addresses and then can go ahead and carry out if the user chooses to do so.

---

The Browser :

Within the internet browsers, there are a number of what we could consider as sub programs, dedicated areas of the browsers that do different types of things. For example -
a. Every browser has a code dedicated to networking that is dealing with those HTTP requests, downloading resources etc.
b. Rendering Engine
c. JavaScript Engine that runs code that's written to manipulate the web page and many other things
d. Every browser deals with Storage, it can store things for example, so that you don't have to download it again among other things.

In this course, we'll be focused on one of these four - The Rendering Engine.

Rendering Engine :

A computer program that transforms an HTML document into a visual, interactive representation of the document for the user. It is the system that goes from the HTML and ends up delivering you the web page visually.

However, as good HTML authors we'll never forget that first and foremost, we're writing good markups so that any user agent can interpret it to it's users appropritately. But here onwards we'll mostly be focused on the browser, interpreting it for the user visually.

---

Blink :

I want you to understand how rendering engines really work and understand that they're really just computer code being written by other people trying their best to conform to the HTML specification.

Blink - It is the name of the Rendering Engine used by chromium and chromium is a set of technologies that backs the Google Chrome browser. So, Blink is the rendering engine inside Google Chrome.

---

Engine Aside (Focus on the internal workings of the browser's rendering engine) :

Parser - That is to analyze text, character by character.

<h1> Hello World! </h1>

We can imagine that the engine starts reading the HTML, character by character. That's what it's programmed to do. And based on the characters it's going to make determinations based on the character. For e.g. if it finds the < character, it assumes it is the beginning of a tag. And it will move on until it finds a greater than character > and then it will say, there's an H1 tag starting here and it will keep that concept in memory. And it'll work through the text and at some point it finds another tag and sees that it's a closing tag. It matches all these concepts and then has something to work with. This information is now in it's memory and then the code decides what to do with that information, can then express appropriately the visual representation.

---

Named Charater References :

<h1> 4 < 3 </h1>

In our HTML document, as we've seen, we have markup and text. But what if some of the text looks like markup?

For example, if the browser rendering engine is going through and it recognizes the tag that was placed in the text. For the above example, the browser rendering engine, the parser in particular realize that no this isn't a part of a tag.

But what if I was writing something like this : <h1> Soham <<some text>> Ray </h1> ?

The parser decided to display the first less than and last greater than characters like this <>. So, this becomes an issue.
HTML has a solution here - https://html.spec.whatwg.org/#named-character-references

I get a table of named character references. This is a way to tell the parser what characters you want to display without actually typing the character. The above example can be written like this - <h1> Soham &lt;&lt;some text&gt;&gt; >> Ray </h1> and now the parser knows exactly what we are trying to do.

---

OBJECT :

A collection of data (information) and code (that is instructions to a computer that accomplishes things) which together represents something.

---

MODEL :

A representation of a thing.

So, if I have a model airplane, it represents a real airplane.

So then, we can also have object models.

OBJECT MODEL :

A collection of objects that represent a thing and provide access to examine or change that thing.

You've already seen that we can have an object that has data and references to code. But let's imagine instead that we are creating an Object Model for an online course like the one you're taking now.

An online course has a teacher. So, we could have an object to represent the teacher. We would have student object. And we might have a video lecture object that represents the video lecture. That said, this entire set of objects represents a thing. It represents an online class. So, we could say that this collection of objects is an online class object model.

We can use the object model to learn about the class, like who's the teacher and student. And there might be code that these objects provide to let us edit the class, make changes etc.

Representation of ONLINE CLASS :

Teacher :

A
0*01 Tony
0*02 Alicea

Student :

B
0*11 John
0*12 Doe

Video Lecture :

C
0*11 Title
0*12 Length

ONLINE CLASS OBJECT MODEL (OCOM) - We would know whenever we saw OM, we meant Object Model. Keep this idea in mind as we move in to one of the most important concepts related to the browser, when it comes to HTML and CSS.

---

Document Object Model (DOM) :

An object model that represents an HTML document, providing the ability to examine and change the document as presented via the user agent.

That means that we write or author an HTML document and the contents of the documents are used to create an object model that represents it, containing some of the SAME data and information, plus more with abilities to examine that document, change that document, not the actual original HTML, but what's presented via the User Agent.

The document object model we'll generally refer to as The DOM (A representation of the HTML document you authored). The document object model is what the browser uses to then build the visual representation of the HTML document.

What do you think the document object model is structured as? What kind of data structures do you think is involved?

- We've been talking about how HTML is well structured as a tree, that a tree representation works well. And so you can imagine that when a browser takes the HTML and creates the document object model, it would make sense that it would also be a tree. And it is. So, you'll also hear reference to the DOM Tree.

---

Building the DOM :

We'll take a deeper look into how the user agent builds the DOM. And we'll take a look at Blink.

We've already seen that the user agent helps the user to get the HTML document that we've placed on a server somewhere. User Agent requests that document. That document is returned to the user agent. It translates that marked up text and delivers a visual experience to the user in the browsers case.

Now, we're zooming in a little bit more on those steps. And now we understand that the user agent takes the markup document. And builds the DOM. It builds an object model that represents what was written in the HTML document. So, from here on out, as we talk about the browser, as we talk about the visual representation that's presented to the user, the web page. We're not going to think about the HTML document as purely what's being transmitted to the screen. Instead we're going to adjust our mental model and think about the DOM. The document object model is what is actually being used to transmit a visual represntation to the user.

---

Rendering Engine :

Firefox - Gecko
Safari - WebKit
