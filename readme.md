# Reproduction of Screen Reader Link Bug

## Steps to Reproduce

- Open the [repro.html](https://raw.githack.com/alflennik/h2-link-repro/main/repro.html) file in Chrome, Firefox, Safari or Edge.
- Turn on VoiceOver on macOS or NVDA on Windows.
- In VoiceOver, press "control + option + command h" to navigate to the first heading. In NVDA, press "h" to navigate to the first heading.
- The screen reader will describe the h2 content including the fact that a link present.
- Press enter to activate the link.
- The link will fail to activate and the page will not change.
- Next, try the above steps with the [repro2.html](https://raw.githack.com/alflennik/h2-link-repro/main/repro2.html) file which shows equivalent behavior even when the h2s are wrapped with links (as opposed to links wrapping the h2s).

## Expected Behavior

When the screen reader describes a link, pressing enter would be expected to activate it.

## Actual Behavior

In order to activate the link, VoiceOver requires users to "jiggle" the cursor by pressing "control + option + right arrow" and then "control + option + left arrow". After that is done, pressing "enter" will activate the link as expected.