# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Hugo static site using the "Jane" theme. The site is configured to be served locally during development and appears to be part of a GitHub Pages setup (based on the parent directory structure).

## Development Commands

- **Start development server**: `hugo server` or `hugo serve`
- **Build the site**: `hugo` (outputs to `public/` directory)
- **Create new content**: `hugo new content/post/filename.md`

## Architecture

- **Configuration**: `hugo.toml` contains the main site configuration including theme settings, menu structure, and parameters
- **Content**: Markdown files are stored in `content/post/` organized by category (`demo/`, `docs/`, `other/`)
- **Theme**: Uses the "Jane" Hugo theme located in `themes/jane/`
- **Assets**: Site-specific assets in `assets/` directory with JavaScript configuration in `assets/jsconfig.json`
- **Archetypes**: Default content templates in `archetypes/default.md`

## Content Structure

- Posts are organized in `content/post/` with subdirectories for different categories
- Default archetype creates posts with date, draft status, and title front matter
- The site supports both English and Chinese content (hasCJKLanguage enabled)

## Theme Configuration

- Theme path resolution configured in `assets/jsconfig.json` to reference theme assets
- Custom CSS and JS can be added via the `customCSS` and `customJS` parameters in `hugo.toml`
- Social links, author information, and site parameters are configured in the `[params]` section

## Build Output

- Generated site files go to `public/` directory
- Resource cache stored in `resources/` directory