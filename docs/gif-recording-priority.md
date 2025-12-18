# GIF Recording Priority Guide

This guide outlines the most valuable GIFs to record for IBO Studio documentation, prioritized by impact and user needs.

## 🎯 Priority 1: Core Editor Workflows (Start Here)

### 1.1 Drag & Drop Components
**File:** `editor/drag-drop-basics.gif`
**Duration:** 8-10 seconds
**What to show:**
1. Open empty canvas
2. Click "+" button in component tree
3. Select a Button component
4. Drag from component list to canvas
5. Position component by dragging on canvas
6. Show component appears on phone preview

### 1.2 Properties Panel Configuration
**File:** `editor/properties-panel-config.gif`
**Duration:** 10 seconds
**What to show:**
1. Select a component on canvas
2. Properties panel slides out from right
3. Change text/label property - see instant update
4. Change color/styling property
5. Toggle a boolean property (like "required")
6. Show how changes appear on phone preview

### 1.3 Component Tree Navigation
**File:** `editor/component-tree-navigation.gif`
**Duration:** 8 seconds
**What to show:**
1. Click on component in tree (highlight on canvas)
2. Click on canvas component (highlight in tree)
3. Expand/collapse parent components
4. Show hierarchical structure (form with child fields)

## 📱 Priority 2: Component Usage (Most Impact)

### 2.1 TextField with Keyboard Types
**File:** `components/textfield-keyboard-types.gif`
**Duration:** 12 seconds
**What to show:**
1. Add TextField component
2. Set keyboard: "text" → show normal keyboard
3. Change to "email" → show email keyboard
4. Change to "number" → show number keyboard
5. Change to "phone" → show phone keyboard

### 2.2 Dropdown Data Binding
**File:** `components/dropdown-data-binding.gif`
**Duration:** 15 seconds
**What to show:**
1. Add Dropdown component
2. Configure static options in properties
3. Switch to data binding mode
4. Connect to existing data source
5. Map value/label keys
6. Show dropdown populated with real data

### 2.3 FormGrid Multi-Column Layout
**File:** `components/formgrid-responsive.gif`
**Duration:** 10 seconds
**What to show:**
1. Add FormGrid component
2. Set columns: 1 → see single column
3. Change to columns: 2 → see responsive layout
4. Add different field types to grid
5. Show how it adapts to phone screen

### 2.4 DateField Picker Interaction
**File:** `components/datefield-picker.gif`
**Duration:** 10 seconds
**What to show:**
1. Add DateField component
2. Click to open date picker
3. Navigate months/days
4. Select date
5. Show selected date in field
6. Optional: Switch to datetime mode

### 2.5 TabContainer Navigation
**File:** `components/tabcontainer-navigation.gif`
**Duration:** 8 seconds
**What to show:**
1. Add TabContainer component
2. Configure multiple tabs with content
3. Click between tabs
4. Show content switching
5. Optional: Swipe gesture on mobile

## 🔗 Priority 3: Data & State Management

### 3.1 Connecting Data Sources
**File:** `workflows/connect-data-source.gif`
**Duration:** 15 seconds
**What to show:**
1. Open Data Sources panel (database icon)
2. Click "Add Data Source"
3. Configure MySQL/PostgreSQL connection
4. Enter credentials and test connection
5. Select tables/views
6. Save data source

### 3.2 State Binding Example
**File:** `workflows/state-binding-calculation.gif`
**Duration:** 12 seconds
**What to show:**
1. Add two number TextFields
2. Add TextField for result (readOnly)
3. Configure onChange calculation: `field1 + field2`
4. Type numbers in first two fields
5. Show result updates automatically

### 3.3 Form Submission with API
**File:** `workflows/form-submit-api.gif`
**Duration:** 15 seconds
**What to show:**
1. Create form with multiple fields
2. Add Submit button
3. Configure submit action with URL and method
4. Fill out form
5. Click submit
6. Show success/error handling

## 🎨 Priority 4: Advanced Features

### 4.1 Version History & Restore
**File:** `editor/version-history-restore.gif`
**Duration:** 12 seconds
**What to show:**
1. Click history icon (clock)
2. View list of published versions
3. Click on older version
4. Preview JSON in right panel
5. Click "Restore" and confirm
6. Show app reverts to previous state

### 4.2 JSON Code View Editing
**File:** `editor/json-code-editing.gif`
**Duration:** 10 seconds
**What to show:**
1. Switch to Code view (</> icon)
2. Show JSON structure
3. Edit a property value in JSON
4. Switch back to Tree view
5. Show changes reflected in UI

### 4.3 SearchBar with Filtering
**File:** `components/searchbar-filtering.gif`
**Duration:** 10 seconds
**What to show:**
1. Add SearchBar component
2. Add List component below it
3. Configure search state key on both
4. Type in search bar
5. Show list filtering in real-time

## 📋 Priority 5: Complete Workflows

### 5.1 Create Complete Contact Form
**File:** `workflows/complete-contact-form.gif`
**Duration:** 25 seconds
**What to show:**
1. Start with empty canvas
2. Add FormGrid
3. Add name, email, phone fields
4. Add submit button
5. Configure validation
6. Test form interaction
7. Connect to API for submission

### 5.2 Product Catalog with Images
**File:** `workflows/product-catalog-cards.gif`
**Duration:** 20 seconds
**What to show:**
1. Add ExpandableCardList
2. Connect to product data source
3. Configure card fields (title, subtitle, image)
4. Add search functionality
5. Test card expansion
6. Add action buttons

### 5.3 Multi-Screen App with Navigation
**File:** `workflows/multi-screen-navigation.gif`
**Duration:** 18 seconds
**What to show:**
1. Configure Navigation Bar tabs
2. Create multiple screens
3. Add different components to each screen
4. Switch between screens via tabs
5. Show navigation state persistence

## 🛠 Recording Guidelines

### Technical Settings
- **Resolution:** 1280x720 (good balance of quality/size)
- **Frame Rate:** 10-15 fps
- **Cursor:** Always visible, highlight clicks
- **Audio:** None needed (GIFs are silent)

### Content Guidelines
- **Focus:** One clear workflow per GIF
- **Pacing:** Slow enough to follow, fast enough to engage
- **Context:** Show before/after states clearly
- **Errors:** If showing error states, make them obvious
- **Success:** Always end on positive outcome

### Optimization Targets
- **Max Duration:** 15 seconds (aim for 8-12 seconds)
- **Max File Size:** 3-5MB per GIF
- **Tools:** ScreenToGif (Windows), Kap (Mac), ezgif.com (compress)

## 📊 Impact Assessment

**High Impact (Record First):**
- Drag & drop basics
- Properties panel usage
- TextField keyboards
- Dropdown data binding
- Form submission workflow

**Medium Impact:**
- Component tree navigation
- Date picker interaction
- Tab navigation
- Data source connection
- State calculations

**Low Impact (Nice to Have):**
- Version history
- JSON editing
- Advanced styling
- Complex layouts

## 🎬 Recording Checklist

For each GIF:
- [ ] Clear starting state shown
- [ ] Cursor movements smooth and visible
- [ ] All clicks/text entry captured
- [ ] End state clearly demonstrates success
- [ ] No distractions in background
- [ ] Compressed to under 5MB
- [ ] Named descriptively with hyphens
- [ ] Tested in documentation markdown

Start with Priority 1 GIFs to quickly improve documentation usability!
