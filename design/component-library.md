# Component Library Specification

This document details the core components for the Auctio web and mobile apps. Components should be built in Figma with variants for state management and responsive behavior. Use Auto Layout, constraints, and design tokens defined in the UI/UX concept.

## Buttons
| Variant | Usage | States | Notes |
| --- | --- | --- | --- |
| Primary | High-emphasis actions like "Jetzt mitbieten" | default, hover, focus, pressed, disabled | Gradient background, white text, drop shadow `0 12px 24px rgba(255,90,60,0.25)` |
| Secondary | Supporting actions like "Zur Wunschliste" | default, hover, focus, pressed | `brand-secondary` outline, transparent fill |
| Tertiary | Text button links | default, hover | Use `brand-secondary` text, underline on hover |
| Icon | Quick actions (favorite, share) | default, hover, active | 44px circle, 2px stroke icons |

## Navigation
### Top App Bar (Web)
- Left: logo, "Auctio" wordmark.
- Center: search bar with category dropdown, quick filters.
- Right: profile avatar dropdown, alerts bell with badge, "Verkaufen" button.
- Scroll behavior: elevate with shadow after 16px scroll.

### Bottom Navigation (Mobile)
Tabs: Home, Suchen, Verkaufen (accented), Alerts, Profil. Use dynamic badges for alerts.

## Cards
| Card | Layout | Highlights |
| --- | --- | --- |
| Auction card | Image (3:2), title, location chip, current bid, timer pill | Hover reveals quick bid + watchlist icons |
| Category capsule | Minimal icon + label, gradient background | Use in curated collections |
| Story card | Full-bleed background, overlay gradient, CTA "Mehr erfahren" | For community stories |

## Forms & Inputs
- Text fields: 12px radius, inset shadow `0 1px 2px rgba(17,24,39,0.08)`, focus outline `2px brand-secondary`.
- Dropdowns: use bottom sheet on mobile.
- Bid stepper: numeric input with +/− controls, auto-fill increment options.

## Feedback & Status
- Toasts: bottom-right web / bottom mobile, auto-dismiss 4s, manual close icon.
- Modals: 32px radius, blurred background overlay.
- Empty states: friendly illustration, localized copy, CTA to explore listings.

## Data Visualization
- Compact line chart for bid history, 4 data points visible.
- Progress ring for seller checklist completion.
- Heatmap badges for activity ("Hot" auctions).

## Motion Guidelines
- Enter/exit animations < 300ms.
- Use bounce easing for success states, linear for countdown transitions.

## Accessibility Considerations
- All interactive elements labeled in German.
- Provide alt text templates in component descriptions.
- Ensure variants with 4.5:1 contrast ratio.

