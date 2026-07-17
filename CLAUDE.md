# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository overview

Single static HTML page ([index.html](index.html)) — no build system, no package manager, no tests. Open the file directly in a browser to run it; no install/build/lint/test commands exist.

## Architecture

Everything (markup, CSS, JS) lives in the one `index.html` file:
- Inline `<style>` block for styling.
- Inline `<script>` block wires two number `<input>` elements to a live sum displayed in `#sum`, updated on each `input` event.

There is no separation between source and output — edits to `index.html` are the deployable artifact.
