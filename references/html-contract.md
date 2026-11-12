# Visual learning HTML contract

Create an editorial learning experience that feels authored for its subject. Visual design supports comprehension and reading comfort; a static diagram is preferable to animation when it explains equally well. A short article does not require a dashboard, a quiz or a complex interactive.

## Reference principles, not templates

- [Distill: Why Momentum Really Works](https://distill.pub/2017/momentum/) places the conceptual visual and controls near the question they explain. Borrow close integration of prose and visual evidence, generous reading space and clear chart labeling.
- [The Pudding: The Physical Traits that Define Men and Women in Literature](https://pudding.cool/2020/07/gendered-descriptions/) uses a subject-specific illustrated opening and a reader prediction before the analysis. Borrow the idea of a distinctive editorial point of view and a question that earns its place; do not reuse artwork or brand style.
- [Bartosz Ciechanowski: Bicycle](https://ciechanow.ski/bicycle/) develops a complex mechanism through simple scenes with direct manipulation. Borrow progressive explanation, clearly labeled cause and effect and small observable changes, not the original assets.

These are optional inspiration, not dependencies, and do not require network access during page use. Do not copy their logos, illustrations, interface designs or wording. Respect licensing when incorporating any third-party assets.

## Art direction

1. Decide the content's character and create a small, coherent design system: background, ink, one main accent, restrained secondary/status colors, typography, spacing and one motif derived from the article. Avoid default purple gradients, stock dashboard grids, repeated floating cards, oversized shadows and ornamental blobs unless the topic genuinely calls for them.
2. Establish hierarchy with a distinctive topic-bearing title, brief deck, unobtrusive provenance and clearly differentiated section headings. Use one readable CJK system font stack; a contrasting locally available serif or sans display face is optional. Do not rely on a remote font. Prefer normal body size around 16–18px, comfortable line-height around 1.6–1.9, and readable line length; adapt for script and content.
3. Create page rhythm through deliberate changes in width, spacing and visual density: a readable prose column; wider diagrams where warranted; captions close to visuals. Use whitespace to group related material, not as empty decoration. Vary section composition without breaking navigation and alignment.
4. Make illustrations, charts, callouts and controls feel part of the same page through consistent type, stroke, color and labels. Treat color as emphasis, not the only way to communicate meaning. Ensure body-text contrast at least 4.5:1 and large-text contrast at least 3:1, and retain clear focus indicators.
5. Responsive from 375px upward: reflow columns, legends and diagram labels; do not shrink complex desktop diagrams until illegible. Avoid horizontal document overflow, clipped text and tiny tap targets; aim for controls at least 44×44 CSS pixels when practical. Set viewport and document language; honor user zoom.

## Visual explanation

For each central idea, choose a proportional representation: annotated diagram for relationships, timeline for sequence, comparison for distinctions, or explanatory prose when a visual adds no value. A mechanism may use a stepper or a small interactive if it helps the reader answer a real question. Avoid repetitive decorative boxes.

If implementing a process, describe concrete input, actors, intermediate states and outcome; add branches only if real and relevant. Keep one shared state for labels, edges and visual highlights. Provide intuitive controls suited to the interaction; an animation must have pause and a complete static alternative, respect reduced motion and stop when offscreen. Make keyboard operation and state feedback accessible. Use original or appropriately licensed visuals, and label simulations and invented examples as such.

## Implementation and checks

- Use semantic sections and headings, UTF-8, appropriate `lang`, an unrestricted viewport, readable links and visible focus. Inline CSS/JS/SVG; no external dependencies by default. Essential content and static explanatory states must remain available without JS; print shows full content, including translation, outcomes and citations, while hiding playback controls.
- Escape HTML and attribute values by context, safely serialize any data embedded in scripts, insert dynamic source text with `textContent`, permit only appropriate HTTP(S) URLs for external links, and use `noopener noreferrer` on new-window links. Do not include source scripts, trackers or credentials.
- Inspect the actual desktop and narrow-screen output, hierarchy, prose measure, alignment, text wrapping, labels and controls. Exercise interactions, keyboard focus, reduced-motion, no-JS and print when the host supports them. Check every actual branch, source attribution and the accuracy of graphical relationships. Report unavailable verification; do not assert a pass without observing it.
