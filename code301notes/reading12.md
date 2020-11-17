# Class 12: Components

## EJS Partials

- use **partials** when you want to reuse the same HTML across multiple views.
- sort of like a function, you **define** a reusable piece of code in a file and include it wherever you need it.
- make partical files in a partials subdirectory in your views directory that contain the HTML code you want to reuse.
- use `<%- include( PARTIAL_FILE ) %>` where the partial file is relative to the template you use it in.

[<-- Back](301readingnotes.md) [Back to Home](README.md)