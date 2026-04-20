# Page background

Block name: Page background
Purpose: background for the page
HTML element candidate: element
Parent: main
Children: Profile card
Layout role: Just a color
Visual role: dark background
Responsive notes: background should fill viewport height and keep card centered on all sizes.
Accessibility note: ensure contrast between background and card/text is readable.

# Profile card

Block name: Profile card
Purpose: groups profile info and links
HTML element candidate: section or article
Parent: Page background
Children: avatar, texts, link list
Layout role: vertical stack
Visual role: dark surface, rounded corners, padding
Responsive notes: width should adapt, max width on desktop
Accessibility note: semantic heading and links

# Avatar image

Block name: Avatar image
Purpose: A picture of the user
HTML element candidate: element ( img )
Parent: Profile card
Children: N/A
Layout role: at the top of the Profile Card
Visual role: a circle placeholder page
Responsive notes: N/A
Accessibility note: N/A

# Name

Block name: Name
Purpose: giving the user name
HTML element candidate: element (Header)
Parent: Profile card
Children: N/A
Layout role: After the Avatar Image
Visual role: Color (white or a bright gray)
Responsive notes: N/A
Accessibility note: N/A

# Location

Block name: Location
Purpose: Providing the Address of the user
HTML element candidate: element (header)
Parent: Profile card
Children: N/A
Layout role: After the Name
Visual role: Green , the font should be bold
Responsive notes: N/A
Accessibility note: N/A

# Bio text

Block name: Bio text
Purpose: giving the Bio of a user (describtion)
HTML element candidate: element (pargraph)
Parent: Profile card
Children: N/A
Layout role: After the Location
Visual role: Color (gray)
Responsive notes: N/A
Accessibility note: N/A

# Social link buttons

Block name: Social link buttons
Purpose: listing the social links
HTML element candidate: list
Parent: Profile card
Children: GitHub, Frontend Mentor, LinkedIn, Twitter, Instagram.
Layout role: After the Bio text and it should be listed vertically
Visual role: listed vertically , background of each child should be as the Bio text color and the font of each button should be as the name font color , rectagular edge with rounded edges.
Responsive notes: hover and foucs the childern ( buttons well turn to a green background) like the Location font color and the font color well be as the main background color
Accessibility note: links

---

# Better Visual Blocks (Professional Version)

Use this as your refined reference. Keep your original version above for learning comparison.

## 1) Page Background

Block name: Page background
Purpose: provide contrast and center the main card in the viewport
HTML element candidate: body (with main inside)
Parent: none (top document layer)
Children: main page container
Layout role: full-page container that centers content
Visual role: dark base color to separate foreground card
Responsive notes: should work from 320px up to large desktop widths; card remains centered
Accessibility note: maintain strong contrast between text/card and background

## 2) Main Content Wrapper

Block name: Main content wrapper
Purpose: define the main region of the page for semantic structure
HTML element candidate: main
Parent: body
Children: profile card
Layout role: single-child layout container
Visual role: usually transparent (layout-only block)
Responsive notes: internal padding prevents card from touching screen edges on small devices
Accessibility note: helps screen readers identify primary page content

## 3) Profile Card

Block name: Profile card
Purpose: group all profile information and actions into one component
HTML element candidate: article (or section)
Parent: main
Children: avatar, name, location, bio, social links list
Layout role: vertical stack with consistent spacing
Visual role: elevated dark surface with rounded corners and internal padding
Responsive notes: fluid width with a max-width cap for desktop readability
Accessibility note: contains one clear heading and meaningful interactive links

## 4) Avatar Image

Block name: Avatar image
Purpose: identify the person visually
HTML element candidate: img
Parent: profile card
Children: none
Layout role: top visual anchor of the card
Visual role: fixed square size displayed as a circle
Responsive notes: size remains stable across breakpoints unless explicitly adjusted
Accessibility note: use descriptive alt text (example meaning: person portrait)

## 5) Name

Block name: Name
Purpose: primary identity text
HTML element candidate: h1
Parent: profile card
Children: none
Layout role: first text block after avatar
Visual role: highest emphasis text in the card
Responsive notes: maintain clear hierarchy and spacing on all screen sizes
Accessibility note: use as the main heading to support document structure

## 6) Location

Block name: Location
Purpose: secondary profile metadata
HTML element candidate: p
Parent: profile card
Children: none
Layout role: appears immediately after name
Visual role: accent text (green) with stronger weight than body copy
Responsive notes: keep readable at narrow widths without wrapping awkwardly
Accessibility note: text must remain readable with sufficient contrast

## 7) Bio Text

Block name: Bio text
Purpose: short descriptive summary of the person
HTML element candidate: p
Parent: profile card
Children: none
Layout role: supporting copy between profile info and action links
Visual role: medium-contrast paragraph text with comfortable line-height
Responsive notes: ensure natural wrapping and no overflow on mobile
Accessibility note: avoid low-contrast gray that reduces readability

## 8) Social Links Group

Block name: Social links group
Purpose: list navigation actions to external social profiles
HTML element candidate: ul containing li > a
Parent: profile card
Children: GitHub, Frontend Mentor, LinkedIn, Twitter, Instagram links
Layout role: vertical list of equal-width interactive items
Visual role: each link styled like a button with consistent height, radius, and spacing
Responsive notes: full-width links inside card; spacing remains consistent on mobile and desktop
Accessibility note: each item is a real anchor link with visible focus state for keyboard users

## 9) Interaction States (Cross-Block Behavior)

Block name: Link interaction states
Purpose: provide feedback for pointer and keyboard users
HTML element candidate: anchor pseudo-classes (hover, focus-visible, active)
Parent: social links group
Children: none
Layout role: no layout change required
Visual role: hover and focus invert colors (green background + dark text)
Responsive notes: behavior should be consistent across all viewport sizes
Accessibility note: focus-visible must be obvious and not removed
