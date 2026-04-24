**Interaction Design Principles**
- - -
{{TOC}}
- - -

## 📖 Index

1. [Visibility](#visibility)
2. [Feedback](#feedback)
3. [Affordance](#affordance)
4. [Constraint](#constraint)
5. [Mapping](#mapping)
6. [Consistency](#consistency)
7. [Simplicity](#simplicity)
8. [Learnability](#learnability)
9. [User Control](#user-control)
10. [Align Reality](#align-reality)
11. [🎯 Principles in Action — Airbnb Booking Flow](#principles-in-action--airbnb-booking-flow)
12. [Summary](#summary)

- - -

## Visibility

Important actions and information should be obvious at a glance, so users can see what they can do next without hunting. Make possible actions obvious.

**› Applied Example**

*A checkout flow shows a clear stepper: Cart → Address → Payment → Review, so users always know where they are and what’s next.*

**› Not Applied Example**

*Long form submit with no progress indicator; user clicks “Pay” and sees a blank screen for 10s, unsure if payment went through.*

**› More Examples**

| Domain || Example |||
|:--|:--|
| Mobile app UI || A ride‑hailing app shows a live map with car position, ETA chip, and “Driver arriving in 3 min” banner so the user immediately knows what’s happening without digging into menus. |||
| Web form || A multi‑step signup form displays a stepper (1–4) with current step highlighted and disabled future steps, so users can see progress and how many steps remain. |||
| File upload || Cloud storage shows a progress bar with percentage, file name, and a small “Uploading 2 of 5” label, making system status and workload visible at a glance. |||
| Navigation in app || A persistent bottom nav with highlighted active icon (“Home”, “Search”, “Library”) keeps current location and main paths always visible instead of hidden behind a hamburger menu. |||
| Email client UI || An email app’s “Compose” button is a large, high‑contrast floating action button that stays visible on the inbox screen, clearly advertising the primary action. |||
| Industrial product || A washing machine has a ring of LEDs around the main knob plus a simple “Wash → Rinse → Spin → Done” indicator row, so the current phase and remaining steps are visible without opening the door. |||
| Architecture – wayfinding || In an airport, large overhead signs with strong color contrast and arrows show “Arrivals”, “Departures”, and gate ranges from far away, making primary routes visible in long sightlines. |||
| Architecture – safety || Stairwells and exits are marked with illuminated “EXIT” signs and floor‑number markers visible even in low light or smoke, making escape paths obvious under stress. |||
| Public transport || Metro platforms use electronic boards showing line name, destination, time to next trains, and platform number, turning otherwise invisible schedule/state into instantly scannable information. |||
| Product / control panel || An induction cooktop highlights the active zone with a bright indicator and shows the heat level (1–9) next to it, making both which burner is on and how hot it is visible to prevent errors. |||
| Design tool (Figma) || When an object is selected, resize handles, alignment guides, and layer names appear simultaneously — the user sees all possible manipulations at a glance instead of digging into menus. |||
| SaaS dashboard || Stripe's dashboard surfaces KPIs (MRR, churn, new customers) as large-number cards with trend arrows and percentage deltas so the health of the business is visible without opening reports. |||
| Collaborative editor || Google Docs shows each collaborator's cursor with their name and color, making presence and current focus visible in real time instead of hidden. |||
| Chat / messaging || Slack shows an unread count badge on channels, a bold channel name, plus a pulsing "typing…" indicator — you can see activity without opening each conversation. |||
| Version control UI || VS Code's gutter shows a colored bar next to added/modified/deleted lines, and the minimap previews the whole file — giving instant visibility of what's changed and where. |||
| Music streaming || Spotify pins a persistent "Now Playing" bar at the bottom showing track, artist, progress, and controls — so what's playing is never hidden behind navigation. |||
| Video platform || YouTube's progress bar shows chapter markers, buffered amount (lighter shade), and watched portion (red), making all timeline state visible in one compact affordance. |||
| Project management || Linear surfaces issue status as colored dots (Todo, In Progress, Done) and cycle progress as a ring chart — team velocity and blockers are visible without drilling down. |||
| E-commerce || Amazon shows the cart count badge on the cart icon and "Only 3 left in stock" next to items, making both your intent and scarcity visible at decision time. |||
| Notifications UI || iOS shows a grouped stack of notifications with app icon, app name, and time so the user can triage importance in under a second. |||
| Map / navigation app || Google Maps shows live traffic in red/yellow/green overlays and ETA updates in real time as conditions change — route health is visible, not hidden. |||
| Onboarding progress || Duolingo shows a progress bar filling as the user answers each question in a lesson, plus a hearts/lives counter — progress and stakes are always visible. |||
| Form state || A password field shows a live strength meter ("Weak → Strong") plus a list of unmet requirements — what's wrong is visible without pressing submit. |||
| Presentation software || Keynote's slide navigator shows numbered thumbnails of every slide, making the entire deck structure visible from any slide you're editing. |||
| Smart appliance || A smart fridge with a transparent OLED door displays contents and expiry warnings without needing to open it, turning hidden state into visible information. |||
| Public signage || Bus stops with real-time displays show "Route 47 — 3 min" digitally instead of just a static timetable, exposing the invisible schedule state to waiting riders. |||
| Automotive dashboard || Tesla's center screen shows surrounding vehicles, lane lines, and autopilot status as a live visualization — the car's perception is visible to the driver. |||
| Accessibility || macOS VoiceOver cursor draws a black rectangle around the focused element, making screen-reader focus location visible for sighted observers too. |||
| Health tech || Apple Watch workout view shows heart rate, calories, elapsed time, and pace simultaneously in a glanceable layout — all vitals visible without scrolling. |||
| Analytics product || Mixpanel highlights anomalies in time-series charts with automatic annotations, making unusual events visible without manual inspection. |||

- - -

## Feedback

Every user action needs a clear system response (visual, sound, haptic, state change) so users know what is happening in the system. Show clear results of every action.

**› Applied Example**

*Tapping a mobile button gives a ripple, changes state to “Loading…”, then to “Done” with a toast confirmation.*

**› Not Applied Example**

*Tapping “Send” on a contact form does nothing visible; users keep tapping, send duplicates, or abandon.*

**› More Examples**

| Domain || Example |||
|:--|:--|
| Mobile Banking App || After tapping “Transfer”, the app shows a brief loading indicator, then a green check icon with “Transfer successful” and updated balance, confirming the operation and its result. |||
| E-Commerce Checkout || When a user clicks “Add to cart”, the button briefly animates, a mini‑cart count increases, and a small confirmation toast appears, signaling the action worked. |||
| Form Validation UI || A payment form shows inline validation: invalid card number fields turn red with an error message, valid ones turn green with a checkmark, guiding correction in real time. |||
| Messaging App || When a message is sent, a single tick, double tick, and “seen” indicator appear at different stages, plus a subtle sending animation so users know delivery status. |||
| Voice Assistant || On “Hey Google” or similar wake words, animated dots or a pulsing ring appear and move with speech, confirming the device heard and is processing the command. |||
| Household Appliance || A microwave beeps when input is accepted, lights up while running, and gives a distinct series of beeps at the end, clearly signaling state changes to the user. |||
| Automotive Interface || When a driver activates turn signals, a blinking dashboard arrow plus a ticking sound provide visual and auditory feedback that the indicator is on and working. |||
| Industrial Control Panel || Pressing an emergency stop button triggers a mechanical “click”, the button latches down in red, and nearby machines power down with indicator lights changing state, confirming activation. |||
| Architecture/Doors || An automatic sliding door gives feedback with proximity sensor lights and audible motor sound as it opens, so users understand it detected them and is responding. |||
| Public Transport/Ticketing || A metro gate beeps and shows a green arrow with remaining balance when a card is accepted, or a red cross and error message when payment fails, clarifying what happened and what to do next. |||
| Pull-to-refresh || iOS shows an elastic rubber-band stretch plus a spinning indicator as you pull a list down — the physics and spinner together confirm the refresh gesture registered. |||
| Design tool selection || Figma flashes a blue outline the moment an object is clicked, and shows a rubber-band rectangle while drag-selecting — every pointer action has an immediate visual echo. |||
| Copy to clipboard || Clicking "Copy" on a code snippet momentarily changes the button label to "Copied!" with a check icon before reverting — silent clipboard actions are made audible in pixels. |||
| Undo snackbar || Gmail shows an "Undo send" snackbar for 5 seconds after sending an email — feedback about what happened plus a control to reverse it. |||
| Search autocomplete || Google shows query suggestions instantly as you type, with the matched substring bolded — every keystroke produces visible system response. |||
| Drag and drop || Trello highlights the drop zone and shows a ghost placeholder where the card will land as you drag — the system's intent is feedback on yours. |||
| File upload progress || Dropbox shows per-file progress bars, total transfer speed, and estimated time remaining — long operations report progress instead of appearing frozen. |||
| Password strength || A live meter shifts from red → orange → green as the user types, with micro-copy naming what's missing ("Add a number") — feedback before submit, not after. |||
| Like / react animation || Instagram's double-tap triggers a heart burst animation scaled from the tap point — the gesture confirms itself through motion. |||
| Save state indicator || Notion shows "Saving…" then "Saved" in the top-right after edits; Google Docs shows "All changes saved in Drive" — silent autosave is made visible. |||
| Payment processing || Stripe Checkout shows a spinner inside the Pay button, then a green check, then redirects — each state change confirms the flow is advancing. |||
| Haptic feedback || iPhone's Taptic Engine produces a distinct "thunk" when Apple Pay completes — a physical confirmation of a virtual transaction. |||
| Video call || Zoom shows a red "Recording" dot and "You are muted" banner the moment either state changes — meeting state changes produce immediate, persistent feedback. |||
| Typing indicator || iMessage shows "..." bubble when the other person is typing — invisible intent is surfaced as visible feedback. |||
| Merge confirmation || GitHub plays a purple "Merged" animation on a PR and sends an email + in-app notification — major actions get multi-channel feedback. |||
| Bluetooth pairing || macOS shows a pairing dialog with a 6-digit code, vibrates the paired device, and confirms with a "Connected" sound — feedback across both devices. |||
| Form autosave || Linear saves drafts as you type and shows a subtle "Draft saved" pill — work-in-progress is confirmed safe continuously. |||
| Loading skeletons || LinkedIn shows shimmering gray placeholders shaped like the eventual content — feedback that something is coming, not that the app is broken. |||
| Camera shutter || iPhone plays a shutter sound and briefly dims the viewfinder when a photo is taken — a multi-sense confirmation that the image was captured. |||
| Elevator panel || A pressed floor button illuminates, a chime sounds on arrival, and the floor indicator animates through numbers — continuous feedback during a multi-second action. |||
| Mechanical keyboard || Each keypress produces a tactile bump, audible click, and screen character — three layers of feedback on a single action. |||

- - -

## Affordance

Elements should look like how they’re meant to be used (e.g., buttons look clickable, sliders look draggable), with clear cues that invite interaction.

**› Applied Example**

*Primary action is a raised, colored button with label “Place order”; hover and press states reinforce clickability.*

**› Not Applied Example**

*Brand makes all CTAs flat text in body color; users don’t realise they’re clickable links, like a “Norman door” of UI.*

**› More Examples**

| Domain || Example |||
|:--|:--|
| Mobile primary button || A raised, colored rectangle with label “Continue” and a drop shadow looks pressable, clearly affording tapping to move forward in the flow. |||
| Hyperlinks on Web || Underlined, colored text inside a paragraph visually distinguishes itself from body copy, affording that it can be clicked to navigate. |||
| Slider control || A horizontal track with a circular thumb suggests dragging left/right to change volume or brightness, mirroring physical sliders. |||
| Text input field || A bordered, empty rectangle with a cursor blinking inside it affords typing; placeholder text “Search” reinforces the action. |||
| Drag-and-drop area || A dashed rectangle with an icon of a file and label “Drop files here to upload” visually and verbally affords dragging files onto it. |||
| Door hardware (industrial) || A horizontal push plate on one side of a door and a vertical pull bar on the other side shape how people interact: plate affords pushing, bar affords pulling. |||
| Car interior controls || A knurled knob on a dashboard affords twisting to adjust volume or temperature more than pushing, due to its cylindrical form and texture. |||
| Public Seating || A wide, flat bench at sitting height with a backrest affords sitting and lingering, while a narrow ledge at standing height affords leaning or perching briefly. |||
| Stairs & Ramps || Steps afford climbing; a gently sloped surface with handrail affords wheeling and walking for more people, extending the affordance of access. |||
| Playground / urban furniture || Low walls and broad steps in a plaza afford sitting and gathering, not just circulation, inviting social use beyond their original function. |||
| Bottom sheet || iOS bottom sheets show a small horizontal "grab bar" at the top, affording dragging up or down to expand/dismiss the sheet. |||
| Block editor || Notion reveals a "+" button and a six-dot drag handle on hover next to each block, affording both inserting new blocks and rearranging existing ones. |||
| Design tool handles || Figma shows corner and edge handles when an object is selected — corners afford uniform scaling, edges afford one-axis resizing, and a rotate handle sits just outside each corner. |||
| Message actions || Slack reveals reaction, reply-in-thread, share, and more icons when you hover a message, affording contextual actions without cluttering the default view. |||
| Media card || Spotify album art darkens and overlays a circular play button on hover, affording one-click playback of the whole album or playlist. |||
| Calendar slot || Google Calendar shows empty time slots as subtly tinted rectangles; clicking one creates an event — the grid cell itself affords event creation. |||
| Swipe gestures || iOS Mail shows a peek of colored archive/trash actions as you pan a message partially, teaching that rows afford horizontal swipes. |||
| Highlight toolbar || Medium shows a floating formatting toolbar (bold, italic, link, quote) above selected text, affording in-context styling without leaving the flow. |||
| Toggle switch || An iOS toggle resembles a physical rocker switch with a circular thumb that slides left/right — its form affords the two-state interaction. |||
| Accordion chevron || A downward-pointing chevron next to a section title affords expansion; after clicking, the chevron rotates upward to afford collapse. |||
| Draggable card || Trello cards lift slightly with a shadow on hover and rotate a few degrees on drag, making clear they're movable physical-feeling objects. |||
| Filter chip with X || A rounded pill with a small "×" icon at its right edge affords both "this is an active filter" and "tap the × to remove it". |||
| Dropdown arrow || A small downward caret next to a label affords "click to open a list", distinguishing dropdowns from static labels. |||
| File attachment || A paperclip icon next to a text input affords attaching files to a message; drag-and-drop zones on the same input extend that affordance. |||
| Color swatch || A circular color chip with a subtle border and hover lift affords "tap to select this color" in design tools and pickers. |||
| Keyboard shortcut hint || Linear shows faded key caps ("⌘K") next to menu items, affording keyboard invocation for users who prefer that path. |||
| Resizable pane || A vertical divider between two panels becomes a draggable handle on hover (cursor changes to ⇔), affording layout customization. |||
| Progress ring || Apple Watch activity rings invite you to "close them" — the incomplete shape itself affords the act of filling via more movement. |||
| Faucet handle || A cross-shaped faucet handle affords turning with a flat palm, while a single lever affords pushing up/down and sideways — hardware shape maps to gesture. |||
| Gear shift knob || A rounded, fist-sized ball with a shift-pattern label affords grasping and moving in specific directions, with the pattern itself teaching the action. |||

- - -

## Constraint

The interface should gently prevent impossible or dangerous actions (disabled states, valid ranges) and reduce the chance of mistakes.

**› Applied Example**

*Date picker disallows past dates for a future booking and greys them out; invalid fields show inline errors.*

**› Not Applied Example**

*Open text field for “Quantity” accepts letters and huge numbers; users submit impossible orders and hit server errors.*

**› More Examples**

| Domain || Applied || Not Applied ||
|:--|:--|
| Signup form || Required fields marked, button disabled until all are valid; password rules enforced inline to prevent bad submissions. || All fields look optional, button always enabled; errors appear only after submit, allowing weak passwords and broken accounts.||
| Date picker || Past dates and impossible ranges (checkout before check‑in) are disabled so only valid bookings are selectable. || Calendar lets you pick any dates; invalid ranges trigger cryptic error dialogs after the fact, causing user frustration.||
| Step‑by‑step wizard || Later steps locked until prerequisites are done (e.g., verify email before payment), enforcing a safe sequence. || User can jump straight to payment, then fails or loses data because identity or essentials weren’t captured earlier.||
| Content length || Character and ratio limits keep posts concise and visually consistent, avoiding layout breaks. || No limits: giant text blocks and odd image sizes break the feed layout and overwhelm readers.||
| Role‑based UI || Only admins see destructive actions; regular users are constrained from critical operations. || Everyone sees “Delete org” or “Reset database” and can click it, leading to accidental catastrophic changes.||
| Shape sorter toy || Only matching shapes fit the holes, physically preventing incorrect placement. || All holes are oversized rectangles; any piece fits anywhere, so the toy gives no guidance or learning signal.||
| USB‑C connector || Geometry constrains insertion so plug only goes in correctly, preventing damage. || A loose multi‑port with ambiguous shapes lets users force cables in misaligned, bending pins and causing failures.||
| Medication packaging || Blister packs and child‑resistant caps constrain easy access, requiring deliberate effort. || Simple screw caps or pop‑off lids; kids can open bottles quickly, increasing poisoning risk.||
| Turnstiles || One person per tap, physical gate constrains passage and enforces fare payment. || Open corridor with just a “Please pay” sign; people flow through freely, evasion is easy, counting is impossible.||
| Guardrails & paths || Railings and marked paths constrain movement near drops or machinery, guiding safe routes. ||Open edges with no railings; people can walk right to the edge, take risky shortcuts, and fall or enter danger zones.||
| Number input stepper || Quantity uses +/− stepper bounded at min 1, max in-stock, so users can never enter 0 or 999 by accident. || Free-text quantity field accepts "abc" or "9999", triggering server errors or fraud flags after submit. ||
| Credit card expiry || Expiry dropdowns only list future months/years within the card's valid window, preventing impossible dates. || Free-text expiry "MM/YY" accepts "13/99" and fails validation deep in the processor, after checkout. ||
| File upload filter || `accept="image/png,image/jpeg"` hides non-image files in the system picker, blocking the wrong-format case upstream. || Any file can be selected; backend rejects it after upload wastes bandwidth and user time. ||
| Character counter || Twitter/X shows a live count with a warning arc turning red past 280 chars, constraining length visibly as you type. || Unbounded text area silently allows a 5000-char novel; submit button returns "too long" with no hint where. ||
| Layer lock (design tool) || Figma lets you lock a layer so accidental drags/edits are blocked; the lock icon makes the state visible. || Every layer is editable; a stray click reshuffles the shared design system file for 20 teammates. ||
| CI merge gate || GitHub disables the Merge button when required checks fail, preventing broken code from reaching main. || Merge is always enabled; the pipeline goes red on main after a bad PR slips through. ||
| Destructive confirmation || Deleting an S3 bucket requires typing the bucket name to confirm — intentional friction on irreversible actions. || A single "Delete" button with a generic "Are you sure?" yes/no dialog that gets dismissed reflexively. ||
| Biometric gate || Apple Pay requires Face ID or Touch ID for purchases over a threshold, constraining large spends to verified users. || One-tap "Buy" with no re-auth; a borrowed phone can rack up charges instantly. ||
| Session timeout || Banking apps auto-log out after 5 minutes idle, constraining the window of exposure if the device is abandoned. || Indefinite session; an unattended phone at a café exposes full account access for hours. ||
| Rate limiting || GitHub API limits 5000 requests/hour per token, constraining accidental infinite loops and abuse. || No limits; one buggy script brings down the service for everyone. ||
| Permission scopes || OAuth apps request specific scopes (email, contacts) that limit what's accessible — granular user consent. || Apps ask for "full access" or nothing, forcing users to over-grant or abandon. ||
| Read-only mode || Google Docs "View only" and "Comment only" modes constrain readers from accidental edits. || Anyone with the link can edit; document state is at the mercy of any clumsy viewer. ||
| Typed confirmation || Heroku requires typing the app name to delete it, and Git requires `--force` to overwrite branches — cost-of-error scales with damage. || One-click delete buttons for production databases, next to cancel — symmetric UI for asymmetric outcomes. ||
| Input mask || A phone field auto-formats "+1 (555) 123-4567" and rejects letters, constraining the shape at entry time. || Free-text phone field accepts anything; downstream SMS fails silently. ||
| Plan-based limits || Free tier caps projects at 3 with clear messaging; upgrade path shown instead of silent failure. || Free tier creates 4th project successfully but breaks in a later flow, leaving users confused about what's allowed. ||
| Age gate || Streaming platforms require DOB before playing rated content, constraining access to age-appropriate material. || Content plays immediately with just a "Are you 18?" Yes/No — trivially bypassed. ||
| Speed bumps || Residential streets use physical bumps to force slower driving past schools and homes. || Signs saying "Slow down" with no physical enforcement; drivers speed through anyway. ||
| Keyed plugs || Grounded plugs and polarized sockets only fit one orientation, preventing miswired connections. || Symmetric two-prong plugs allow reversed polarity, risky for sensitive electronics. ||
| Anti-scald valve || Shower mixers with an internal stop prevent the handle from going past a preset max temperature. || Free-rotating mixers allow 70°C water, scalding children in a moment. ||
| Scaffolding toe boards || Short vertical boards at the base of platforms prevent tools and debris from being kicked over the edge. || Open platform edges; dropped wrenches become projectiles for workers below. ||

- - -

## Mapping

Controls should map naturally to results (e.g., left slider = move left, top item = appears first) so users can predict outcomes.

**› Applied Example**

*Media player uses left/right arrows for previous/next, vertical slider where up = louder, matching physical controls.*

**› Not Applied Example**

*Four stove-like controls (or light switches) arranged in a row but controlling a 2×2 grid layout, forcing trial‑and‑error.*

**› More Examples**

| Domain || Example |||
|:--|:--|
| Video player timeline || A horizontal scrubber represents time from left (past) to right (future); dragging the handle right moves the video forward, matching our mental model of timelines. |||
| Mobile volume slider || A vertical slider where up = louder and down = quieter, mirroring physical volume keys and common metaphors of “higher” meaning more. |||
| Carousel navigation || Left arrow moves to previous item, right arrow to next; dots are laid out horizontally in the same order as items, so position on the bar maps to position in the sequence.|||
| Map zoom controls || Pinch out to zoom in and pinch in to zoom out; the gesture directly maps to the content “coming closer” or “moving away” visually on screen.|||
| Multi‑column layout editor || Column width handles are dragged inside the layout itself; moving a divider left/right immediately reshapes adjacent columns, so the control’s location matches the effect area.|||
| Stove burner controls (industrial) || Four knobs arranged in a 2×2 grid that matches the physical layout of four burners; top‑left knob controls top‑left burner, etc., so spatial arrangement maps one‑to‑one.|||
| Car seat adjustment || Seat‑shaped control on the side of a car seat: pushing the front of the control moves the real seat forward, pushing the back moves it backward, matching the seat icon’s shape.|||
| Faucet temperature || Dual‑handle faucet with red handle on the left and blue on the right, where turning left increases hot water and right increases cold, mapping color and direction to temperature.|||
| Building elevator panel || Floor buttons arranged vertically in numeric order; higher floors placed higher on the panel so pressing “10” (higher button) feels like going up.|||
| Wayfinding signage || Overhead signs placed on the side of the corridor that corresponds to the direction of the destination (e.g., “Gates A1–A10 →” on the right side), mapping spatial position of sign to direction of travel.|||
| Brightness slider (iOS) || The vertical brightness slider literally fills up as brightness increases — the amount of light on screen is mirrored by the fullness of the control. |||
| Text alignment icons || Align-left, center, right, and justify buttons display miniature lines arranged exactly the way the text will look after the action — the icon is a preview. |||
| Bold / Italic buttons || The "B" button is rendered bold, "I" is italic, "U" is underlined — the control visually embodies its effect. |||
| Color picker hue slider || A rainbow gradient where the thumb position maps directly to the selected hue on the color wheel — drag to a position, get that exact color. |||
| Indent / outdent (Notion) || Arrow pointing right indents a block (moves text right); arrow pointing left outdents — direction of arrow = direction of content movement. |||
| Align buttons in design tools || Figma's align-left, align-top, distribute-horizontally buttons use arrows and edges that visually describe the spatial result. |||
| Music EQ sliders || Vertical sliders arranged left-to-right across frequency bands (bass → treble); raising a slider raises that frequency's gain — position maps to pitch and amplitude. |||
| Mouse cursor || Moving the mouse right moves the cursor right on screen — physical gesture 1:1 with digital response across any distance. |||
| Steering wheel || Turning the wheel clockwise steers the car right; the angular direction of the hands maps to the angular direction of the vehicle. |||
| Upload / Download arrows || Up-arrow icons for upload (content leaving your device, going "up" to server) and down-arrow for download — direction matches mental model of "the cloud is up there". |||
| WiFi / signal bars || Taller bars = stronger signal; the vertical amount maps to signal strength so glancing is enough. |||
| Battery icon || A filling green bar inside a battery silhouette maps remaining charge to visible fullness — universal across devices. |||
| Airplane mode icon || An airplane silhouette represents the state where only in-flight-safe radios are active — the icon maps to the context where the mode matters. |||
| Playback controls || ⏮ rewind, ⏯ play/pause, ⏭ forward arrows point in the direction of time they affect — the glyph is a compass for time. |||
| Sort direction arrow || A column header with ↑ means ascending, ↓ descending — arrow direction maps to the sort order's direction in the list. |||
| Presentation transitions || Keynote's "Push from right" transition visually pushes slide A left as slide B enters from the right — the name, direction, and motion all align. |||
| Haptic directional feedback || Apple Watch uses a tap pattern that moves "left" or "right" along your wrist during navigation — the sensation maps to the turn direction. |||
| Tilt-based game controls || Racing games steer via device tilt: tilt left, car goes left — the physical gesture maps to the in-game outcome without any learning curve. |||
| Calendar layout || Week view goes left-to-right Monday → Sunday matching how most cultures write time; today is highlighted with a colored cell — spatial = temporal. |||
| Thermostat dial || Turning a Nest dial clockwise raises the target temperature, counterclockwise lowers it, and the ring colors shift red → blue — direction and color map to heat. |||

- - -

## Consistency

Reuse patterns, layouts, and behaviors so users can transfer knowledge across the product and feel in control.

**› Applied Example**

*Mobile app reuses same bottom nav, icon style, and interaction patterns across all screens and platforms.*

**› Not Applied Example**

*“Save” is a checkmark in one view, a floppy icon in another, and auto‑save elsewhere, leaving behavior unpredictable.*

**› More Examples**

| Domain || Example |||
|:--|:--|
| Design system buttons || All primary actions use the same color, corner radius, size, and label style across web and app, so “primary button = main next step” everywhere. |||
| Navigation patterns || Every product in a suite uses the same top bar pattern (logo left, search center, profile menu right), so users instantly know where to look. |||
| Form Patterns || All forms use the same label position, error color, helper text style, and success state, reducing cognitive load when filling different flows.|||
| Iconography || Icons share stroke weight, corner style, and metaphor (trash = delete, magnifier = search) across all screens, avoiding conflicting meanings.|||
| Interaction Feedback || Hover, pressed, focus, and loading states behave identically for all buttons and links, so one learned pattern applies everywhere.|||
| Industrial Product Family || A company’s appliance line (oven, microwave, dishwasher) uses the same knob logic, icon sets, and display language, so learning one helps you use the others.|||
| Car Dashboard || Turn indicators, wiper controls, and light controls are in consistent locations across model years, preserving muscle memory for drivers switching cars.|||
| Building Signage || All wayfinding signs in a campus use the same typeface, arrow style, color code, and hierarchy, so once you decode one sign, the rest are effortless.|||
| Urban Furniture || Benches, bus stops, trash cans, and bike racks share a coherent material palette, color, and construction logic, making the system legible as one family.|||
| Architectural Details || Door hardware, switches, and finishes repeat rules (e.g., all bathrooms have the same fixtures, layout logic, and symbols), so occupants quickly learn what to expect room to room.|||
| Human Interface Guidelines || Apple HIG standardizes navigation bars, action sheets, tab bars across all iOS apps — switching apps doesn't require relearning where controls live. |||
| Material Design || Android apps built on Material share elevation, motion, and component behavior, so a user fluent in Gmail is also fluent in Google Calendar. |||
| Payment flow pattern || Stripe's card → expiry → CVC → ZIP order is reused by most web checkouts, so returning users can fill it from muscle memory. |||
| Keyboard shortcuts || Figma's ⌘D duplicates, V selects, T adds text — identical across web and desktop apps, preserving power-user muscle memory between platforms. |||
| Google account chip || A profile avatar at top-right opens account switcher across Gmail, Drive, Docs, YouTube, Calendar — a single learned pattern for identity management. |||
| SaaS sidebar || Slack, Linear, Notion, and Figma all use a left sidebar with workspace picker at top, navigation middle, and user/settings at bottom — learning one teaches the pattern. |||
| iOS Settings list || Every Settings pane uses the same grouped table view with section headers, disclosure arrows, and toggles — new apps slot into this template seamlessly. |||
| Amazon "Buy now" || The yellow Buy-now button sits in the same place on every product page and behaves identically across categories, books → electronics → groceries. |||
| Airbnb listing card || Image carousel, title, rating, price-per-night always in the same positions in search, favorites, and past trips — pattern recognition is instant. |||
| Office ribbon || Microsoft Word, Excel, and PowerPoint all use the ribbon with File / Home / Insert tabs; learning one app's ribbon structure transfers to the others. |||
| E-commerce PDP || Image left, title and price top-right, add-to-cart below, reviews at the bottom — this template is so consistent across Amazon, Shopify stores, and Flipkart that users feel at home anywhere. |||
| Video player controls || Play/pause bottom-left, volume next to it, time code center, fullscreen bottom-right — YouTube, Netflix, Vimeo, and Prime Video converge so hands know where to go without looking. |||
| Messaging layout || Conversation list left, chat center, details right — WhatsApp, iMessage, Slack, Teams, Discord all use this structure, making switching chat apps low-effort. |||
| Music streaming nav || Spotify, Apple Music, YouTube Music, Amazon Music all offer Home / Search / Library tabs — the mental model transfers across services. |||
| Social profile pattern || Twitter/X, LinkedIn, Instagram, GitHub all show avatar, name, bio, stats, and a feed below — new networks slot into a known template. |||
| Error states || An error banner with a red icon, title, description, and retry CTA is used consistently across a product so "something went wrong, here's what to do" is recognizable. |||
| Empty states || Same illustration style, title, description, and primary CTA pattern used for empty inbox, empty search, empty list — unfamiliar screens feel familiar. |||
| Loading states || Shimmer skeletons in the shape of content everywhere in the app, never a spinner-in-the-middle in one view and a skeleton in another. |||
| Date / time format || One format (e.g., "Apr 24, 2026 · 3:42 PM") used in emails, logs, exports, headers — users don't reparse the format each time. |||
| Currency formatting || ₹1,23,456.78 (Indian numbering) or $1,234,567.89 (US) used uniformly; mixing formats within the same product erodes trust and increases errors. |||

- - -

## Simplicity

Show only what’s necessary at each moment, remove decorative noise, and structure tasks so they’re mentally lightweight.

**› Applied Example**

*Onboarding shows one task per screen with clear primary action, progressive disclosure for advanced options.*

**› Not Applied Example**

*Dashboard crams charts, filters, promos, tooltips, and chat widget into one view; users can’t see what to do first.*

**› More Examples**

| Domain || Example |||
|:--|:--|
| Search experience || Google's homepage is a logo, a search bar, and two buttons — decades of restraint pay off because the one thing you came for is obvious. |||
| Focused writing tool || iA Writer hides formatting, sidebars, and chrome while you write; the page is just text, cursor, and word count — attention is on the sentence. |||
| Reading app || Kindle removes chapters, nav, and toolbars while reading, leaving only text and page turn — the device disappears into the book. |||
| Meditation app || Headspace opens with one large "Press to start" circle instead of a course catalog, reducing the friction to actually meditating. |||
| Onboarding pattern || Duolingo asks one question per screen ("What's your goal?", "How much time?") — each choice is a single decision, never a wall of options. |||
| Single-question forms || Typeform shows one question at a time with big typography and smooth transitions, turning a 20-question form into 20 small, clear moments. |||
| Minimal dashboard || Linear's inbox and active issues view hides everything non-essential; keyboard shortcuts replace visible menus, keeping pixels for content. |||
| Swipe-first UI || Tinder reduces a dating profile to one card, two gestures — infinite options collapse into a single decision per moment. |||
| Wearable UI || Apple Watch screens each host one primary interaction (complication, dial, confirm) — a tiny display forces ruthless scoping. |||
| Calculator app || iOS Calculator shows digits, operators, and result — no history, no chrome — because the task is unambiguously arithmetic. |||
| Mobile onboarding || Notion's empty state is a blinking cursor and a "/" hint — no tour, no modal, the feature teaches itself through use. |||
| Landing page hero || Stripe's homepage leads with one sentence and one CTA before any navigation expands — visitors aren't forced to parse the whole product upfront. |||
| Smart speaker || An Amazon Echo has one button and a ring of LEDs; everything else is voice — the product's surface area is radically smaller than a phone. |||
| Thermostat || The Nest thermostat is one dial and a single temperature reading — a household appliance distilled to its core task. |||
| Vacuum robot || A Roomba's primary interface is one "Clean" button; scheduling and mapping live in an optional app for users who want them. |||
| Camera app (iPhone) || Opens to a viewfinder with one shutter button; modes live in a horizontal swipe row — the primary task is one tap away. |||
| Messaging compose || iMessage's compose view is a text field and send button — everything else (media, effects) is behind one + icon. |||
| Single-task appliances || A MUJI kettle has one switch; nothing to learn, nothing to misread, nothing to break. |||
| Dieter Rams radios || Braun's T3 pocket radio shows only the dial, a tuning window, and a single selector — a lesson in removing everything inessential. |||
| Tadao Ando architecture || Interior spaces built of raw concrete, a single slit of light, and empty volume — the architecture recedes so the experience of the moment dominates. |||
| Japanese ticket machine || A fare map above the machine plus large coin/bill slots; no chrome, no upsells — the one action (buy a ticket) is direct. |||
| Minimalist product page || Apple product pages use huge imagery, short headlines, and one price + buy button — decisions are about the product, not the layout. |||
| Wizard pattern || TurboTax walks users through one question per screen ("Do you have W-2 income?") instead of a 40-field form — complexity is revealed in time. |||
| Status page || A SaaS status page says "All systems operational" as the hero state — if nothing is wrong, nothing else needs to be said. |||
| Notification pattern || Slack's "Do Not Disturb" has a single toggle with a duration picker — the feature is one concept, one control. |||
| Checkout button || Gumroad's single-page checkout is email + card + buy — three fields and done, optimized for the single goal of completing the purchase. |||
| Kindle device || Only an e-ink screen and a few hardware buttons; no notifications, no color, no browser — the device is designed to do one thing and not distract from it. |||
| Bookmarking tool || Pocket's save flow is one tap in a share sheet — no tags, no folders required, the essential action first, optional metadata later. |||
| Bento boxes || A traditional Japanese bento box physically separates a meal into clear compartments, removing the decision of "how much of what" at mealtime. |||
| Voting booth || A well-designed ballot has one question per page with large checkboxes and plain language — a high-stakes task made cognitively light. |||
| Single-button mouse || The original Mac mouse had one button; anything that could be clicked was clickable the same way, zero learning curve. |||
| Reading glasses rack || Chemist stores sort glasses by diopter on a simple grid with a try-on mirror — one dimension (strength), one decision, no staff needed. |||
| Chopsticks || Two sticks, no mechanism — the "interface" for a complex activity (picking up varied foods) is radically minimal and endlessly adaptable. |||

- - -

## Learnability

A good interface teaches itself. First-time users should be able to pick it up through discoverable cues, familiar patterns, empty states, tooltips, and gentle onboarding — and experienced users should remember how to use it weeks later without relearning.

**› Applied Example**

*A new user opens Figma for the first time and sees a sample file, contextual tooltips on tools, and a "Getting started" panel; hovering any icon reveals its keyboard shortcut, so the tool teaches itself while being used.*

**› Not Applied Example**

*A pro video editor throws the user into a blank timeline with 50 densely packed tools, no tooltips, no starter template, no hint of where to begin — users bounce within minutes.*

**› More Examples**

| Domain || Example |||
|:--|:--|
| Language learning app || Duolingo starts with the easiest words, introduces one grammar concept at a time, and rewards progress with streaks — difficulty climbs just ahead of ability. |||
| Design tool onboarding || Figma opens a sample file for first-time users with labeled layers explaining components, frames, and auto-layout — users learn by poking at a living example, not reading docs. |||
| Chat product || Slack's Slackbot DMs new users with a conversational setup ("Want to upload a profile photo?") — onboarding hides inside a natural chat flow. |||
| Empty state as teacher || A project management app's empty board says "Create your first task" with an arrow to the + button and a 30-second example — the absence of content becomes a lesson. |||
| Keyboard shortcut discovery || Gmail's "?" key opens a comprehensive shortcut cheat sheet; Linear prints shortcuts next to every menu item — the power layer is always one hint away. |||
| Contextual tooltips || Notion shows a "/" slash-command hint in empty blocks ("Type / for commands") — the feature teaches itself at the moment of need. |||
| Template library || Canva's homepage shows thousands of starter templates by use case (Instagram post, resume, invitation); users remix rather than start from a blank canvas. |||
| Sample projects || CodePen, Glitch, and Replit ship with runnable example projects; learners fork and modify rather than decoding a README. |||
| Progressive disclosure || Photoshop offers "Essentials", "Photography", and "Painting" workspace presets so beginners see 15 tools and pros see 80 — the learning curve is configurable. |||
| Product tour || Stripe Dashboard runs a guided "Welcome" tour highlighting the first three actions: create a product, accept a test payment, view the ledger — one flow at a time. |||
| Feature hints || Arc Browser drops subtle "Did you know?" cards in low-traffic moments ("Try ⌘T to open a new tab") — hints at teachable moments without being intrusive. |||
| Git UI || GitHub Desktop guides brand-new users through "clone a repository", "make a commit", "push" with visual steps — command-line Git's notorious curve is flattened to buttons. |||
| Error as lesson || React's error overlay tells you exactly which file, line, and component threw, with a link to docs — errors become tutorials. |||
| Shortcut prompting || Superhuman's onboarding spends 30 minutes teaching 15 keyboard shortcuts with a real coach; the product is hard to learn, and they lean in instead of hiding it. |||
| Undo as safety net || Google Docs, Figma, and VS Code make ⌘Z infinite — users learn by experimenting without fear, because nothing they do is permanent. |||
| Video walkthroughs || Loom embeds contextual short videos in settings pages ("How to invite your team — 45 sec") so text instructions have an optional visual. |||
| In-app coachmarks || A new feature gets a one-time coachmark pointing to its location on release day, then quietly retires — the feature announces itself once. |||
| Interactive onboarding || Intercom's "Product Tours" feature lets any SaaS build clickable walkthroughs: try the real product with a gentle assistant guiding your hand. |||
| Microcopy teaching || An upload field that says "PNG or JPG, up to 10 MB" teaches the rule inline, so the user never sees the "unsupported format" error. |||
| Form helper text || A password field with live requirement checklist ("✓ 8 characters  ✗ 1 number") teaches the policy while enforcing it. |||
| Recognize over recall || Gmail's autocomplete in To: shows recent contacts — users recognize a name rather than remembering an email address. |||
| Reveal-on-hover || Notion's drag handles and + buttons appear only on hover, so the UI is clean for experts but discoverable for new users who explore with the mouse. |||
| Inline examples || GitHub's PR description field shows a collapsed example template — new contributors see the expected structure without reading the contributor guide. |||
| Video game tutorial || Nintendo's Mario and Zelda introduce mechanics in enclosed "safe rooms" that quietly teach through level design — no text tutorial needed. |||
| Microwave presets || A "Popcorn" or "Reheat" button encodes the right time and power for common tasks; users don't need to learn wattage math. |||
| Car dashboard icons || Universal symbols (fuel pump, engine warning, seatbelt) mean new drivers can decode alerts in any car — the icon set is the lesson. |||
| Home appliance labels || IKEA instructions with only diagrams teach assembly regardless of language — the grammar of arrows and numbered steps is universal. |||
| Museum audio guide || A numbered exhibit with matching audio prompts ("Press 12 for the Mona Lisa") makes a building with 35,000 artworks learnable in a single visit. |||
| Public library signage || Dewey Decimal and color-coded shelf labels, plus self-serve kiosks with "How to find a book" animations, teach the system through use. |||
| Airport signage progression || Signs escalate in specificity as you walk: "Gates" → "Gates A1–A40" → "A23 →" — the wayfinding system teaches itself by progressive narrowing. |||
| Restaurant menu structure || Grouping by course (Starters, Mains, Desserts) and price range teaches the cuisine's structure and order of decisions — no explanation needed. |||
| Apprentice model (trades) || A carpenter's workshop layout (cut zone → join zone → finish zone) teaches the workflow order through spatial arrangement. |||

- - -

## User Control

Users should feel in charge. Give them a clear way to undo, cancel, skip, customize, override, or exit at every step — and never trap them in a state they didn't choose. The system serves the user, not the other way around.

**› Applied Example**

*Gmail shows an "Undo send" snackbar for 5 seconds after sending; drafts are autosaved; any action can be reversed with ⌘Z; and the user can skip onboarding, mute threads, or customize keyboard shortcuts to their taste.*

**› Not Applied Example**

*An app auto-updates overnight without asking, loses open tabs, plays a tutorial video on every launch that can't be skipped, and shows autoplay video ads that unmute every time the page loads.*

**› More Examples**

| Domain || Example |||
|:--|:--|
| Undo everywhere || Figma, Google Docs, and VS Code all keep infinite undo history; users explore freely knowing any action is reversible. |||
| Undo send || Gmail's "Undo send" gives 5–30 seconds to retract a sent email — a single control that saves reputations daily. |||
| Draft autosave || Notion, Linear, and iOS Notes save every keystroke; closing the app mid-sentence loses nothing, putting the user in charge of when to stop. |||
| Cancel in progress || Browser "Stop" button, file copy "Cancel" — long operations are interruptible at any moment. |||
| Skip tutorial || Any onboarding with "Skip" in the top-right respects users who already know or want to explore — forced tutorials are a control violation. |||
| Back button || Web browsers and mobile apps preserve history; the universal Back button keeps users from feeling lost or trapped. |||
| Incognito / private mode || Browsers let users opt out of history and cookies for a session — a clear, named mode that restores privacy on demand. |||
| Mute / Do Not Disturb || OS-level DND silences notifications on the user's terms (scheduled, while driving, while presenting). |||
| Keyboard shortcut customization || Emacs, VS Code, and Figma let power users remap every shortcut — the product adapts to the user, not the reverse. |||
| Layout customization || Trello, Linear, and Jira let users reorder columns, pin views, and hide sections — the product conforms to the user's workflow. |||
| Dark mode toggle || macOS, iOS, and most modern apps give a three-way choice (Light / Dark / System) — visual preference is the user's, not the designer's. |||
| Notification preferences || Slack, Gmail, and LinkedIn offer granular per-category notification controls — users pick what's worth interrupting them for. |||
| Soft delete / Trash || Gmail's Trash, macOS's Trash, Figma's deleted pages panel — destructive actions are reversible for 30 days, so users are never one click from disaster. |||
| Escape closes modal || Pressing Esc dismisses dialogs in almost every OS and app — a universal exit hatch that keeps users from feeling stuck. |||
| Autoplay off || YouTube, Netflix, and Instagram all provide a toggle to disable autoplay; respecting users who don't want passive consumption. |||
| Snooze / remind later || Gmail and iOS Mail let users snooze an email until a chosen time — control over your own attention schedule. |||
| Logout everywhere || Google, Apple, and Stripe show active sessions with a "Sign out of all devices" option — users retain control of their identity across the fleet. |||
| Export your data || GDPR-inspired data export: Google Takeout, Apple's Data & Privacy, Notion's export — the user owns their data and can walk away. |||
| Readable download queue || Browsers show each download with pause / resume / cancel — long operations don't hold the user hostage. |||
| Right to opt out of emails || Every marketing email ends with an unsubscribe link — one-click recovery of the inbox. |||
| Confirmation with defaults || "Close without saving?" dialogs default to the safe option (Cancel), but the unsafe option exists — users stay in charge. |||
| Edit / delete your own content || Comments, posts, and messages in Reddit, Slack, and iMessage can be edited or deleted — the user's past expression is still theirs. |||
| Two-factor setup options || Authenticator app, SMS, security key, passkey — users choose the security method that fits their threat model. |||
| Privacy review prompts || iOS nudges users to review which apps still have location or contacts access — continual reconsent keeps control in the user's hands. |||
| Reduced motion / accessibility || OS-level toggles for reduced motion, larger text, bold text, increased contrast — the UI adapts to sensory preferences. |||
| Customizable feed || Mastodon and RSS readers give a chronological, unsorted feed; the algorithm's role is opt-in, not imposed. |||
| Override AI suggestions || GitHub Copilot suggests code with Tab to accept, Esc to dismiss — the AI proposes, the user disposes. |||
| Pause subscription || Apple Music, Netflix, and gym memberships with "Pause" options let users step away without losing their data and habits. |||
| Power / off switch || Every well-designed device has a clear off — the ultimate form of control. |||
| Chef's pass on food || A restaurant kitchen's "send it back" protocol treats the diner as the last authority on what leaves the pass. |||
| Car override || Modern cars with lane-keep assist let a firm steering input override the computer — the human stays the pilot. |||
| Emergency stop || Industrial machinery has a big red button within reach that halts everything — human control trumps automation. |||
| Thermostat manual override || Smart thermostats let users override the schedule for a few hours, then resume — automation is a default, not a mandate. |||

- - -

## Align Reality

Match the language, objects, workflows, and mental models of the user's real world. Use words they actually say, metaphors they already grasp, and sequences that mirror how things work outside the product.

**› Applied Example**

*A mail app uses "inbox", "sent", "reply", "forward" and an envelope icon — terms every user already knows. Trello mirrors a physical whiteboard with sticky notes: boards, lists, cards you drag between columns, matching the Kanban mental model one-to-one.*

**› Not Applied Example**

*A consumer app surfaces its internal jargon: "Provision a new artifact-bundle in the k8s pod" on the dashboard. Users have no existing concept to attach this to, so every click requires translation.*

**› More Examples**

| Domain || Example |||
|:--|:--|
| Email metaphor || Inbox, outbox, folders, archive, trash, reply, forward — all lifted from physical office mail, so nobody has to be taught what they mean. |||
| Kanban board || Trello, Jira, and Linear mirror a physical board with sticky notes moving through columns — the workflow is already understood from whiteboards. |||
| Shopping cart || Amazon, Shopify, and every e-commerce site use "cart", "checkout", "shipping", "billing" — all borrowed from grocery stores and mail order. |||
| Calendar views || Day / Week / Month / Year in Google Calendar, Apple Calendar, and Outlook match how people already think about time. |||
| Photo album || iOS Photos organizes by date and location, just like a physical photo album — no new concept to learn. |||
| Music library || Spotify and Apple Music use "album", "artist", "playlist", "library", "queue" — all from physical music consumption history. |||
| Desktop metaphor || Files, folders, desktop, trash, shortcuts — the entire OS UI is a virtual office desk that was immediately intuitive in the 1980s and still is. |||
| Recycle bin / Trash || Deleted items go to a visible bin you can still see into and restore from — matches how people actually handle paper they're "not sure" about throwing away. |||
| Book reader || Kindle and iBooks animate page turns and show page numbers — the digital book reads like the physical one it replaces. |||
| Maps orientation || Google Maps keeps north up by default (matching paper maps) but lets users rotate to match heading while driving — both mental models supported. |||
| Banking accounts || "Checking", "Savings", "Credit card", "Routing number" — all retained from paper banking, so new digital banks are instantly legible. |||
| Restaurant reservation || OpenTable asks for party size, time, and occasion — the same things a host asks on the phone. |||
| Video editor timeline || Premiere and Final Cut show horizontal tracks for video and audio, matching physical tape editing — editors coming from film feel at home. |||
| Audio waveform || Every DAW (Logic, Ableton, Pro Tools) shows audio as a waveform — a representation that matches how humans visualize sound in the abstract. |||
| Code editor || VS Code uses line numbers, tabs, panels, and projects — matching paper code and IDE conventions developers already know. |||
| Spreadsheet grid || Excel's A1, B2 row-column addressing matches the graph paper and ledger books it replaced — decades of users onboard for free. |||
| Presentation slides || Keynote and PowerPoint use the metaphor of physical slides and a presenter's deck — the language of "deck", "slide", "transition" predates computing. |||
| Image cropping || Photoshop's crop tool uses a rectangular selection with corner handles and a dimmed outer area — matches how photographers crop with cardboard L-frames. |||
| Real-world physics in motion || iOS's rubber-band scroll, Material's momentum scrolling, and bounce-at-edges mirror how physical objects behave with inertia and friction. |||
| Weather icons || Sun, cloud, rain, snow, lightning — universal symbols anyone can read before they can read. |||
| Mail-style conversations || Threaded reply views in Gmail match how paper letter exchanges feel — a stack of back-and-forth correspondence. |||
| Health metrics || "Steps", "heart rate", "sleep hours" — terms borrowed from doctors, fitness coaches, and sleep science, already in the cultural vocabulary. |||
| Photo filters named after film || Instagram's "Kodak", "Polaroid"-inspired filters borrow the aesthetic language of analog photography. |||
| Cooking timers || Kitchen apps use "minutes", "hours", "start", "stop", and an alarm sound — identical to the egg timer in the drawer. |||
| Door icons in apps || A hotel booking app uses a door + key icon for "check in" because that's how real check-in works. |||
| Checkout receipt || Online order confirmations mimic paper receipts: date, items, subtotal, tax, total, order number — the structure is a hundred years old. |||
| Architectural floor labels || Ground Floor / First Floor / Mezzanine in a building lobby sign matches how occupants talk about the space. |||
| Room naming || A smart home app calls rooms "Living room", "Bedroom", "Kitchen" — the words people already use at home, not "Zone A". |||
| Signage by color || Red = stop, Green = go, Yellow = caution — a color language with centuries of real-world reinforcement, used correctly in UIs with the same meaning. |||
| Navigation landmarks || Google Maps walking directions say "turn right at the Starbucks" because humans navigate by landmarks, not compass bearings. |||
| Cash register drawers || Physical POS systems open a cash drawer at the end of a sale — the sequence matches what customers and staff expect from muscle memory. |||
| Filing cabinet in software || Evernote and Bear use notebooks, notes, tags — a hybrid of filing cabinets and index cards, so writers transfer workflow 1:1. |||
| Unit selection || Dieting apps let users pick "cups", "grams", "ounces" — meeting users in whichever unit they grew up measuring. |||
| Calendar holidays || Any good calendar app shows regional holidays localized to the user's country — aligning with the real calendar the user lives by. |||

- - -

## 🎯 Principles in Action — Airbnb Booking Flow

Below is a real-world, best-in-class flow — **Airbnb's booking journey** — walked screen by screen, with every principle highlighted at the moment it's working.

> **Tip:** the HTML version of this document makes this flow clickable screen-by-screen. In markdown, read it top to bottom.

### Screen 1 of 7 — Search (Home)

*The user lands on Airbnb with one goal: find a place to stay.*

| Principle || How it shows up here |||
|:--|:--|
| Visibility || The search bar is the largest element on the page ("Where are you going?"). Category pills (Beach, Cabins, Design, Tiny homes) scroll horizontally at top, exposing the range of inventory without a menu. |||
| Affordance || The search bar has a pronounced border, shadow, and the placeholder text is a direct question. The magnifier icon at the right looks clickable. |||
| Consistency || The listing card — image carousel, title, dates, price, rating — is the same template used on every Airbnb screen. Learn it once, recognize it forever. |||
| Simplicity || The homepage asks for one thing (a destination) and defers everything else (dates, guests, filters) to later screens or a modal. |||
| Align Reality || The vocabulary is human: "Where are you going?", "I'm flexible", "This weekend". The machine learns the user's language, not the reverse. |||

### Screen 2 of 7 — Search Results (Map + List)

*The user scans options on a map and in a list side by side.*

| Principle || How it shows up here |||
|:--|:--|
| Visibility || Prices show as colored pill labels on map pins; hovering a card lifts its pin. Both geography and catalog are visible simultaneously. |||
| Feedback || Hovering a listing card highlights its map pin; clicking a map pin opens a card preview — each interaction produces an immediate spatial echo. |||
| Mapping || A pin's position on the map is the listing's real-world latitude/longitude. The control and the outcome share the same coordinate system. |||
| Constraint || Filter sliders (price range, bedrooms) bound the selection to valid values. Impossible combinations never appear in the UI. |||
| User Control || Users can toggle list / map / split view, reorder by price or rating, save to wishlist, or clear all filters at any time. |||

### Screen 3 of 7 — Listing Detail

*A single property is opened; the user evaluates it.*

| Principle || How it shows up here |||
|:--|:--|
| Affordance || The pink "Reserve" button on the right-hand booking panel is the only primary-colored element — unmistakably the next action. |||
| Visibility || The sticky booking panel keeps price, dates, guests, and total visible as the user scrolls through photos and reviews — the decision-relevant information never leaves the viewport. |||
| Consistency || Every listing page has the same structure: photo grid → title/host → booking panel → highlights → description → amenities → reviews → map → rules. A familiar anatomy. |||
| Align Reality || Language is natural: "Host", "guests", "nights", "check-in / check-out", "house rules". These are the words travelers already use. |||
| User Control || Wishlist (heart icon), share, and back are all present in the header. The user can leave, save, or send the listing to a friend with one tap each. |||

### Screen 4 of 7 — Date & Guest Selection

*The user picks dates and confirms how many people.*

| Principle || How it shows up here |||
|:--|:--|
| Mapping || The calendar lays days out as a 7-column grid mirroring a real week; selecting a date feels like circling it on a paper calendar. |||
| Constraint || Unavailable dates are visually disabled (struck-through, greyed); minimum-stay rules auto-expand the selection to a valid range. Invalid states are impossible to construct. |||
| Feedback || As the range is selected, a colored band connects the start and end dates; the total price updates live in the booking panel. |||
| Visibility || A breakdown pops open showing base rate × nights + cleaning fee + Airbnb fee + taxes — the money flow is transparent before paying. |||
| Learnability || The calendar widget follows a near-universal pattern; users arrive already fluent because every travel site on earth uses it. |||

### Screen 5 of 7 — Review & Confirm

*A summary of the trip before payment.*

| Principle || How it shows up here |||
|:--|:--|
| Visibility || Full summary: trip dates, guest count, host name, ground rules, cancellation policy, total cost with line items. No hidden surprises. |||
| Constraint || "I agree to the House Rules" and cancellation policy acknowledgement are required before "Confirm & Pay" activates. |||
| Simplicity || One primary CTA. Edit links beside each section for small changes without restarting the flow. |||
| User Control || Each section has an "Edit" affordance; the user can adjust dates, guests, or payment method without abandoning and retrying. |||
| Feedback || The Confirm & Pay button is dim until prerequisites are met; active color returns when the form is valid — the gate is visible. |||

### Screen 6 of 7 — Payment

*Card details and billing.*

| Principle || How it shows up here |||
|:--|:--|
| Affordance || Input fields are clearly bordered with labels and placeholder format hints ("MM/YY", "CVC"). The card icon appears inside the number field. |||
| Feedback || Real-time card brand detection — a Visa, Mastercard, or Amex logo fades in as the first digits are typed, confirming the card type. |||
| Constraint || The expiry dropdown only lists future months and years; the CVC input is numeric-only with a 3–4 character limit; typos at this step are nearly impossible. |||
| Consistency || The payment UX is identical across experiences (booking, gift cards, Airbnb Experiences). Returning users fill it from muscle memory. |||
| Align Reality || Standard financial terms (Card number, Expiry, CVC, Billing address, ZIP) — the same language as every physical or online checkout. |||

### Screen 7 of 7 — Confirmation

*The booking is done.*

| Principle || How it shows up here |||
|:--|:--|
| Feedback || A large green check with "You're going to Lisbon!" — unmistakable success. A haptic tap on mobile, a celebratory micro-animation on web. |||
| User Control || The cancellation policy and a "Cancel reservation" link are immediately accessible in case of buyer's remorse. |||
| Align Reality || The confirmation reads like a real travel itinerary: destination, dates, host, address, check-in code — everything a paper booking confirmation would have. |||
| Learnability || A tips panel suggests the logical next steps: message the host, add the trip to a calendar, review the neighborhood guide. The product teaches its ecosystem at a useful moment. |||
| Simplicity || One status (Booked!), one primary next action (View trip). Supplementary info lives below the fold — available, not demanding. |||

> **Takeaway for designers:** every well-designed flow stacks 4–6 principles per screen. Principles don't compete — they reinforce. If a screen feels off, check which of the ten principles it's quietly breaking.

- - -

## Summary

| Principle | Goal ||
|:--|:--|
| Visibility | Make possible actions obvious. ||
| Feedback | Show clear results of every action. ||
| Affordance | Make controls suggest their use. ||
| Constraints | Prevent errors and impossible actions. ||
| Mapping | Align controls with outcomes intuitively. ||
| Consistency | Reduce learning by reusing patterns. ||
| Simplicity | Lower cognitive load and clutter.          ||
| Learnability | Make it easy to pick up and remember. ||
| User control | Let users feel safe and in charge. ||
| Align Reality | Align with user expectations, mental model, language and the way things work. ||
