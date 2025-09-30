# GopherWood 3D Loader - Technical Specifications

## Bundle Dimensions & Weights

### 6' Dogear Pickets
- Dimensions: 47" W × 47" H × 72" L (3.92' × 3.92' × 6')
- Weight: 1,400 lbs per bundle
- Pieces: 560 pickets per bundle
- Stacking: Maximum 2 high
- Loading pattern: 2×2 (2 wide, 2 high per row)

### 4x4x8 Rough Posts
- Dimensions: 42" W × 17" H × 96" L (3.5' × 1.42' × 8')
- Weight: 816 lbs per bundle
- Pieces: 48 posts per bundle
- Stacking: Maximum 5 high

### 2x4x8 Rough Runners
- Dimensions: 42" W × 17" H × 96" L (3.5' × 1.42' × 8')
- Weight: 918 lbs per bundle
- Pieces: 108 runners per bundle
- Stacking: Maximum 5 high

## Loading Algorithms

### Picket Positioning
1. Bundles 1-2: Left side (bottom, top)
2. Bundles 3-4: Right side (bottom, top)
3. Continues in 2×2 pattern front to back
4. Odd picket: Reserved for rear center
5. Pickets 9-10: Rear right for strapping (when exactly 10 or with lumber)

### Lumber Positioning
1. First 5: Left side, stacked vertically
2. Next 5: Right side, stacked vertically
3. Bundles 11-15: Left side, new row
4. Bundles 16-20: Right side, new row
5. Positions tightly against existing bundles

### Mixed Load Protocol
- Standard: 17 pickets + 7 4x4s + 7 2x4s
- Loading sequence: Pickets → 4x4s → 2x4s → Reserved picket
