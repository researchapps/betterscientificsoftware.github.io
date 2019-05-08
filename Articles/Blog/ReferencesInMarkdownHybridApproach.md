# Wikipedia-Like References In GitHub Markdown

#### Contributed by [Mark C. Miller](https://github.com/markcmiller86)

#### Publication date: May 1, 2019

We use blocks of Lorem Ipsum text to
demonstrate attempting using
[GitHub Flavored Markdown](https://github.github.com/gfm/)
to achieve Wikipedia style footnoting and references. 
Also, we use 4 different link examples...

- Ftp link to a pdf file using a number as a handle
- YouTube video link using a 3-letter initial as a handle
- Normal wikipedia page link using a two-digit number as a handle
- Link to a specific page of a PDF using a number as a handle

We've noticed GitHub's rendering on GitHub site doesn't support the FTP link
but maybe the BSSw site does?

Some of our goals with this are to support...

- Mobile friendly
- Get teaser or summary text about the purpose of a linked reference
  before having to actually follow the link
- Link to reference list then to actual reference
- Separately listed references at the end of the article
- Maximally GitHib Markdown friendly
- Minimal use of in-line HTML
  - `<sup>XX</sup>` for footnote super-scripting
- Minimal requirement on back-end processing
- Avoid duplication of link/reference content
- Ease of use for authors

A key issue is that [GitHub Flavored Markdown](https://github.github.com/gfm/)
does not support creation of user-defined *anchors*. It does support *anchors*
but only for an implicit name-mangling of section headings. We could support
our list of references as level-6 (`######`) section headings but by default
those render (as `<h6>`) with far too much verticle space between each entry.

### Examples of the Possible Strategies

- [Hybrid of Reference Style Links and In-Line HTML Anchors](#hybrid-of-reference-style-links-and-in-line-html-anchors)

## Hybrid of Reference Style Links and In-Line HTML Anchors

Lorem ipsum dolor sit amet, consectetur adipiscing elit<sup>[A1]</sup>.
Sed quis dui et tortor molestie malesuada. Donec non consectetur arcu,
at semper magna.  Maecenas consectetur porttitor justo ac aliquam.
Curabitur vel faucibus augue<sup>[A1],[ALCM]</sup>. Maecenas vestibulum
orci vitae libero blandit, sit amet maximus turpis pharetra. Sed ultrices
tellus non pulvinar lacinia. In nec mi lobortis, euismod dui at, dapibus
turpis. Proin et ornare ex<sup>[A3]</sup>. Praesent in posuere risus.
Vivamus eleifend nulla eu nisi tincidunt, a mollis mi tincidunt. Nulla
quis velit vel felis mattis tincidunt a ac neque. Aenean viverra leo et
mollis gravida. Integer et fermentum tellus. Phasellus a arcu vitae ipsum
interdum finibus.<sup>[A1],[A02],[A3]</sup>

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris vel velit eget elit tempor tristique nec sed leo. Vivamus commodo nisl tellus, lobortis imperdiet nisl consequat in. Sed tellus ex, laoreet eu dapibus sed, malesuada imperdiet diam. Nunc eu rutrum dui. Nam ut turpis neque. Mauris at nulla faucibus, ullamcorper dolor in, tincidunt ante. Quisque consequat ullamcorper quam, quis ullamcorper sapien sollicitudin eu. Curabitur mattis ipsum et elit semper sollicitudin. Cras ut eros vitae tellus pharetra commodo. Donec blandit sagittis purus ac commodo. Curabitur fermentum suscipit odio, ac pellentesque ipsum auctor eu.


[A1]: #B1 "Whole Book 'Apollo Guidance Computer Architecture and Operation'"
[ALCM]: #BLCM "Women Manufacturing AGC Rope Core"
[A02]: #B02 "IBM System 360 Model 20 Specs"
[A3]: #B3 "Random Page of Reliability Report"

<br>

References | &nbsp;
:--- | :--- 
<a name="B1"></a>01 | Apple, Jr., R.W. &nbsp; [Whole Book 'Apollo Guidance Computer Architecture and Operation'](ftp://ssh.esac.esa.int/pub/ekuulker/Apollo15/The-Apollo-Guidance-Computer-Architecture-and-Operation.pdf) (Transcript of the recording of a meeting between President Nixon and H. R. Haldeman). Watergate.info website. June 23, 1972. Retrieved January 17, 2007.
<a name="BLCM"></a>02 | [IBM System 360 Model 20 Specs](https://en.wikipedia.org/wiki/IBM_System/360_Model_20) &nbsp; narrative by R.W. Apple, Jr.; chronology by Linda Amster; general ed.: Gerald Gold. (1973). The Watergate hearings: break-in and cover-up; proceedings. New York: Viking Press. 
<a name="B02"></a>03 | Kilpatrick, Carroll (November 18, 1973) &nbsp; [Women Manufacturing AGC Rope Core](https://youtu.be/YIBhPsyYCiM)
<a name="B3"></a>04 | Dean, John W. The Nixon Defense: What He Knew and When He Knew It, pp. 610–620, Penguin Group, 2014 &nbsp; [Random Page of Reliability Report](https://www.ibiblio.org/apollo/klabs/history/history_docs/r713.pdf?#page=39) 

<!-- I found table breaks without a table head with characters in both cells, so I am trying different approach  -->

<br>

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris vel velit eget elit tempor tristique nec sed leo. Vivamus commodo nisl tellus, lobortis imperdiet nisl consequat in. Sed tellus ex, laoreet eu dapibus sed, malesuada imperdiet diam. Nunc eu rutrum dui. Nam ut turpis neque. Mauris at nulla faucibus, ullamcorper dolor in, tincidunt ante. Quisque consequat ullamcorper quam, quis ullamcorper sapien sollicitudin eu. Curabitur mattis ipsum et elit semper sollicitudin. Cras ut eros vitae tellus pharetra commodo. Donec blandit sagittis purus ac commodo. Curabitur fermentum suscipit odio, ac pellentesque ipsum auctor eu.

<br>

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris vel velit eget elit tempor tristique nec sed leo. Vivamus commodo nisl tellus, lobortis imperdiet nisl consequat in. Sed tellus ex, laoreet eu dapibus sed, malesuada imperdiet diam. Nunc eu rutrum dui. Nam ut turpis neque. Mauris at nulla faucibus, ullamcorper dolor in, tincidunt ante. Quisque consequat ullamcorper quam, quis ullamcorper sapien sollicitudin eu. Curabitur mattis ipsum et elit semper sollicitudin. Cras ut eros vitae tellus pharetra commodo. Donec blandit sagittis purus ac commodo. Curabitur fermentum suscipit odio, ac pellentesque ipsum auctor eu.

<!---
Publish: preview
Categories: collaboration
Topics: projects and organizations
Tags: bssw-blog-article
Level: 2
Prerequisites: default
Aggregate: none
--->