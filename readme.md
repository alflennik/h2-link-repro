# Reproduction of Screen Reader Link Bug

## Steps to Reproduce

- Open the repro.html file in Chrome.
- Turn on VoiceOver
- In VoiceOver, press "control + option + command h" to navigate to the first heading.
- VoiceOver will describe the h2 content includin the fact that it is a link.
- Press enter to activate the link.
- The link will fail to activate and the link will not change.

## Expected Behavior

When the screen reader describes a link, pressing enter is expected to activate it.

## Actual Behavior

In order to activate the link, VoiceOver requires users to "giggle" the cursor by pressing "control + option + right arrow" and then "control + option + left arrow". After that has happened, pressing "enter" will activate the link as expected.