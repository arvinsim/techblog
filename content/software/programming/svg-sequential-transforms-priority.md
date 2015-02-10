+++
date = "2015-02-10T20:35:14+08:00"
description = "The SVG transform does not behave as you might expect"
title = "SVG Sequential Transforms Priority"
article-type = ["tip"]
tags = ["svg", "transform"]
+++

When you want to do a series of sequential transforms on an SVG element, keep in mind that it is applied right to left.

In this example, this SVG code does the translate first, then the scaling, then the rotation.

    <g transform="rotate(45) scale(2) translate(100, 100)">

It is counterintuitive but that is how it works.  Hopefully this solves some problems you might have on your SVG transforms.
