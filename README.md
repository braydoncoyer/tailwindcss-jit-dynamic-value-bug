After enabling the TailwindCSS JIT compiler in a Next.js project, I created a div with a background color defined by an arbitrary value (bg-[#db1424]). The browser updates and I can see the div with the appropriate color applied. If I try to extract this hex color into a variable and inject it as a classname via template literals, it does not show up in the browser.

The example repo linked to this issue has two divs: one with an arbitrary bg value injected with template literals, and another div with an arbitrary bg value pasted inline. The second div is the only one showing the correct value in the browser.

I've run into weird cases with the dynamically injected color works at times when I tinker with restarting the dev server or changing the hex color, but I can't find a pattern to narrow down the issue.
