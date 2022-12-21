<h1>1. Understanding HTML</h1>

<h2>1) Introduction to HTML</h2>
- What is HTML? HTML is used to create web pages in a programming language. Web sites are all created using HTML.<br>
- Meaning and Features of HTML: Hyper Text Markup Language (HTML) refers to text that goes beyond simple text and has the ability to connect to certain parts of a webpage, or links. Markup Language is a type of programming language, characterized by its structural and hierarchical representation of information. HTML writes .html as a file extension and writes html code inside the file.<br>
- History of HTML: HTML was developed in the 1990s by British physicist Tim Berners-Lee. The initial purpose of the development was for researchers to quickly share information and documents. It's not the current form of web documents, but the purpose of sharing information is still the same.<br>
https://developer.mozilla.org/ko/docs/Web/HTML<br><br>

<h2>2) HTML Grammar – Tags</h2>
- What is Tag? HTML is a set of tags, and tags are the most important and basic rules in HTML. Tags have the meaning of 'tags, name tags to show something', and they are interpreted as similar in HTML. When we write code using various tags, the browser recognizes it and expresses the content.<br>
- How to use tags: The tags are represented by the <,> symbol and have a name between the <,> symbols. Most tags consist of a start tag and an end tag, and the end tag is preceded by the '/' symbol. The actual screen will be located between the start and end tags.<br>
<h1>Hello, HTML</h1> -> For the most basic example, code to output 'Hello, HTML' using <h1>
https://www.w3schools.com/tags/ref_byfunc.asp<br>
- What is an element? The entire tag, including the content, is called an element. Tags and elements have different meanings, but many people use the same meaning as tags, so be careful not to confuse them.<br>
https://developer.mozilla.org/ko/docs/Web/HTML/Element<br><br>

<h2>3) HTML Grammar – Properties</h2>
- What is an attribute? An attribute is a setting that allows you to provide additional information to the tag or control the behavior or representation of the tag.<br>
- How to use properties: Properties consist of names and values. Separate the tag name with a space after the tag name in the start tag and express it as property name = 'Property value'. Attribute values are expressed in single quotes (') and double quotes (").<br>
<h1 id="title">Hello, HTML</h1> -> <h1> Code for declaring the title value by adding the id attribute to the tag
- How to use multiple properties: Multiple properties exist, depending on their meaning and purpose, and you can declare multiple properties in a single tag. Use spaces to declare multiple properties.<br>
<h1 id="title" class="main">Hello, HTML</h1> -> Code for declaring two attributes: id and class
The declaration order of the properties does not affect the tag, and the result is the same even if the class is declared before id.<br>
- Type of property: Attributes are categorized by type into global properties available for all tags and attributes available only for specific tags. It is also divided into optional writable attributes and required attributes for a particular tag. The id and class used in the example are global properties.<br>
https://www.w3schools.com/tags/ref_standardattributes.asp<br>
https://www.w3schools.com/tags/ref_attributes.asp<br><br>

  <h2>4) HTML Grammar – Tag Overlapping</h2>
- Nesting Tags: You can declare another tag inside the tag. When using overlapping tags, overlapping child tags must not deviate from the parent tag.<br>
Invalid example: <i> started in <h1>Hello, <i>HTML</h1></i> -> <h1> but it is not correct to declare the tag alternately, declaring the tag before the end tag of the end tag of the parent <i>
Valid examples: <h1>Hello, <i>HTML</i></h1> ->You must first declare the end tag of <h1> and then declare the end tag of <h1>.<br>
http://validator.kldp.org/<br><br>

<h2>5) HTML Grammar – Empty Tags</h2>
- What is an Empty Tag? By default, the tag consists of a pair of start tags and two end tags, and the contents are inserted between them. However, some tags have tags that do not, and these tags are called empty tags with no content.
<br>, <img src=">, <input type="> empty tag has no content and no exit tag is required.<br>
- Features of empty tags: Empty tags are tags that are used for other purposes, even if they are not displayed on the screen through properties or on the screen. A typical case of empty tags is when the browser has to draw content directly on the screen. These tags are called replacement tags because the browser replaces the content. There are not only tags that are replaced by empty tags, but there are tags that are used for other purposes because there is no actual output on the screen. The example code <br> is in this case.<br>
https://developer.mozilla.org/en-US/docs/Glossary/Empty_element<br><br>

 <h2>6) HTML Grammar – Blank</h2>
- Space in HTML: By default, HTML ignores more than one space.<br>
<h1>Hello, HTML</h1>
<h1>Hello, HTML</h1>
<h1>
Hello,
HTML
</h1>
-> HTML ignores more than one space and opening, so all three of these are the same text
will appear on the screen.<br>
Editor used in the course: https://atom.io/<br>
https://www.hongkiat.com/blog/change-default-text-wrapping-html-css/<br><br>

<h2>7) HTML Grammar – Annotation</h2>
- Comment Tags in HTML: Annotations are meant to be used only for memo purposes without being exposed to the screen. If you mark it as an annotation in an HTML file, the browser does not recognize and interpret the part. Mark the beginning of the annotation as <!--> and end with the --> mark.<br>
<!-- Everything written here is annotated. --><br>
<!-- Comments can also be written in multiple lines.<br>
<h1>Hello, HTML</h1>
The <h1> tag above is not interpreted by the browser. --><br>
https://www.w3schools.com/tags/tag_comment.asp<br><br>

  <h2>8) The basic structure of a document</h2>
- HTML Basic Structure (HTML Document): The basic structure of HTML is a basic content that must be entered when creating a Web document, and is largely divided into document type definitions and <html> elements.<br>
<!DOCTYPE html>
<html lang=”ko”> 
<head>
<meta charset=”UTF-8”>
<title>HTML</title>
</head>
<body>
<h1>Hello, HTML</h1>
</body>
</html>
- Document type definition: Document type definition is commonly referred to as doctype (DTD). This is a declaration that tells the browser which version this document is created and must be declared at the top of the document.<br>
- <html>Element: After document type declaration, the <html> tag must appear, and the <head> tag and <body> tag are children. The lang property in the <html> tag means in which language the document was written. Tags located in the <head> tag are not displayed on the browser screen. Instead, it acts like setting the default information for documents or linking external style sheet files and js files. The charset property of the <meta> tag specifies how characters are encoded. The <body> tag contains what appears on the actual browser screen, and most of the tags we're dealing with in the future will be here.<br>
- The code above is the most basic document structure, usually with more tags than this.<br>
https://www.w3schools.com/tags/tag_doctype.asp<br>
https://www.w3schools.com/tags/tag_html.asp<br>
https://www.w3schools.com/tags/tag_head.asp<br>
https://www.w3schools.com/tags/tag_body.asp<br>
https://www.w3scholos.com/tags/tag_meta.asp<br>
