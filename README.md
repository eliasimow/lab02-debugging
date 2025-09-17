
# Submission
- Create a pull request to this repository
- In the README, include the names of both your team members
- In the README, create a link to your shader toy solution with the bugs corrected
- In the README, describe each bug you found and include a sentence about HOW you found it.
- Make sure all three of your shadertoys are set to UNLISTED or PUBLIC (so we can see them!)

Ruben & Jacky teammates

https://www.shadertoy.com/view/wcsBDf

uv was used instead of uv2 -- found by connecting the zoomed in display to the original UV ratio

vec instead of vec2 -- compiler error, easy to find

resolution for calculating h -- observed that the screen was stretched, knew there had to be something wrong with raymarch.

increased march count to avoid warping while march slows by spheres -- noticed warping and that the ground wasn't being drawn as far back as it should. Assumed that, since the march worked properly until then, it was just an issue of distance. 

specular reflection direction was calculated with eye, not dir -- printed out some test values and determined that the used specular vec was bunk. Found it by observing.
