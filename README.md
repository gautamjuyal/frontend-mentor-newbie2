Created the project using pure css.
Flexbox was my go to move for almost all the stuff.
Now the challenging part, the hover state for NFT image.
I tried following approaches:

1. Using background property and img
 (a) Created the img-box div.
 (b) Assinged the nft image as background-image.
 (c) Assigned the given hsl cyan color as background-color.
 (d) View svg as added via img src tag.
Now the problem with this approach was that the image would get scaled up to cover the div, or the div would get smaller to fit the image size.

2. Using psuedo elements.
  (a) Created a psuedo element after.
  (b)Added a background image (view svg) and background-color (cyan) to it.
  (c) Set background repeat to no-repeat and background-position to center.
 
 NOW the challenge was to trigger pseudo element on hover.
 
 First apporach : Set initial scale for ::after 0;
                  Set scale as 1 on hover.
                 *The problem arose accordint to my specualtion : Any action can be triggered in a pseudo element only when it's parent element is clicked, hover, etc.

Second approach : Set display to none (absoute noob move)
                   Since the display was set to none, there was nothing to hover on to.
                   Thus this didn't work.
                   
Final approach: Set opacity for ::after as 0;
                Set opacity 1 on hover.
                
