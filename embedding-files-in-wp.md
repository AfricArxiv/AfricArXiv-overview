# How to embed files and sheets into the wp website

# Google Doc/Sheet
- https://support.google.com/docs/answer/183965?co=GENIE.Platform%3DDesktop&hl=en

## Changing the size of the spreadsheets embeds on AfricArxiv's WordPress website

Spreadheets embeds are iframe.
You can simply change their size by applying the CSS property "height" to them.

For that, go to Appearence > Customise  and add the following code.

<code>
iframe {
    height: 10rem;
}
</code>


To avoid changing the size of all the iframes on the site, even those that are not spreadheets embeds, you need to add to the CSS rule a selector that allows you to change only the size of the desired iframes.

For example, one could identify a specific CSS class on a page containing the embed and add it to the CSS rule.

For example, we could have, 

<code>
.page-id-1237 iframe {
    height: 10rem;
}
</code>

Thus, only the iframe on the page with the class .page-id-1237 will have its size changed.


