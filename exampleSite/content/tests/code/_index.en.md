+++
description = "Some testing for different styles used in syntax highlighting and preformatted blocks"
title = "Code"
+++

Some testing for different styles used in syntax highlighting and preformatted blocks.

## Inline Code

`This is some very long inline code. Where does it wrap?`

What about wrapping short inline code if multiple sections are written `side` `by` `side`?

What about wrapping short inline code if multiple sections are written `side`/`by`/`side`?

What about wrapping long inline code if multiple sections are written `side567` `by34567` `side567`?

What about wrapping long inline code if multiple sections are written `side567`/`by34567`/`side567`?

Can we just use a <code>simple HTML element </code>?

## Block Code

````
Code fences without any selected language
````

````json
{
  "well": "some JSON in codefences in here"
}
````

<pre><code>{
  "well": "some JSON in HTML elements here"
}
</code></pre>

````jsonxmylmsl
{
  "well": "Code fences with non existing language"
}
````

## Block Preformatted

    Some preformatted stuff with markdown indentation

<pre>
Some preformatted stuff in HTML elements
</pre>

## Nested Shortcode

### 1 Shortcode

#### %%

{{% highlight json "linenos=inline,hl_lines=1 2,anchorlinenos=true" %}}
{
  "Hello": "World" "Hello": "World" "Hello": "World"
}
{{% /highlight %}}

#### <>

{{< highlight json "linenos=table,hl_lines=1 2,anchorlinenos=true" >}}
{
  "Hello": "World" "Hello": "World" "Hello": "World"
}
{{< /highlight >}}

### 2 Shortcodes

#### %% %%

{{% tab title="json" %}}
{{% highlight html "linenos=table,hl_lines=1 2,anchorlinenos=true" %}}
{
  "Hello": "World" "Hello": "World" "Hello": "World"
}
{{% /highlight %}}
{{% /tab %}}

#### %% <>

{{% tab title="json" %}}
{{< highlight html "linenos=table,hl_lines=1 2,anchorlinenos=true" >}}
{
  "Hello": "World" "Hello": "World" "Hello": "World"
}
{{< /highlight >}}
{{% /tab %}}

#### <> %%

{{< tab title="json" >}}
{{% highlight html "linenos=table,hl_lines=1 2,anchorlinenos=true" %}}
{
  "Hello": "World" "Hello": "World" "Hello": "World"
}
{{% /highlight %}}
{{< /tab >}}

#### <> <>

{{< tab title="json" >}}
{{< highlight html "linenos=table,hl_lines=1 2,anchorlinenos=true" >}}
{
  "Hello": "World" "Hello": "World" "Hello": "World"
}
{{< /highlight >}}
{{< /tab >}}

### 3 Shortcodes

#### %% %% %%

{{% tabs %}}
{{% tab title="json" %}}
{{% highlight html "linenos=table,hl_lines=1 2,anchorlinenos=true" %}}
{
  "Hello": "World" "Hello": "World" "Hello": "World"
}
{{% /highlight %}}
{{% /tab %}}
{{% /tabs %}}

#### %% %% <>

{{% tabs %}}
{{% tab title="json" %}}
{{< highlight html "linenos=table,hl_lines=1 2,anchorlinenos=true" >}}
{
  "Hello": "World" "Hello": "World" "Hello": "World"
}
{{< /highlight >}}
{{% /tab %}}
{{% /tabs %}}

#### %% <> %%

{{% tabs %}}
{{< tab title="json" >}}
{{% highlight html "linenos=table,hl_lines=1 2,anchorlinenos=true" %}}
{
  "Hello": "World" "Hello": "World" "Hello": "World"
}
{{% /highlight %}}
{{< /tab >}}
{{% /tabs %}}

#### %% <> <>

{{% tabs %}}
{{< tab title="json" >}}
{{< highlight html "linenos=table,hl_lines=1 2,anchorlinenos=true" >}}
{
  "Hello": "World" "Hello": "World" "Hello": "World"
}
{{< /highlight >}}
{{< /tab >}}
{{% /tabs %}}

#### <> %% %%

{{< tabs >}}
{{% tab title="json" %}}
{{% highlight html "linenos=table,hl_lines=1 2,anchorlinenos=true" %}}
{
  "Hello": "World" "Hello": "World" "Hello": "World"
}
{{% /highlight %}}
{{% /tab %}}
{{< /tabs >}}

#### <> %% <>

{{< tabs >}}
{{% tab title="json" %}}
{{< highlight html "linenos=table,hl_lines=1 2,anchorlinenos=true" >}}
{
  "Hello": "World" "Hello": "World" "Hello": "World"
}
{{< /highlight >}}
{{% /tab %}}
{{< /tabs >}}

#### <> <> %%

{{< tabs >}}
{{< tab title="json" >}}
{{% highlight html "linenos=table,hl_lines=1 2,anchorlinenos=true" %}}
{
  "Hello": "World" "Hello": "World" "Hello": "World"
}
{{% /highlight %}}
{{< /tab >}}
{{< /tabs >}}

#### <> <> <>

{{< tabs >}}
{{< tab title="json" >}}
{{< highlight html "linenos=table,hl_lines=1 2,anchorlinenos=true" >}}
{
  "Hello": "World" "Hello": "World" "Hello": "World"
}
{{< /highlight >}}
{{< /tab >}}
{{< /tabs >}}
