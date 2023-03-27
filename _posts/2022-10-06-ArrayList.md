---
keywords: fastai
title: ArrayList
toc: false
badges: true
comments: true
author: Calissa
categories: [java, labs]
image: images/arrayList.png
nb_path: _notebooks/2022-10-06-ArrayList.ipynb
layout: notebook
---

<!--
#################################################
### THIS FILE WAS AUTOGENERATED! DO NOT EDIT! ###
#################################################
# file to edit: _notebooks/2022-10-06-ArrayList.ipynb
-->

<div class="container" id="notebook-container">
        
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Arrays">Arrays<a class="anchor-link" href="#Arrays"> </a></h3><p>Can hold any datatype (ex: primitives or objects) but have fixed size</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="ArrayList">ArrayList<a class="anchor-link" href="#ArrayList"> </a></h3><p>Can only hold objects but you can change their size. Can get around the limitation of datatypes by using a wrapper class of whatever primitive data type you want to put (ex: Integer for int)</p>
<p>They're kind of like a wrapper around Java's arrays that make them easier to use</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-java"><pre><span></span><span class="kn">import</span> <span class="nn">java.util.Arrays</span><span class="p">;</span>
<span class="kn">import</span> <span class="nn">java.util.ArrayList</span><span class="p">;</span> 

<span class="kd">public</span> <span class="kd">class</span> <span class="nc">ArrayVArrayList</span> <span class="p">{</span> 

    <span class="kd">public</span> <span class="kd">static</span> <span class="kt">void</span> <span class="nf">main</span><span class="p">(</span><span class="n">String</span><span class="o">[]</span> <span class="n">args</span><span class="p">){</span>

        <span class="c1">//Declaring an Array</span>
        <span class="c1">// Also can do: String[] scrumArray = new String[4]; //initializes string array and must give size</span>
                    <span class="c1">// ^^ all 4 elements are null until they are set</span>

        <span class="n">String</span><span class="o">[]</span> <span class="n">scrumArray</span> <span class="o">=</span> <span class="p">{</span><span class="s">&quot;Calissa&quot;</span><span class="p">,</span> <span class="s">&quot;Evan&quot;</span><span class="p">,</span> <span class="s">&quot;Kian&quot;</span><span class="p">,</span> <span class="s">&quot;Samuel&quot;</span><span class="p">};</span> <span class="c1">//initializes values right away, size is implied</span>

        <span class="c1">//Declaring an ArrayList</span>
        <span class="c1">// Also can do: ArrayList&lt;String&gt; scrumArrayList = new ArrayList&lt;&gt;(); //instantiate arraylist, must declare datatype, uses diamond (&lt;&gt;) operator  </span>

        <span class="n">ArrayList</span><span class="o">&lt;</span><span class="n">String</span><span class="o">&gt;</span> <span class="n">scrumArrayList</span> <span class="o">=</span> <span class="k">new</span> <span class="n">ArrayList</span><span class="o">&lt;&gt;</span><span class="p">(</span><span class="n">Arrays</span><span class="p">.</span><span class="na">asList</span><span class="p">(</span><span class="s">&quot;Calissa&quot;</span><span class="p">,</span> <span class="s">&quot;Evan&quot;</span><span class="p">,</span> <span class="s">&quot;Kian&quot;</span><span class="p">,</span> <span class="s">&quot;Samuel&quot;</span><span class="p">));</span> <span class="c1">//passes .asList method (values you want to have in your arrayList)</span>

        <span class="c1">//Getting value from Array</span>
        <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="n">scrumArray</span><span class="o">[</span><span class="mi">1</span><span class="o">]</span><span class="p">);</span>

        <span class="c1">//Getting value from Array</span>
        <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="n">scrumArrayList</span><span class="p">.</span><span class="na">get</span><span class="p">(</span><span class="mi">1</span><span class="p">));</span>

        <span class="c1">//Getting length from Array</span>
        <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="n">scrumArray</span><span class="p">.</span><span class="na">length</span><span class="p">);</span> <span class="c1">//field on array</span>

        <span class="c1">//Getting length from ArrayList</span>
        <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="n">scrumArrayList</span><span class="p">.</span><span class="na">size</span><span class="p">());</span> <span class="c1">//size is method call</span>

        <span class="c1">//Adding element to end of ArrayList</span>
        <span class="n">scrumArrayList</span><span class="p">.</span><span class="na">add</span><span class="p">(</span><span class="s">&quot;John&quot;</span><span class="p">);</span> <span class="c1">//calls add method, pass element you want to add</span>
        <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="n">scrumArrayList</span><span class="p">.</span><span class="na">get</span><span class="p">(</span><span class="mi">4</span><span class="p">));</span>

        <span class="c1">//Change element in Array</span>
        <span class="n">scrumArray</span><span class="o">[</span><span class="mi">1</span><span class="o">]</span> <span class="o">=</span> <span class="s">&quot;Hassan&quot;</span><span class="p">;</span>
        <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="n">scrumArray</span><span class="o">[</span><span class="mi">1</span><span class="o">]</span><span class="p">);</span>

        <span class="c1">//Change element in ArrayList</span>
        <span class="n">scrumArrayList</span><span class="p">.</span><span class="na">set</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span> <span class="s">&quot;Hassan&quot;</span><span class="p">);</span>
        <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="n">scrumArrayList</span><span class="p">.</span><span class="na">get</span><span class="p">(</span><span class="mi">1</span><span class="p">));</span>

        <span class="c1">//Remove element in ArrayList</span>
        <span class="cm">/*</span>
<span class="cm">         * Note: Can also do scrumArrayList.remove(&quot;ObjectName&quot;);</span>
<span class="cm">         */</span>

        <span class="n">scrumArrayList</span><span class="p">.</span><span class="na">remove</span><span class="p">(</span><span class="mi">1</span><span class="p">);</span>
        <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="n">scrumArrayList</span><span class="p">.</span><span class="na">get</span><span class="p">(</span><span class="mi">1</span><span class="p">));</span>

        <span class="c1">//Print Array</span>
        <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="n">scrumArray</span><span class="p">);</span> <span class="c1">//gives memory address</span>

        <span class="c1">//^^In order to print array you have to do a for loop and iterate over all elements</span>

        <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="n">scrumArrayList</span><span class="p">);</span> <span class="c1">//implemented two string method so it prints out nicely</span>


<span class="p">}</span>

<span class="p">}</span>

<span class="n">ArrayVArrayList</span><span class="p">.</span><span class="na">main</span><span class="p">(</span><span class="kc">null</span><span class="p">);</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>Evan
Evan
4
4
John
Hassan
Hassan
Kian
[Ljava.lang.String;@438de3d0
[Calissa, Kian, Samuel, John]
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

</div>
 
