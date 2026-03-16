# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a single-file travel itinerary website for a Japan cycling/rail trip (April 18 – May 14, 2026) for Sam & Jess. There is no build system, package manager, or dependencies — just open `japan_trip_full_itinerary.html` in a browser.

## Architecture

One self-contained HTML file with ~1,100 lines of embedded CSS and no JavaScript. External dependency: Google Fonts CDN (DM Serif Display, DM Sans).

### CSS Design System

CSS custom properties define the visual language:
- **Mode colors:** Cycling `#2E8B57` (green), Train `#3B6FA0` (blue), Flight `#9B5BA5` (purple)
- **Base palette:** Background `#FAF8F4` (cream), text `#2C2A25` (brown)
- **Responsive breakpoint:** 600px

### Content Structure

Each stop follows a consistent template:
1. **Stop card** — header (stop number, city, dates), vibe narrative, data grid, highlights (tag UI), trivia, links
2. **Relocation card** — transport mode, route, duration, cost, step-by-step directions

The itinerary covers 10 stops: Osaka → Kyoto → Onomichi → Ikuchijima → Imabari → Uchiko → Ozu → Matsuyama → Tokyo → Osaka (departure).

### Key Numbers
- 275 km total cycled (Shimanami Kaido is the centerpiece: 75 km across islands; also includes Imabari→Uchiko ~80 km and Ozu→Matsuyama ~58 km)
- 3 train relocations (Kyoto→Onomichi, Matsuyama→Tokyo, Tokyo→Osaka), 1 flight
- Bikes travel in rinko bags (folded/bagged for train transport)
