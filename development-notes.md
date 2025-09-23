# GopherWood 3D Loader - Development Notes

## Current Status: 85% Complete

### Working Features
- ✅ Three.js 3D scene with proper lighting and shadows
- ✅ Aluminum trailer visualization (48' and 53' options)
- ✅ Systematic loading logic - bundles snap to proper rows
- ✅ Real bundle dimensions (47"×47"×72" pickets, 42"×17"×96" posts/runners)
- ✅ 200 bundles each type in organized yard stacks
- ✅ Visual feedback (bundles turn green when over trailer)
- ✅ Inventory tracking and management
- ✅ Left/right side positioning (Z: -2, +2)

### Critical Issues to Fix
- ❌ Second layer stacking detection broken - bundles won't stack on top of each other
- ❌ Camera rotation controls not working - right-click + drag should orbit view

## Technical Architecture
- **Framework**: Three.js r128
- **Rendering**: WebGL with shadow mapping
- **Interaction**: Raycasting for mouse controls
- **Positioning**: Systematic row-based loading from trailer front (position 0)

## Loading Logic Details
- **Pickets**: 6-foot rows from front of trailer
- **Posts/Runners**: 8-foot rows from front of trailer
- **Stacking**: 2 high max for pickets, 5 high max for posts/runners
- **Height limit**: 8 feet above trailer deck

## Development Phases

### Phase 1: Foundation (Complete)
- Three.js scene setup
- Trailer modeling with stake pockets and DOT bumper
- Bundle creation system
- Mouse interaction framework

### Phase 2: Loading Logic (85% Complete)
- Systematic row positioning implemented
- Bundle snapping to proper positions
- Visual feedback system
- Left/right side positioning

### Phase 3: Remaining Work
- Fix stacking detection for second layer
- Implement camera rotation controls
- Test full capacity loading scenarios

## Known Technical Issues
1. **Stacking Detection**: `findStackingPosition()` function not detecting existing bundles properly
2. **Camera Controls**: Right-click drag event conflicts with bundle selection
3. **Event Handling**: Mouse event listeners may be interfering with each other

## Next Steps
1. Debug stacking logic - bundles should detect others within 2-3 feet
2. Separate camera rotation from bundle interaction events
3. Test mixed load scenarios (17 pickets + 8 posts + 14 runners)
4. Verify all 39 bundles can load on 53' trailer

## Console Debug Messages
- Green text shows successful loading actions
- Bundle positioning coordinates logged
- Inventory updates tracked in real-time
- Error messages for stacking failures

## File Structure
- `index.html` - Main application
- `versions/backup-v2.html` - Working backup before final fixes
