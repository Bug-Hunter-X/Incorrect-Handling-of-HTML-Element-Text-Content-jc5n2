# Uncommon HTML Bug: Text Content Handling

This repository demonstrates a subtle but important bug related to accessing and manipulating the text content of HTML elements, specifically when those elements contain HTML tags within them.  The common mistake revolves around the misuse of `textContent` when only the plain text is desired.

## The Problem

The `textContent` property returns *all* text content, including text within HTML tags.  This can lead to unexpected results when you only want the visible text for the user.

## The Solution

Use `innerText` to get only the rendered text content, excluding any text nested within HTML tags.