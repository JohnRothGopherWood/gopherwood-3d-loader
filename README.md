# GopherWood 3D Trailer Loading System

## Overview
Professional 3D visualization system for optimal forklift loading of lumber products onto flatbed trailers. Ensures DOT compliance and maximum space utilization.

## Version 10 - Production Ready
- Fixed odd picket reservation system (17th picket loads at rear)
- Corrected lumber stacking patterns for 10+ bundles
- Fixed pickets 9-10 rear positioning logic (only when exactly 10 or with lumber)
- Resolved 18-picket loading bug

## Product Specifications
- **Pickets (6' Dogear)**: 47"×47"×72", 1,400 lbs, 560 pieces/bundle
- **4x4x8 Rough Posts**: 42"×17"×96", 816 lbs, 48 pieces/bundle
- **2x4x8 Rough Runners**: 42"×17"×96", 918 lbs, 108 pieces/bundle

## Key Features
- Systematic row-based loading (6' rows for pickets, 8' rows for lumber)
- Mixed Load Protocol (17 pickets + 7 posts + 7 runners)
- DOT compliance (48,000 lbs max, 13.5' height limit)
- Odd picket reservation system
- Fill gaps first protocol
- Special rear positioning for pickets 9-10

## Loading Patterns
- Pickets: 2×2 stacking pattern (left-bottom, left-top, right-bottom, right-top)
- Lumber: 5 high per side, then new row
- Mixed loads: Pickets → 4x4s → 2x4s → Reserved picket

## Testing Completed
✅ Odd/even picket counts
✅ Lumber balancing (12+ bundles)
✅ Mixed load protocols
✅ Removal/editing functions
✅ Weight/height limits
✅ 48'/53' trailer switching

## Usage
Open `gopherwood-3d-loader-v10-production.html` in any modern web browser.

## Development Notes
- Built with Three.js r128
- Self-contained HTML (no dependencies)
- ~85% production ready
- Tested extensively with real forklift operator feedback

## Author
John Roth - GopherWood Lumber
