---
keywords: fastai
title: Java Conditionals
toc: false
badges: true
comments: true
author: Calissa
categories: [java, labs]
image: images/conditionals.jpeg
nb_path: _notebooks/2022-09-07-conditionals.ipynb
layout: notebook
---

<!--
#################################################
### THIS FILE WAS AUTOGENERATED! DO NOT EDIT! ###
#################################################
# file to edit: _notebooks/2022-09-07-conditionals.ipynb
-->

<div class="container" id="notebook-container">
        
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="If-Else-Statements">If-Else Statements<a class="anchor-link" href="#If-Else-Statements"> </a></h3><p>If-Else statements are conditional statements that determine which section of code to run.</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-java"><pre><span></span><span class="cm">/*</span>
<span class="cm"> Example 1:</span>
<span class="cm"> If condition is not true, else is executed</span>
<span class="cm"> */</span>

<span class="kt">int</span> <span class="n">x</span> <span class="o">=</span> <span class="mi">5</span><span class="p">;</span> <span class="c1">// variable x</span>
<span class="k">if</span> <span class="p">(</span><span class="n">x</span><span class="o">&lt;</span><span class="mi">4</span><span class="p">){</span> <span class="c1">// the line of code within the if statement will not be executed as x is not less than 4</span>
    <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;X is less than 4&quot;</span><span class="p">);</span>
<span class="p">}</span>
<span class="k">else</span> <span class="p">{</span> <span class="c1">// the line of code within the else statement is executed because first condition is not true</span>
    <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;X is greater than 4&quot;</span><span class="p">);</span>
<span class="p">}</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>X is greater than 4
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-java"><pre><span></span><span class="cm">/*</span>
<span class="cm"> Example 2:</span>
<span class="cm"> If condition is true, else is not executed</span>
<span class="cm"> */</span>

<span class="kt">int</span> <span class="n">x</span> <span class="o">=</span> <span class="mi">3</span><span class="p">;</span> <span class="c1">// variable x</span>
<span class="k">if</span> <span class="p">(</span><span class="n">x</span><span class="o">&lt;</span><span class="mi">4</span><span class="p">){</span> <span class="c1">// the line of code within the if statement will be executed as x is less than 4</span>
    <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;X is less than 4&quot;</span><span class="p">);</span>
<span class="p">}</span>
<span class="k">else</span> <span class="p">{</span> <span class="c1">// the line of code within the else statement is not executed because first condition is true</span>
    <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;X is greater than 4&quot;</span><span class="p">);</span>
<span class="p">}</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>X is less than 4
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="If-Elseif-Else-Statements">If-Elseif-Else Statements<a class="anchor-link" href="#If-Elseif-Else-Statements"> </a></h3><p>If-Elseif-Else statements are another conditional statement, this time with 3 different code segments to execute from. Both the if and elseif need a condition, while the else does not.</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-java"><pre><span></span><span class="cm">/*</span>
<span class="cm"> Example 3:</span>
<span class="cm">If condition false, else if condition true. Else if code is executed</span>
<span class="cm"> */</span>

<span class="kt">int</span> <span class="n">x</span> <span class="o">=</span> <span class="mi">2</span><span class="p">;</span> <span class="c1">// variable x</span>
<span class="k">if</span> <span class="p">(</span><span class="n">x</span><span class="o">&lt;</span><span class="mi">4</span> <span class="o">&amp;&amp;</span> <span class="n">x</span><span class="o">&gt;</span><span class="mi">3</span> <span class="p">){</span> <span class="c1">// the line of code within the if statement will not be executed, as x is not between 3 and 4</span>
    <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;X is less than 4&quot;</span><span class="p">);</span>
<span class="p">}</span>
<span class="k">else</span> <span class="k">if</span> <span class="p">(</span><span class="n">x</span> <span class="o">==</span> <span class="mi">2</span><span class="p">){</span> <span class="c1">// the line of code within the else if statement is executed as x is equal to 2</span>
    <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;X is equal to 2&quot;</span><span class="p">);</span>
<span class="p">}</span>
<span class="k">else</span> <span class="p">{</span> <span class="c1">// the line of code within the else statement is not executed because the previous condition is true</span>
    <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;X is greater than 4&quot;</span><span class="p">);</span>
<span class="p">}</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>X is equal to 2
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Switch-case">Switch-case<a class="anchor-link" href="#Switch-case"> </a></h3><p>There are many ways to write code. In the case of conditionals, a switch case can be used to replace a if-elseif-else statement. In a switch statement, one of many code blocks will be executed.</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-java"><pre><span></span><span class="c1">// this is an if-else-else statement</span>
<span class="n">String</span> <span class="n">cheese</span> <span class="o">=</span> <span class="s">&quot;Gouda&quot;</span><span class="p">;</span>
<span class="k">if</span> <span class="p">(</span><span class="n">cheese</span> <span class="o">==</span> <span class="s">&quot;Cheddar&quot;</span><span class="p">){</span> <span class="c1">// tests if cheese = cheddar</span>
    <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;Cheddar originated in Somerset&quot;</span><span class="p">);</span>
<span class="p">}</span>
<span class="k">else</span> <span class="k">if</span> <span class="p">(</span><span class="n">cheese</span> <span class="o">==</span> <span class="s">&quot;Gouda&quot;</span><span class="p">){</span> <span class="c1">// tests if cheese = gouda</span>
    <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;Gouda originated in the Netherlands&quot;</span><span class="p">);</span>
<span class="p">}</span>
<span class="k">else</span> <span class="k">if</span> <span class="p">(</span><span class="n">cheese</span> <span class="o">==</span> <span class="s">&quot;Milk&quot;</span><span class="p">){</span> <span class="c1">// tests if cheese = milk</span>
    <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;Milk is made from cows, goats, and other mammals&quot;</span><span class="p">);</span>
<span class="p">}</span>
<span class="k">else</span> <span class="k">if</span> <span class="p">(</span><span class="n">cheese</span> <span class="o">==</span> <span class="s">&quot;Cheese&quot;</span><span class="p">){</span> <span class="c1">// tests if cheese = cheese</span>
    <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;Cheese is very yummy&quot;</span><span class="p">);</span>
<span class="p">}</span>
<span class="k">else</span><span class="p">{</span> <span class="c1">// if cheese is none of these</span>
    <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;Sorry, I don&#39;t have any information about &quot;</span> <span class="o">+</span> <span class="n">cheese</span><span class="p">);</span>
<span class="p">}</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>Gouda originated in the Netherlands
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-java"><pre><span></span><span class="c1">//the statement above can also be written like:</span>
<span class="n">String</span> <span class="n">cheese</span> <span class="o">=</span> <span class="s">&quot;Gouda&quot;</span><span class="p">;</span>
<span class="k">switch</span><span class="p">(</span><span class="n">cheese</span><span class="p">)</span> <span class="p">{</span>
    <span class="k">case</span> <span class="s">&quot;Cheddar&quot;</span><span class="p">:</span> <span class="c1">// tests if cheese = cheddar</span>
        <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;Cheddar originated in Somerset&quot;</span><span class="p">);</span>
        <span class="k">break</span><span class="p">;</span>
    <span class="k">case</span> <span class="s">&quot;Gouda&quot;</span><span class="p">:</span> <span class="c1">// tests if cheese = gouda</span>
        <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;Gouda originated in the Netherlands&quot;</span><span class="p">);</span>
        <span class="k">break</span><span class="p">;</span>
    <span class="k">case</span> <span class="s">&quot;Milk&quot;</span><span class="p">:</span> <span class="c1">// tests if cheese = milk</span>
        <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;Milk is made from cows, goats, and other mammals&quot;</span><span class="p">);</span>
        <span class="k">break</span><span class="p">;</span>
    <span class="k">case</span> <span class="s">&quot;Cheese&quot;</span><span class="p">:</span> <span class="c1">// tests if cheese = cheese</span>
        <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;Cheese is very yummy&quot;</span><span class="p">);</span>
    <span class="k">default</span><span class="p">:</span> <span class="c1">// if cheese is none of these</span>
        <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;Sorry, I don&#39;t have any information about &quot;</span> <span class="o">+</span> <span class="n">cheese</span><span class="p">);</span>   
<span class="p">}</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>Gouda originated in the Netherlands
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="De-Morgan's-Law">De Morgan's Law<a class="anchor-link" href="#De-Morgan's-Law"> </a></h3><p>De Morgan's Law illustrates how compound boolean expressions are read. It helps you simplify code and your logic operators.</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-java"><pre><span></span><span class="kt">boolean</span> <span class="n">a</span> <span class="o">=</span> <span class="kc">true</span><span class="p">;</span>
<span class="kt">boolean</span> <span class="n">b</span> <span class="o">=</span> <span class="kc">false</span><span class="p">;</span>

<span class="k">if</span> <span class="p">(</span><span class="o">!</span><span class="p">(</span><span class="n">a</span> <span class="o">&amp;&amp;</span> <span class="n">b</span><span class="p">)){</span>
    <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;!(true &amp;&amp; false) is true&quot;</span><span class="p">);</span>
<span class="p">}</span>
<span class="k">else</span> <span class="p">{</span>
    <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;!(true &amp;&amp; false) is false&quot;</span><span class="p">);</span>
<span class="p">}</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>!(true &amp;&amp; false) is true
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

</div>
 
